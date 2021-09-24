---
title: Rotear as solicitações de hierarquia da pasta pública
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: ec35df8e-4d75-4aa1-8b9c-ae1db7e05772
description: Todas as solicitações de informações de pasta pública que exigem conhecimento da hierarquia de pastas públicas, como mover, atualizar, excluir ou localizar pastas públicas, precisam ser roteados para a caixa de correio padrão da hierarquia de pastas públicas para o usuário específico. Para rotear as solicitações para essa caixa de correio, você precisa definir os headers X-AnchorMailbox e X-PublicFolderMailbox para valores específicos retornados pelo serviço de Descoberta Automática.
ms.openlocfilehash: e86e1956db33b7ad8e654a22b980900b4f59dd87
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513119"
---
# <a name="route-public-folder-hierarchy-requests"></a>Rotear as solicitações de hierarquia da pasta pública

Todas as solicitações de informações de pasta pública que exigem conhecimento da hierarquia de pastas públicas, como mover, atualizar, excluir ou localizar pastas públicas, precisam ser roteados para a caixa de correio padrão da hierarquia de pastas públicas para o usuário específico. Para rotear as solicitações para essa caixa de correio, você precisa definir os headers **X-AnchorMailbox** e **X-PublicFolderMailbox** para valores específicos retornados pelo serviço de Descoberta Automática. 
  
**Visão geral das pastas públicas**

|Cabeçalho|Do que preciso?|Como faço para obter isso?|
|:-----|:-----|:-----|
|**X-AnchorMailbox** <br/> |O [valor PublicFolderInformation](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) de uma resposta SOAP de Descoberta Automática [GetUserSettings,](https://msdn.microsoft.com/library/office/dd877096%28v=exchg.150%29.aspx) que se torna o valor do header **X-AnchorMailbox.**<br/><br/> ![Resposta X-AnchorMailbox](media/Ex15_PF_PFH_Anchor.png)| 1. Envie uma **solicitação GetUserSetting** com o endereço SMTP para a caixa de correio do usuário.<br/><br/>2. Armazenar em cache o valor **do elemento PublicFolderInformation** que o serviço de Descoberta Automática retorna. Pode ser um cache de uma chamada de Descoberta Automática existente em seu código ou uma nova chamada [getUserSettings](#bk_getpfinfoewsma) da API gerenciada do EWS ou uma solicitação [SOAP getUserSettings](#bk_getpfinfoews).  <br/><br/>3. Use o **elemento PublicFolderInformation** para preencher o valor do header **X-AnchorMailbox.** O valor do **elemento PublicFolderInformation** é um endereço SMTP.  <br/> |
|**X-PublicFolderMailbox** <br/> |O [valor server](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) de uma resposta de Descoberta Automática [POX](https://msdn.microsoft.com/library/bb204082%28v=exchg.150%29.aspx), que se torna o valor do header **X-PublicFolderMailbox.**<br/><br/> ![Resposta X-PublicFolderMailbox](media/Ex15_PF_PFH_PFMailbox.png)|1. [Chame o serviço de Descoberta Automática POX](#bk_makeautodrequest) usando o endereço de email **X-AnchorMailbox.**  <br/><br/>2. Use o **elemento Server** retornado pelo serviço descoberta automática para preencher o valor do header **X-PublicFolderMailbox.** O valor da **X-PublicFolderMailbox** é um endereço SMTP em que o nome de usuário é um GUID.  <br/> |

<br/>

Depois de determinar os valores de header, inclua-os ao fazer solicitações de hierarquia de pastas [públicas.](#bk_setheadervalues)
  
As etapas deste artigo são específicas para solicitações de hierarquia de pastas públicas. Para determinar se sua solicitação é uma hierarquia de pastas públicas ou uma solicitação de conteúdo, consulte [Roteamento de solicitações de pasta pública](public-folder-access-with-ews-in-exchange.md#bk_routing).
  
## <a name="determine-the-value-of-the-x-anchormailbox-header-by-using-the-ews-managed-api"></a>Determinar o valor do header X-AnchorMailbox usando a API Gerenciada do EWS
<a name="bk_getpfinfoewsma"> </a>

Para recuperar o [valor PublicFolderInformation (POX)](https://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) usando a API Gerenciada do EWS, você pode armazenar em cache o valor do **elemento PublicFolderInformation** que uma chamada existente para o serviço de Descoberta Automática retorna ou fazer uma nova chamada. 
  
Se você estiver fazendo uma nova chamada, poderá Obter configurações do usuário usando a API Gerenciada do [EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)Obter configurações de usuário usando a API Gerenciada do [EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed) para seu código e, em seguida, chamar o método de exemplo **GetUserSettings** usando o código a seguir, que recupera apenas o valor do **elemento PublicFolderInformation.** Inclua o endereço SMTP do usuário da caixa de correio como um parâmetro de entrada. 
  
```cs
GetUserSettingsResponse userResponse = GetUserSettings(adservice, "sonyaf@contoso.com", 3, UserSettingName.PublicFolderInformation);
Console.WriteLine("X-AnchorMailbox value for public folder hierarchy requests: {0}", userResponse.Settings[UserSettingName.PublicFolderInformation]);
```

Após a execução do código, as seguintes informações são exibidas no console:
  
`X-AnchorMailbox for public folder hierarchy requests: SharedPublicFolder@contoso.com`

Agora que você tem o **valor PublicFolderInformation,** inclua-o como o valor do header X-AnchorMailbox em todas as solicitações de hierarquia de pastas públicas. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="determine-the-value-of-the-x-anchormailbox-header-using-soap"></a>Determinar o valor do header X-AnchorMailbox usando SOAP
<a name="bk_getpfinfoews"> </a>

O exemplo de código a seguir mostra como recuperar o **valor PublicFolderInformation** usando a [operação GETUserSettings](https://msdn.microsoft.com/library/dd877096%28v=exchg.150%29.aspx) SOAP. O usuário da caixa de correio é especificado no elemento [Mailbox](https://msdn.microsoft.com/library/dd877076%28v=exchg.150%29.aspx) e o [elemento RequestedSettings](https://msdn.microsoft.com/library/office/dd877107%28v=exchg.150%29.aspx) limita a resposta ao [valor PublicFolderInformation.](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2007_SP1</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://pod51042.outlook.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>sonyaf@contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>PublicFolderInformation</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>
```

A resposta inclui o **valor PublicFolderInformation.** 
  
```XML
<UserSetting i:type="StringSetting">
    <Name>PublicFolderInformation</Name>
    <Value>SharedPublicFolder@contoso.com</Value>
</UserSetting>
```

Agora que você tem o **valor PublicFolderInformation,** inclua-o como o valor do header X-AnchorMailbox em todas as solicitações de hierarquia de pastas públicas. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="make-an-autodiscover-request-to-determine-the-x-publicfolderinformation-value"></a>Fazer uma solicitação de Descoberta Automática para determinar o valor X-PublicFolderInformation
<a name="bk_makeautodrequest"> </a>

Faça uma solicitação de Descoberta Automática usando o endereço SMTP **PublicFolderInformation,** que agora está sendo usado como o **valor X-AnchorMailbox.** Use o [Exchange 2013:](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) Obter configurações do usuário com exemplo de código de Descoberta Automática para chamar o serviço de Descoberta Automática porque simplifica o processo de Descoberta Automática para você. Este exemplo de código usa os argumentos de linha de comando listados na tabela a seguir para chamar o serviço de Descoberta Automática POX no endereço SMTP **PublicFolderInformation.** 
  
|**Argumento de linha de comando**|**Descrição**|
|:-----|:-----|
|emailAddress  <br/> |O **endereço SMTP PublicFolderInformation.**  <br/> |
|-skipSOAP  <br/> | Use solicitações de Descoberta Automática POX para este cenário.  <br/> |
|-auth AuthEmailAddress  <br/> |O endereço de email do usuário da caixa de correio, que é usado para autenticação. Você será solicitado a inserir a senha do usuário da caixa de correio ao executar o exemplo.  <br/> |
   
Por exemplo, quando SharedPublicFolder@contoso.com é o endereço SMTP do **elemento PublicFolderInformation** e sonyaf@contoso.com é o usuário da caixa de correio, os argumentos de linha de comando devem ter esta aparência. 
  
`SharedPublicFolder@contoso.com -skipSOAP -auth sonyaf@contoso.com`

Quando você executar o **Exchange 2013:** Obter configurações do usuário com exemplo de Descoberta Automática, a última resposta de Descoberta Automática deve ser bem-sucedida e incluir todas as configurações de usuário associadas ao GUID da caixa de correio. O [valor](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) server associado ao elemento Tipo de [Protocolo](https://msdn.microsoft.com/library/bb204278%28v=exchg.150%29.aspx)[](https://msdn.microsoft.com/library/office/bb204223%28v=exchg.150%29.aspx) EXCH é o valor de header **X-PublicFolderInformation.** 
  
```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    …
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <Protocol>
        <Type>EXCH</Type>
        <Server>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</Server>

```

Como alternativa, se você não quiser usar o **Exchange 2013:** Obter configurações do usuário  com exemplo de Descoberta Automática, você pode obter o valor server gerando uma lista de pontos de extremidade de Descoberta Automática [e](how-to-generate-a-list-of-autodiscover-endpoints.md)enviando a seguinte solicitação de Descoberta Automática POX para cada URL até receber uma resposta bem-sucedida. SharedPublicFolder@contoso.com é o valor do **header X-PublicFolderMailbox.** 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>SharedPublicFolder@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

Para obter mais informações sobre o processo de Descoberta Automática, consulte Descoberta Automática para [Exchange,](autodiscover-for-exchange.md) [Gerar](how-to-generate-a-list-of-autodiscover-endpoints.md)uma lista de pontos de extremidade de Descoberta Automática e Obter configurações do usuário Exchange usando a [Descoberta](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)Automática .
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a>Definir os valores dos headers X-AnchorMailbox e X-PublicFolderMailbox
<a name="bk_setheadervalues"> </a>

Usando o valor do endereço SMTP **PublicFolderInformation** adquirido em Determine o valor do [header X-AnchorMailbox](#bk_getpfinfoewsma) usando a API Gerenciada do EWS ou Determine o valor do [header X-AnchorMailbox](#bk_getpfinfoews) usando SOAP e o valor de Servidor adquirido em Fazer uma solicitação de Descoberta Automática para determinar o [valor X-PublicFolderInformation](#bk_makeautodrequest), de definir os valores dos headers **X-AnchorMailbox** e  **X-PublicFolderMailbox** em sua solicitação de conteúdo de pasta pública. 
  
Por exemplo, dado um endereço **SMTP PublicFolderInformation** de SharedPublicFolder@contoso.com e um valor server de 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com, inclua os seguintes headers ao fazer chamadas para os métodos ou operações **a** seguir. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com` <br/>
`X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com`

**Chamadas de pasta pública que exigem os headers X-AnchorMailbox e X-PublicFolder**

|**Métodos da API Gerenciada do EWS**|**Operações do EWS**|
|:-----|:-----|
|[Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Folder.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Folder.Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
Para adicionar esses cabeçalhos usando a API Gerenciada do EWS, use o [método HttpHeaders.Add.](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "SharedPublicFolder@contoso.com");service.HttpHeaders.Add("X-PublicFolderMailbox", "1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com");
```

Por exemplo, o código a seguir mostra uma solicitação [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) com o **header X-AnchorMailbox** e **X-PublicFolderMailbox** definido para os valores recuperados nos exemplos deste artigo. 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
User-Agent: SoapSender1.0
X-AnchorMailbox: SharedPublicFolder@contoso.com
X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com
Host: outlook.office365.com
Content-Length: 1174
Expect: 100-continue
Connection: Keep-Alive
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:IsEqualTo>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:FieldURIOrConstant>
            <t:Constant Value="My Public Contacts" />
          </t:FieldURIOrConstant>
        </t:IsEqualTo>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:FolderId Id="AQEuAAADy/LIWjRCp0GFb0W6aGPbwwEARg5aCLUc8k6wLfl1c0a/2AAAAwIAAAA=" ChangeKey="AQAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/XB" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também

- [Acesso a pastas públicas com EWS em Exchange](public-folder-access-with-ews-in-exchange.md)    
- [Rotear as solicitações de conteúdo de pasta pública](how-to-route-public-folder-content-requests.md)    
- [Obter configurações do usuário usando a API Gerenciada do EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)
    

