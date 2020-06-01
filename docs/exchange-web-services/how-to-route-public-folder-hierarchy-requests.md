---
title: Rotear solicitações de hierarquia de pasta pública
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ec35df8e-4d75-4aa1-8b9c-ae1db7e05772
description: Todas as solicitações de informações de pasta pública que exigem o conhecimento da hierarquia de pastas públicas, como mover, atualizar, excluir ou localizar pastas públicas, precisam ser encaminhadas para a caixa de correio de hierarquia de pasta pública padrão para o usuário específico. Para encaminhar as solicitações para essa caixa de correio, você precisa definir os cabeçalhos X-AnchorMailbox e X-PublicFolderMailbox como valores específicos retornados pelo serviço de descoberta automática.
ms.openlocfilehash: 2773aa3ab29868c69d1fb088deb6c8a96dfb9ecc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455687"
---
# <a name="route-public-folder-hierarchy-requests"></a>Rotear solicitações de hierarquia de pasta pública

Todas as solicitações de informações de pasta pública que exigem o conhecimento da hierarquia de pastas públicas, como mover, atualizar, excluir ou localizar pastas públicas, precisam ser encaminhadas para a caixa de correio de hierarquia de pasta pública padrão para o usuário específico. Para encaminhar as solicitações para essa caixa de correio, você precisa definir os cabeçalhos **x-AnchorMailbox** e **x-PublicFolderMailbox** como valores específicos retornados pelo serviço de descoberta automática. 
  
**Visão geral das pastas públicas**

|Cabeçalho|O que eu preciso?|Como posso obtê-lo?|
|:-----|:-----|:-----|
|**X-AnchorMailbox** <br/> |O valor [PublicFolderInformation](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) de uma resposta SOAP de descoberta automática do [GetUserSettings](https://msdn.microsoft.com/library/office/dd877096%28v=exchg.150%29.aspx) , que se torna o valor do cabeçalho **X-AnchorMailbox** .<br/><br/> ![FAZER](media/Ex15_PF_PFH_Anchor.png)| 1. envie uma solicitação de **GetUserSetting** com o endereço SMTP da caixa de correio do usuário.<br/><br/>2. Armazene em cache o valor do elemento **PublicFolderInformation** que o serviço de descoberta automática retorna. Isso pode ser um cache de uma chamada de descoberta automática existente em seu código ou uma nova [chamada de API gerenciada do EWS GetUserSettings](#bk_getpfinfoewsma) ou uma [solicitação SOAP GetUserSettings](#bk_getpfinfoews).  <br/><br/>3. Use o elemento **PublicFolderInformation** para preencher o valor do cabeçalho **X-AnchorMailbox** . O valor do elemento **PublicFolderInformation** é um endereço SMTP.  <br/> |
|**X-PublicFolderMailbox** <br/> |O valor do [servidor](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) de uma [resposta de descoberta automática de Pox](https://msdn.microsoft.com/library/bb204082%28v=exchg.150%29.aspx), que se torna o valor do cabeçalho **X-PublicFolderMailbox** .<br/><br/> ![FAZER](media/Ex15_PF_PFH_PFMailbox.png)|1. [chame o serviço de descoberta automática do Pox](#bk_makeautodrequest) usando o endereço de email **X-AnchorMailbox** .  <br/><br/>2. Use o elemento **Server** retornado pelo serviço de descoberta automática para preencher o valor do cabeçalho **X-PublicFolderMailbox** . O valor do **X-PublicFolderMailbox** é um endereço SMTP em que o nome de usuário é um GUID.  <br/> |

<br/>

Depois de determinar os valores de cabeçalho, inclua-os [quando fizer solicitações de hierarquia de pastas públicas](#bk_setheadervalues).
  
As etapas neste artigo são específicas para solicitações de hierarquia de pastas públicas. Para determinar se sua solicitação é uma hierarquia de pasta pública ou uma solicitação de conteúdo, consulte [Routing Public Folder](public-folder-access-with-ews-in-exchange.md#bk_routing)requests.
  
## <a name="determine-the-value-of-the-x-anchormailbox-header-by-using-the-ews-managed-api"></a>Determinar o valor do cabeçalho X-AnchorMailbox usando a API gerenciada do EWS
<a name="bk_getpfinfoewsma"> </a>

Para recuperar o valor de [PublicFolderInformation (POX)](https://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) usando a API gerenciada do EWS, você pode armazenar em cache o valor do elemento **PublicFolderInformation** que uma chamada existente para o serviço de descoberta automática retorna ou fazer uma nova chamada. 
  
Se você estiver fazendo uma nova chamada, poderá [obter as configurações do usuário usando a API gerenciada do EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)[para obter as configurações do usuário usando a API gerenciada do EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed) para o seu código e, em seguida, chamar o método de exemplo **GetUserSettings** usando o código a seguir, que recupera apenas o valor do elemento **PublicFolderInformation** . Inclua o endereço SMTP do usuário da caixa de correio como um parâmetro de entrada. 
  
```cs
GetUserSettingsResponse userResponse = GetUserSettings(adservice, "sonyaf@contoso.com", 3, UserSettingName.PublicFolderInformation);
Console.WriteLine("X-AnchorMailbox value for public folder hierarchy requests: {0}", userResponse.Settings[UserSettingName.PublicFolderInformation]);
```

Depois de executar o código, as seguintes informações são exibidas no console:
  
`X-AnchorMailbox for public folder hierarchy requests: SharedPublicFolder@contoso.com`

Agora que você tem o valor **PublicFolderInformation** , inclua-o como o valor para o cabeçalho X-AnchorMailbox em todas as solicitações de hierarquia de pasta pública. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="determine-the-value-of-the-x-anchormailbox-header-using-soap"></a>Determinar o valor do cabeçalho X-AnchorMailbox usando SOAP
<a name="bk_getpfinfoews"> </a>

O exemplo de código a seguir mostra como recuperar o valor **PublicFolderInformation** usando a operação SOAP [GetUserSettings](https://msdn.microsoft.com/library/dd877096%28v=exchg.150%29.aspx) . O usuário da caixa de correio é especificado no elemento [Mailbox](https://msdn.microsoft.com/library/dd877076%28v=exchg.150%29.aspx) e o elemento [RequestedSettings](https://msdn.microsoft.com/library/office/dd877107%28v=exchg.150%29.aspx) limita a resposta para o valor [PublicFolderInformation](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2007_SP1</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://pod51042.outlook.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

A resposta inclui o valor **PublicFolderInformation** . 
  
```XML
<UserSetting i:type="StringSetting">
    <Name>PublicFolderInformation</Name>
    <Value>SharedPublicFolder@contoso.com</Value>
</UserSetting>
```

Agora que você tem o valor **PublicFolderInformation** , inclua-o como o valor para o cabeçalho X-AnchorMailbox em todas as solicitações de hierarquia de pasta pública. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="make-an-autodiscover-request-to-determine-the-x-publicfolderinformation-value"></a>Fazer uma solicitação de descoberta automática para determinar o valor X-PublicFolderInformation
<a name="bk_makeautodrequest"> </a>

Faça uma solicitação de descoberta automática usando o endereço SMTP **PublicFolderInformation** , que agora está sendo usado como o valor **X-AnchorMailbox** . Use o [Exchange 2013: obter as configurações do usuário com](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) o exemplo de código de descoberta automática para chamar o serviço de descoberta automática, pois ele simplifica o processo de descoberta automática. Este exemplo de código usa os argumentos de linha de comando listados na tabela a seguir para chamar o serviço de descoberta automática do POX no endereço SMTP do **PublicFolderInformation** . 
  
|**Argumento de linha de comando**|**Descrição**|
|:-----|:-----|
|emailAddress  <br/> |O endereço SMTP **PublicFolderInformation** .  <br/> |
|-skipSOAP  <br/> | Use as solicitações de descoberta automática do POX para este cenário.  <br/> |
|-auth authEmailAddress  <br/> |O endereço de email do usuário da caixa de correio, que é usado para autenticação. Você será solicitado a inserir a senha do usuário da caixa de correio quando executar o exemplo.  <br/> |
   
Por exemplo, quando SharedPublicFolder@contoso.com é o endereço SMTP do elemento **PublicFolderInformation** , e sonyaf@contoso.com é o usuário da caixa de correio, os argumentos de linha de comando devem ter a seguinte aparência. 
  
`SharedPublicFolder@contoso.com -skipSOAP -auth sonyaf@contoso.com`

Quando você executa o **Exchange 2013: obter as configurações de usuário com** o exemplo de descoberta automática, a última resposta de descoberta automática deve ser bem-sucedida e incluir todas as configurações de usuário associadas ao GUID da caixa de correio. O valor do [servidor](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) associado ao elemento do[tipo](https://msdn.microsoft.com/library/office/bb204223%28v=exchg.150%29.aspx) de [protocolo](https://msdn.microsoft.com/library/bb204278%28v=exchg.150%29.aspx)Exch é o valor do cabeçalho **X-PublicFolderInformation** . 
  
```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    …
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <Protocol>
        <Type>EXCH</Type>
        <Server>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</Server>

```

Como alternativa, se você não deseja usar o **Exchange 2013: obter as configurações do usuário com** o exemplo de descoberta automática, você pode obter o valor do **servidor** [gerando uma lista de pontos de extremidade de descoberta automática](how-to-generate-a-list-of-autodiscover-endpoints.md)e, em seguida, enviando a seguinte solicitação de descoberta automática Pox para cada URL até receber uma resposta bem-sucedida. SharedPublicFolder@contoso.com é o valor do cabeçalho **X-PublicFolderMailbox** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>SharedPublicFolder@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

Para obter mais informações sobre o processo de descoberta automática, consulte [descoberta automática do Exchange](autodiscover-for-exchange.md), [gerar uma lista de pontos de extremidade de descoberta automática](how-to-generate-a-list-of-autodiscover-endpoints.md)e [obter as configurações de usuário do Exchange usando a descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a>Definir os valores dos cabeçalhos X-AnchorMailbox e X-PublicFolderMailbox
<a name="bk_setheadervalues"> </a>

Usando o valor do endereço SMTP **PublicFolderInformation** adquirido em [determine o valor do cabeçalho x-ANCHORMAILBOX usando a API gerenciada do EWS](#bk_getpfinfoewsma) ou [determine o valor do cabeçalho x-AnchorMailbox usando SOAP](#bk_getpfinfoews) e o valor do **servidor** adquirido em [fazer uma solicitação de descoberta automática para determinar o valor x-PublicFolderInformation](#bk_makeautodrequest), defina os valores dos cabeçalhos **x-AnchorMailbox** e **X-PublicFolderMailbox** em sua solicitação de conteúdo de pasta pública. 
  
Por exemplo, dado um endereço SMTP **PublicFolderInformation** de SharedPublicFolder@contoso.com e um valor de **servidor** de 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com, inclua os seguintes cabeçalhos ao fazer chamadas para os seguintes métodos ou operações. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com` <br/>
`X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com`

**Chamadas de pasta pública que exigem os cabeçalhos X-AnchorMailbox e X-PublicFolder**

|**Métodos da API gerenciada do EWS**|**Operações do EWS**|
|:-----|:-----|
|[Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Pasta. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Pasta. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Folder. move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
Para adicionar esses cabeçalhos usando a API gerenciada do EWS, use o método [HttpHeaders. Add](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) . 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "SharedPublicFolder@contoso.com");service.HttpHeaders.Add("X-PublicFolderMailbox", "1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com");
```

Por exemplo, o código a seguir mostra uma solicitação [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) com o cabeçalho **x-AnchorMailbox** e **x-PublicFolderMailbox** definido como os valores recuperados nos exemplos deste artigo. 
  
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
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

## <a name="see-also"></a>Também consulte

- [Acesso a pastas públicas com o EWS no Exchange](public-folder-access-with-ews-in-exchange.md)    
- [Rotear solicitações de conteúdo de pasta pública](how-to-route-public-folder-content-requests.md)    
- [Obter configurações de usuário usando a API gerenciada do EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)
    

