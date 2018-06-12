---
title: Rotear as solicitações de hierarquia de pasta pública
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ec35df8e-4d75-4aa1-8b9c-ae1db7e05772
description: Todas as solicitações de informações de pasta pública que requerem conhecimento da hierarquia de pasta pública, como mover, atualizar, excluir ou localizar pastas públicas, precisam ser roteado para a caixa de correio de hierarquia de pasta pública de padrão para o usuário determinado. Para rotear as solicitações para essa caixa de correio, você precisará definir os cabeçalhos X-AnchorMailbox e X-PublicFolderMailbox para especificar os valores retornados pelo serviço de descoberta automática.
ms.openlocfilehash: 983431864729edbb040a7206dae416d10bfb2b7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750826"
---
# <a name="route-public-folder-hierarchy-requests"></a>Rotear as solicitações de hierarquia de pasta pública

Todas as solicitações de informações de pasta pública que requerem conhecimento da hierarquia de pasta pública, como mover, atualizar, excluir ou localizar pastas públicas, precisam ser roteado para a caixa de correio de hierarquia de pasta pública de padrão para o usuário determinado. Para rotear as solicitações para essa caixa de correio, você precisará definir os cabeçalhos **X-AnchorMailbox** e **X-PublicFolderMailbox** para especificar os valores retornados pelo serviço de descoberta automática. 
  
**Visão geral de pastas públicas**

|Cabeçalho|O que é necessário?|Como obtê-lo?|
|:-----|:-----|:-----|
|**X-AnchorMailbox** <br/> |O valor de [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx) de uma resposta de descoberta automática SOAP [GetUserSettings](http://msdn.microsoft.com/en-us/library/office/dd877096%28v=exchg.150%29.aspx) , que se torna o valor do cabeçalho **X-AnchorMailbox** .<br/><br/> ![TAREFAS PENDENTES](media/Ex15_PF_PFH_Anchor.png)| 1. envie uma solicitação de **GetUserSetting** com o endereço SMTP da caixa de correio do usuário.<br/><br/>2. o valor do elemento **PublicFolderInformation** que o serviço de descoberta automática retorna o cache. Isso pode ser um cache de uma chamada de descoberta automática existente no seu código, ou uma nova [chamada EWS Managed API GetUserSettings](#bk_getpfinfoewsma) ou uma [solicitação SOAP GetUserSettings](#bk_getpfinfoews).  <br/><br/>3. use o elemento **PublicFolderInformation** para preencher o valor do cabeçalho **X-AnchorMailbox** . O valor do elemento **PublicFolderInformation** é um endereço SMTP.  <br/> |
|**X-PublicFolderMailbox** <br/> |O valor de [servidor](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx) de uma [resposta de descoberta automática de POX](http://msdn.microsoft.com/en-us/library/bb204082%28v=exchg.150%29.aspx), que se torna o valor do cabeçalho **X-PublicFolderMailbox** .<br/><br/> ![TAREFAS PENDENTES](media/Ex15_PF_PFH_PFMailbox.png)|1. o serviço de [call POX descoberta automática](#bk_makeautodrequest) usando o endereço de email **X-AnchorMailbox** .  <br/><br/>2. use o elemento de **servidor** retornado pelo serviço de descoberta automática para preencher o valor do cabeçalho **X-PublicFolderMailbox** . O valor do **X-PublicFolderMailbox** é um endereço SMTP onde o nome de usuário é um GUID.  <br/> |

<br/>

Após ter determinado os valores de cabeçalho, incluí-los [quando você faz solicitações de hierarquia de pasta pública](#bk_setheadervalues).
  
As etapas neste artigo são específicas para solicitações de hierarquia de pasta pública. Para determinar se a sua solicitação é uma hierarquia de pasta pública ou a solicitação de conteúdo, consulte [Roteamento solicitações de pasta pública](public-folder-access-with-ews-in-exchange.md#bk_routing).
  
## <a name="determine-the-value-of-the-x-anchormailbox-header-by-using-the-ews-managed-api"></a>Determinar o valor do cabeçalho X-AnchorMailbox usando a API gerenciada de EWS
<a name="bk_getpfinfoewsma"> </a>

Para recuperar o valor de [PublicFolderInformation (POX)](http://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) usando a API gerenciada de EWS, você pode armazenar em cache o valor do elemento **PublicFolderInformation** retorna uma chamada existente ao serviço de descoberta automática ou fazer uma nova chamada. 
  
Se você estiver fazendo uma nova chamada, você pode [obter configurações de usuário usando a API gerenciada de EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)[obter configurações de usuário usando a API gerenciada de EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed) para seu código e, em seguida, chame o **GetUserSettings** de exemplo do método usando o código a seguir, que recupera somente o valor do elemento **PublicFolderInformation** . Inclua o endereço SMTP do usuário da caixa de correio como um parâmetro de entrada. 
  
```cs
GetUserSettingsResponse userResponse = GetUserSettings(adservice, "sonyaf@contoso.com", 3, UserSettingName.PublicFolderInformation);
Console.WriteLine("X-AnchorMailbox value for public folder hierarchy requests: {0}", userResponse.Settings[UserSettingName.PublicFolderInformation]);
```

Após a execução do código, as informações a seguir serão exibidas no console:
  
`X-AnchorMailbox for public folder hierarchy requests: SharedPublicFolder@contoso.com`

Agora que você tem o valor de **PublicFolderInformation** , incluí-lo como o valor para o cabeçalho X-AnchorMailbox em todas as solicitações de hierarquia de pasta pública. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="determine-the-value-of-the-x-anchormailbox-header-using-soap"></a>Determinar o valor do cabeçalho X-AnchorMailbox usando SOAP
<a name="bk_getpfinfoews"> </a>

O exemplo de código a seguir mostra como recuperar o valor de **PublicFolderInformation** usando a operação de SOAP [GetUserSettings](http://msdn.microsoft.com/en-us/library/dd877096%28v=exchg.150%29.aspx) . O usuário de caixa de correio for especificado no elemento de [caixa de correio](http://msdn.microsoft.com/en-us/library/dd877076%28v=exchg.150%29.aspx) e o elemento [RequestedSettings](http://msdn.microsoft.com/en-us/library/office/dd877107%28v=exchg.150%29.aspx) limita a resposta para o valor de [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2007_SP1</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
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

A resposta inclui o valor de **PublicFolderInformation** . 
  
```XML
<UserSetting i:type="StringSetting">
    <Name>PublicFolderInformation</Name>
    <Value>SharedPublicFolder@contoso.com</Value>
</UserSetting>
```

Agora que você tem o valor de **PublicFolderInformation** , incluí-lo como o valor para o cabeçalho X-AnchorMailbox em todas as solicitações de hierarquia de pasta pública. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="make-an-autodiscover-request-to-determine-the-x-publicfolderinformation-value"></a>Fazer uma solicitação de descoberta automática para determinar o valor X-PublicFolderInformation
<a name="bk_makeautodrequest"> </a>

Fazer uma solicitação de descoberta automática usando o endereço de SMTP **PublicFolderInformation** , que agora está sendo usado como o valor **X-AnchorMailbox** . Use o [Exchange 2013: obter configurações de usuário com a descoberta automática](http://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) amostra de código para chamar o serviço de descoberta automática, porque ele simplifica o processo de descoberta automática para você. Este exemplo de código usa os argumentos de linha de comando listados na tabela a seguir para chamar o serviço de descoberta automática de POX no endereço SMTP **PublicFolderInformation** . 
  
|**Argumento da linha de comando**|**Descrição**|
|:-----|:-----|
|emailAddress  <br/> |O endereço de **PublicFolderInformation** SMTP.  <br/> |
|-skipSOAP  <br/> | Use as solicitações de descoberta automática de POX para este cenário.  <br/> |
|-auth authEmailAddress  <br/> |Endereço de email do usuário da caixa de correio, que é usado para autenticação. Você será solicitado a inserir a senha do usuário da caixa de correio quando você executa o exemplo.  <br/> |
   
Por exemplo, quando SharedPublicFolder@contoso.com é o endereço SMTP do elemento **PublicFolderInformation** e sonyaf@contoso.com é o usuário de caixa de correio, os argumentos de linha de comando devem estar no formato. 
  
`SharedPublicFolder@contoso.com -skipSOAP -auth sonyaf@contoso.com`

Quando você executa o **Exchange 2013: obter configurações de usuário com a descoberta automática** amostra, a última resposta da descoberta automática deve ter êxito e incluir todas as configurações de usuário associadas a GUID de caixa de correio. O valor do [servidor](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx) associado ao elemento de [protocolo](http://msdn.microsoft.com/en-us/library/bb204278%28v=exchg.150%29.aspx)EXCH[tipo](http://msdn.microsoft.com/en-us/library/office/bb204223%28v=exchg.150%29.aspx) é o valor de cabeçalho **X-PublicFolderInformation** . 
  
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

Como alternativa, se você não quiser usar o **Exchange 2013: obter configurações de usuário com a descoberta automática** amostra, você pode obter o valor do **servidor** [gerando uma lista de pontos de extremidade de descoberta automática](how-to-generate-a-list-of-autodiscover-endpoints.md)e, em seguida, enviando a seguir Autodiscover POX solicitação de cada URL até receber uma resposta bem-sucedida. SharedPublicFolder@contoso.com é o valor do cabeçalho **X-PublicFolderMailbox** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>SharedPublicFolder@contoso.com</EMailAddress>
    <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

Para obter mais informações sobre o processo de descoberta automática, consulte [obter configurações de usuário do Exchange usando a descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md), [gerar uma lista de pontos de extremidade de descoberta automática](how-to-generate-a-list-of-autodiscover-endpoints.md)e [descoberta automática do Exchange](autodiscover-for-exchange.md).
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a>Defina os valores dos cabeçalhos X-AnchorMailbox e X-PublicFolderMailbox
<a name="bk_setheadervalues"> </a>

Usando o valor do endereço **PublicFolderInformation** SMTP adquirido em [determinar o valor do cabeçalho X-AnchorMailbox usando a API gerenciada de EWS](#bk_getpfinfoewsma) ou [determinar o valor do cabeçalho X-AnchorMailbox usando SOAP](#bk_getpfinfoews) e o servidor ** **valor adquirido em [tornar uma solicitação de descoberta automática para determinar o valor X-PublicFolderInformation](#bk_makeautodrequest), defina os valores dos cabeçalhos **X-AnchorMailbox** e **X-PublicFolderMailbox** em sua solicitação de conteúdo de pasta pública. 
  
Por exemplo, devido a um endereço de **PublicFolderInformation** SMTP do SharedPublicFolder@contoso.com e o valor de um **servidor** de 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com, inclua os seguintes cabeçalhos ao fazer chamadas para o seguinte métodos ou operações. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com` <br/>
`X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com`

**Chamadas de pasta pública que exigem os cabeçalhos X-AnchorMailbox e X-PublicFolder**

|**Métodos de API gerenciada de EWS**|**Operações de EWS**|
|:-----|:-----|
|[Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Folder.Move](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
Para adicionar esses cabeçalhos usando a API gerenciada de EWS, use o método [HttpHeaders.Add](http://msdn.microsoft.com/en-us/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) . 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "SharedPublicFolder@contoso.com");service.HttpHeaders.Add("X-PublicFolderMailbox", "1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com");
```

Por exemplo, o código a seguir mostra uma solicitação [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) com o cabeçalho **X-AnchorMailbox** e **X-PublicFolderMailbox** definido para os valores recuperados nos exemplos neste artigo. 
  
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

- [Acessar pastas públicas com EWS no Exchange](public-folder-access-with-ews-in-exchange.md)    
- [Rotear as solicitações de conteúdo de pasta pública](how-to-route-public-folder-content-requests.md)    
- [Obter configurações de usuário usando a API gerenciada de EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)
    

