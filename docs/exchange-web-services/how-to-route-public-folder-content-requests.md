---
title: Rotear solicitações de conteúdo de pasta pública
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 59d2f05e-90fb-471e-ac06-70becc15b295
description: Todas as solicitações de informações de pasta pública que envolvem o conteúdo da pasta pública precisam ser encaminhadas para a caixa de correio de pasta pública que mantém o conteúdo da pasta de destino. Para encaminhar as solicitações para essa caixa de correio, você precisa definir os cabeçalhos X-AnchorMailbox e X-PublicFolderMailbox como valores específicos.
ms.openlocfilehash: 523b9c8efc65253f7970fffeb5800e451784522d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527731"
---
# <a name="route-public-folder-content-requests"></a>Rotear solicitações de conteúdo de pasta pública

Todas as solicitações de informações de pasta pública que envolvem o conteúdo da pasta pública precisam ser encaminhadas para a caixa de correio de pasta pública que mantém o conteúdo da pasta de destino. Para encaminhar as solicitações para essa caixa de correio, você precisa definir os cabeçalhos **x-AnchorMailbox** e **x-PublicFolderMailbox** como valores específicos. 
  
A tabela a seguir fornece uma visão geral do processo:
  
**Visão geral da pasta pública**

|Cabeçalho|O que eu preciso?|Como posso obtê-lo?|
|:-----|:-----|:-----|
|**X-AnchorMailbox** <br/> |1. [os valores x-AnchorMailbox e x-PublicFolderInformation](how-to-route-public-folder-hierarchy-requests.md) da caixa de correio de hierarquia de pasta pública.<br/><br/>2. o GUID da caixa de correio de pasta pública que contém o conteúdo da caixa de correio, que é enviado para o serviço de descoberta automática.<br/><br/>  O **AutoDiscoverSMTPAddress** na resposta Autodisover se torna o valor do cabeçalho **X-AnchorMailbox** .  <br/> ![FAZER](media/Ex15_PF_PFContent.png)| 1. Use o exemplo de código neste artigo, que [implementa a API gerenciada do EWS](#bk_determineguidewsma). Ou [use o EWS](#bk_determineguidews) e converta seus resultados para obter um GUID.<br/><br/>2. [faça uma solicitação de descoberta automática](#bk_makeautodrequest) usando o GUID mais o nome de domínio.<br/><br/>3. Use o valor do elemento **AutoDiscoverSMTPAddress** retornado na resposta de descoberta automática para [preencher o valor dos cabeçalhos](#bk_setheadervalues).  <br/> |
|**X-PublicFolderMailbox** <br/> |Seu trabalho é concluído, o valor X-PublicFolderMailbox é o mesmo que o valor X-AnchorMailbox!  <br/> |Você já tem!  <br/> |
   
Depois de determinar os valores de cabeçalho, inclua-os [quando fizer solicitações de conteúdo de pasta pública](#bk_setheadervalues).
  
As etapas neste artigo são específicas para solicitações de conteúdo de pasta pública. Para determinar se sua solicitação é uma hierarquia de pasta pública ou uma solicitação de conteúdo, consulte [Routing Public Folder](public-folder-access-with-ews-in-exchange.md#bk_routing)requests.

<a name="bk_determineguidewsma"> </a>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-the-ews-managed-api"></a>Determinar o GUID da caixa de correio de pasta pública usando a API gerenciada do EWS


Para determinar o GUID da caixa de correio de conteúdo de pasta pública, use o exemplo de código a seguir, que faz o seguinte: 
  
- Usa os cabeçalhos **x-AnchorMailbox** e **x-PublicFolderInformation** que você recuperou por [solicitações de hierarquia de pasta pública de roteamento](how-to-route-public-folder-hierarchy-requests.md).
    
- Chama o método [FindFolders](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) da API gerenciada do EWS e inclui uma solicitação para a propriedade **PR_REPLICA_LIST** (0x66980102) 
    
O valor **PR_REPLICA_LIST** identifica o GUID da caixa de correio da pasta pública que tem o conteúdo da pasta. A propriedade **PR_REPLICA_LIST** é uma matriz de bytes, mas é convertida como um GUID para este cenário. O GUID e o nome de domínio são concatenados para formar o endereço em que a descoberta automática deve ser chamada. 
  
Este exemplo pressupõe que `service` é o objeto [ExchangeService](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) para o usuário da caixa de correio `PFHAnchorHeader` e que `PFHMailboxHeader` são os valores dos cabeçalhos **x-AnchorMailbox** e **x-PublicFolderMailbox** , e o domínio é o nome do domínio usado pelo locatário. 
  
```cs
public static string GetMailboxGuidAddress(ExchangeService service, String PFHAnchorHeader, String PFHMailboxHeader, String domain)
{
    // Create a new folder view, and pass in the maximum number of folders to return.
    FolderView view = new FolderView(10);
    // Create an extended property definition for the PR_REPLICA_LIST property.
    ExtendedPropertyDefinition PR_REPLICA_LIST = new ExtendedPropertyDefinition(0x6698, MapiPropertyType.Binary);
    // As a best practice, limit the properties returned to only those required.
    // In this case, return the folder ID, the folder display name, and 
    // the value of the PR_REPLICA_LIST extended property definition.
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.DisplayName, PR_REPLICA_LIST);
    service.HttpHeaders.Add("X-AnchorMailbox", PFHAnchorHeader);
    service.HttpHeaders.Add("X-PublicFolderMailbox", PFHMailboxHeader);
    // Add a call to the CertificateValidationCallback method here if needed.
    // ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;
    // Call FindFolders to retrieve the folder hierarchy, starting with the PublicFolderRoot folder.
    // This method call results in a FindFolder call to EWS.
    FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.PublicFoldersRoot, view);
    string GuidAsString = null;
    List<string> Guids = new List<string>();
    // For each folder under the root, display the name, and copy the value of the 
    // PR_REPLICA_LIST byte array to a string value. 
    foreach (Folder folder in findResults.Folders)
    {
        Console.WriteLine("Public folder display name: {0}", folder.DisplayName);
        byte[] ByteArr = (byte[])folder.ExtendedProperties[0].Value;
        GuidAsString = System.Text.Encoding.ASCII.GetString(ByteArr, 0, 36);
        Guids.Add(GuidAsString);
        Console.WriteLine("Address for Autodiscover: {0}.{1}\r\n", GuidAsString, domain);
    }
    // Concatenate the GUID value of the PR_REPLICA_LIST with the domain name to generate the 
    // SMTP address to use for the AutoDiscover request for the public folder content mailbox.
    string AutoDSMTPAddress = GuidAsString + "@" + domain;
    // Check that all folders have the same GUID value. If they do not, use the GUID value of the
    // folder that you're requesting content for.
    string commonGuid = CompareGuidsForEquality(Guids);
    if (commonGuid == "Not Equal")
    {
        Console.WriteLine("The GUIDs for all the folders in the hierarchy are not the same. Run the Autodiscover sample using the address returned above that is associated with the folder in your hierarchy request.", AutoDSMTPAddress);
        return null;
    }
    else
    {
        Console.WriteLine("The GUIDs for all public folders in the hierarchy are the same. Run the Autodiscover sample using the {0} address.", AutoDSMTPAddress);
        return AutoDSMTPAddress;
    }
}
// Method to compare the GUID for each folder under the public folder root.
// If each GUID is the same, return the GUID.
// If the GUIDs are not the same, return "Not equal".
public static string CompareGuidsForEquality(List<string> list)
{
    string NotEqual = "Not equal";
    string first = list.First();
    return list.All(x => x == first) ? first : NotEqual;
}
```

Se você recebeu o erro "a solicitação falhou. A conexão subjacente foi fechada: não foi possível estabelecer uma relação de confiança para o canal seguro de SSL/TLS ", você precisará [Adicionar uma chamada a um método de retorno de chamada de validação](how-to-validate-a-server-certificate-for-the-ews-managed-api.md). Um espaço reservado e um comentário para esse método estão incluídos no exemplo de código.
  
Se o GUID da caixa de correio for o mesmo para todas as pastas públicas na raiz da pasta pública, o exemplo indicará o endereço a ser usado ao [chamar a descoberta automática](#bk_makeautodrequest) na saída do console e como o valor de retorno. Se o GUID da caixa de correio não for o mesmo para todas as pastas públicas na raiz da pasta pública, você precisará [fazer uma solicitação de descoberta automática](#bk_makeautodrequest) no endereço associado à pasta em sua solicitação de conteúdo. 

<a name="bk_determineguidews"> </a>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-ews"></a>Determinar o GUID da caixa de correio de pasta pública usando o EWS

O exemplo de código a seguir mostra como recuperar o valor da propriedade **PR_REPLICA_LIST** (0x66980102) usando a operação EWS [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) . Para o elemento [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) , o atributo **PropertyTag** é definido como o valor decimal (26264) da propriedade **PR_REPLICA_LIST** e o atributo **recordtypepropriedade** é definido como **Binary**.
  
Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa o método **FindFolders** para [determinar o GUID da caixa de correio de pasta pública usando a API gerenciada do EWS](#bk_determineguidewsma).
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0913.015
Accept-Encoding: gzip,deflate
Authorization: Basic c29ueWFmQGNvbnRvc28xMDAwLm9ubWljcm9zb2Z0LmNvbTpFWENIIzIwMTQ=
Host: outlook.office365.com
Cookie: ClientId=KZPBLKA9ZMPXAQDW
Content-Length: 1005
Expect: 100-continue
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:ExtendedFieldURI PropertyTag="26264" PropertyType="Binary" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="publicfoldersroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **FindFolder** com uma mensagem [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) que inclui o valor da propriedade estendida **PR_REPLICA_LIST** . Observe que o valor da propriedade aparece na resposta do EWS como o formato de cadeia de caracteres de uma matriz de bytes codificada em base 64. Alguns valores de cabeçalho na resposta são reduzidos para legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="1019" MinorBuildNumber="15" Version="V2_17" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body>
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="2" TotalItemsInView="2" IncludesLastItemInRange="true">
            <t:Folders>
              <t:ContactsFolder>
                <t:FolderId Id="AAEuAAAAAADL8shaNEKnQYVvRbpoY9vDAQBGDloItRzyTrAt+XVzRr/YAABdofPkAAA=" ChangeKey="AwAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/2h"/>
                <t:DisplayName>My Public Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x6698" PropertyType="Binary"/>
                  <t:Value>MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="AQEuAAADy/LIWjRCp0GFb0W6aGPbwwEARg5aCLUc8k6wLfl1c0a/2AAAAxEAAAA=" ChangeKey="AQAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/W/"/>
                <t:DisplayName>SampleFolder</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x6698" PropertyType="Binary"/>
                  <t:Value>MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

Para usar o valor do **PR_REPLICA_LIST** RETORNADO no XML, MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA = =, para determinar o GUID da caixa de correio, o valor deve ser convertido em um GUID em um formato semelhante à forma como o valor é convertido no [exemplo de código de API gerenciada do EWS](#bk_determineguidewsma). O GUID é concatenado com o nome de domínio para criar um endereço SMTP, que é incluído na [solicitação de descoberta automática](#bk_makeautodrequest).
  
## <a name="make-an-autodiscover-request"></a>Fazer uma solicitação de descoberta automática
<a name="bk_makeautodrequest"> </a>

Use o endereço retornado pelo `GetMailboxGuidAddress` método para chamar a descoberta automática. Recomendamos que você use o [Exchange 2013: obter as configurações do usuário com](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) o exemplo de código de descoberta automática para chamar o serviço de descoberta automática porque ele simplifica o processo de descoberta automática para você. Este exemplo de código usa os argumentos de linha de comando listados na tabela a seguir para chamar o serviço de descoberta automática do POX para recuperar o valor do [AutoDiscoverSMTPAddress](https://msdn.microsoft.com/library/office/dn750991%28v=exchg.150%29.aspx) associado ao GUID da caixa de correio. 

  
|**Argumento**|**Descrição**|
|:-----|:-----|
|emailAddress  <br/> |O endereço retornado pelo `GetMailboxGuidAddress` método em [determine o GUID da caixa de correio de pasta pública](#bk_determineguidewsma).  <br/> |
|-skipSOAP  <br/> |Indica que as solicitações de descoberta automática do POX são obrigatórias.  <br/> |
|-auth authEmailAddress  <br/> |O endereço de email do usuário da caixa de correio, que é usado para autenticação. Você será solicitado a inserir a senha do usuário da caixa de correio quando executar o exemplo.  <br/> |
   
Por exemplo, os argumentos de linha de comando devem ter a seguinte aparência:
  
`1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com -skipSOAP -auth sonyaf@contoso.com`

Em que `1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` é o endereço retornado pelo método **GetMailboxGuidAddress** e `sonyaf@contoso.com` é o usuário da caixa de correio. 
  
Quando você executa o **Exchange 2013: obter as configurações de usuário com** o exemplo de descoberta automática, a última resposta de descoberta automática deve ser bem-sucedida e incluir todas as configurações de usuário associadas ao GUID da caixa de correio. Salve a configuração de usuário do **AutoDiscoverSMTPAddress** localmente, pois você usará isso na próxima etapa. 
  
Como alternativa, se você não deseja usar o **Exchange 2013: obter configurações do usuário com** o exemplo de descoberta automática, você pode obter a configuração de usuário do **AutoDiscoverSMTPAddress** [gerando uma lista de pontos de extremidade de descoberta automática](how-to-generate-a-list-of-autodiscover-endpoints.md)e, em seguida, enviando a seguinte solicitação de descoberta automática do Pox para cada URL até receber uma resposta bem-sucedida.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

Para obter mais informações sobre o processo de descoberta automática, consulte [descoberta automática do Exchange](autodiscover-for-exchange.md), [gerar uma lista de pontos de extremidade de descoberta automática](how-to-generate-a-list-of-autodiscover-endpoints.md)e [obter as configurações de usuário do Exchange usando a descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a>Definir os valores dos cabeçalhos X-AnchorMailbox e X-PublicFolderMailbox
<a name="bk_setheadervalues"> </a>

Usando o valor do **AutoDiscoverSMTPAddress** adquirido em [fazer uma solicitação de descoberta automática](#bk_makeautodrequest), defina os valores dos cabeçalhos **x-AnchorMailbox** e **x-PublicFolderMailbox** em sua solicitação de conteúdo de pasta pública. 
  
Por exemplo, dado um AutoDiscoverSMTPAddress de NewPublicFolder@contoso.com, inclua os seguintes cabeçalhos ao fazer chamadas para os seguintes métodos ou operações.
  
`X-AnchorMailbox: NewPublicFolder@contoso.com`<br/>
`X-PublicFolderMailbox: NewPublicFolder@contoso.com`

**Chamadas de pasta pública que exigem os cabeçalhos X-AncorMailbox e X-PublicFolder**

|**Métodos da API gerenciada do EWS**|**Operações do EWS**|
|:-----|:-----|
|[Item. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Item. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [Item. Copy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [Item. move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [Item. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
   
Para adicionar esses cabeçalhos usando a API gerenciada do EWS, use o método [HttpHeaders. Add](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) . 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "NewPublicFolder@contoso.com");
service.HttpHeaders.Add("X-PublicFolderMailbox", "NewPublicFolder@contoso.com");
```

O código a seguir mostra uma solicitação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) com o cabeçalho **x-AnchorMailbox** e **x-PublicFolderMailbox** definidos para os valores recuperados nos exemplos deste artigo. 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
User-Agent: SoapSender1.0
X-AnchorMailbox: NewPublicFolder@contoso.com
X-PublicFolderMailbox: NewPublicFolder@contoso.com
Authorization: Basic c29ueWFmQGNvbnRvc28xMDAwLm9ubWljcm9zb2Z0LmNvbTpFWENIIzIwMTQ=
Host: outlook.office365.com
Content-Length: 688
Expect: 100-continue
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="publicfoldersroot" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também

- [Acesso a pastas públicas com o EWS no Exchange](public-folder-access-with-ews-in-exchange.md)    
- [Descoberta Automática do Exchange](autodiscover-for-exchange.md)    
- [Gerar uma lista de pontos de extremidade de Descoberta Automática](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [Obter as configurações de usuário do Exchange usando a Descoberta Automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
  