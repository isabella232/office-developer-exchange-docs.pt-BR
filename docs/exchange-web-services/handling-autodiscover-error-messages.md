---
title: Manipulação de mensagens de erro de Descoberta Automática
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: e5939ec2-1100-4174-8a88-5a6e09b60b23
description: Saiba mais sobre os diferentes tipos de erros de descoberta automática e o que fazer com eles.
localization_priority: Priority
ms.openlocfilehash: 0cba7e54cb251a9775e0971826560e277dcd9d2d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455958"
---
# <a name="handling-autodiscover-error-messages"></a>Manipulação de mensagens de erro de Descoberta Automática

Saiba mais sobre os diferentes tipos de erros de descoberta automática e o que fazer com eles.
  
A descoberta automática permite que os aplicativos recuperem informações de configuração automaticamente e funcionem muito. No entanto, as coisas nem sempre vão de acordo com o plano. Vamos examinar os erros comuns que podem ocorrer e como você pode tratá-los para minimizar a necessidade de solicitar que o usuário configure manualmente o cliente.
  
## <a name="http-status-errors"></a>Erros de status HTTP
<a name="bk_HttpErrors"> </a>

O primeiro tipo de erro que você pode encontrar ao enviar solicitações de descoberta automática é o status HTTP. Se o status do HTTP na sua resposta for diferente de 200 (OK), a carga de resposta não conterá a resposta de descoberta automática que você estava procurando. Para simplificar, podemos agrupar códigos de status não 200 em três categorias.
  
**Tabela 1. Códigos de status HTTP**

|**Código de status**|**Tipo de erro**|**Para lidar com...**|
|:-----|:-----|:-----|
|301 ou 302  <br/> |Redirecionar erro  <br/> |Reenvie sua solicitação para o URI contido no cabeçalho de resposta HTTP "local". Para obter detalhes, consulte [tratamento de erros de redirecionamento](#bk_HandlingRedirects).  <br/> |
|401  <br/> |Erro não autorizado  <br/> |Como o [processo de descoberta automática](autodiscover-for-exchange.md) envolve a tentativa de várias URLs potenciais, você poderia obtê-la em apenas uma URL para que a próxima aceite suas credenciais. Por esse motivo, você não deve considerar um único erro 401 para indicar que as credenciais são inválidas. No entanto, se você receber erros 401 de várias URLs, talvez queira solicitar que o usuário reinsira a senha (se possível).  <br/> |
|Qualquer outro status diferente de 200  <br/> |Erro de ponto de extremidade de descoberta automática inválido  <br/> |Considere a URL que retorna qualquer outro código de status diferente de 200 para ser inválido e continue tentando a próxima URL em sua lista.  <br/> |
   
## <a name="autodiscover-errors"></a>Erros de descoberta automática
<a name="bk_AutodiscoverErrors"> </a>

Mesmo se você receber um código de status de 200 (OK) após enviar uma solicitação de descoberta automática, isso não significa que o servidor enviou as informações necessárias. O status 200 significa que você tem uma resposta de descoberta automática, e essa resposta pode conter um erro dentro da carga. O local das informações de erro difere dependendo se o formato é SOAP ou POX.
  
### <a name="soap-autodiscover-errors"></a>Erros de descoberta automática de SOAP

Para descoberta automática de SOAP, a resposta pode conter um ou mais elementos de [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) em locais diferentes. Normalmente, você pode esperar um como um elemento filho do elemento [Response (SOAP)](https://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) e um como um filho de cada elemento [userresponse (SOAP)](https://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) na resposta. Você também pode encontrar um como um filho de um elemento [UserSettingError (SOAP)](https://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) , se houver um. O contexto do erro depende de onde o elemento **ErrorCode** está localizado, da seguinte maneira: 
  
- Como um elemento filho do elemento **Response** , o elemento **ErrorCode** representa um erro que se aplica a toda a solicitação. 
    
- Como um filho do elemento **userresponse** , ele representa um erro que se aplica apenas ao usuário específico. 
    
- Como um filho de um elemento **UserSettingError** , ele representa um erro que se aplica a uma configuração específica que foi solicitada. 
    
Vamos dar uma olhada em um exemplo de resposta. Neste exemplo, o elemento **ErrorCode** sob o elemento **Response** tem um valor de "NOERROR", que indica o êxito geral. No entanto, o elemento **ErrorCode** sob o elemento **userresponse** tem um valor de "RedirectAddress", que indica que ocorreu um erro para esse usuário específico. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/" 
    xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>14</h:MajorVersion>
      <h:MinorVersion>3</h:MinorVersion>
      <h:MajorBuildNumber>136</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2010_SP2</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>RedirectAddress</ErrorCode>
            <ErrorMessage>Redirection address.</ErrorMessage>
            <RedirectTarget>elvin@mail.contoso.com</RedirectTarget>
            <UserSettingErrors />
            <UserSettings />
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

O artigo [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) contém uma lista completa de possíveis erros. A maioria delas indica um erro irrecuperável, mas algumas garantias especiais de tratamento. 
  
**Tabela 2. Valores SOAP Autodisover ErrorCode**

|**Valor de ErrorCode**|**Para lidar com...**|
|:-----|:-----|
|RedirectAddress  <br/> |[Reiniciando a descoberta automática com um novo endereço de email](#bk_RestartAutodiscover) com o endereço de email no elemento [RedirectTarget (SOAP)](https://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) .  <br/> |
|RedirectUrl  <br/> |[Reenviar sua solicitação para uma nova URL](#bk_ResendRequest) para a URL no elemento **RedirectTarget** .  <br/> |
|ServerBusy  <br/> |Tente esta URL novamente após um pequeno atraso. Você pode aguardar uma quantidade de tempo definida ou simplesmente mover esta URL para o final da lista de URLs a serem tentadas. Se você receber esse erro várias vezes de uma URL, considere a URL como inválida.  <br/> |
   
### <a name="pox-autodiscover-errors"></a>Erros de descoberta automática do POX

O serviço de descoberta automática do POX relata erros um pouco diferente. Erros não recuperáveis estão contidos no elemento [Error (POX)](https://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) . O artigo [ErrorCode (POX)](https://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) contém uma lista completa de possíveis códigos de erro. 
  
Os erros de redirecionamento estão contidos no elemento [Action (POX)](https://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) . Qualquer valor do elemento **Action** diferente de "Settings" indica um erro de redirecionamento. 
  
**Tabela 3. Valores de Autodisover de código POX**

|**Valor da ação**|**Para lidar com...**|
|:-----|:-----|
|redirectAddr  <br/> |[Reiniciando a descoberta automática com um novo endereço de email](#bk_RestartAutodiscover) com o endereço de email no elemento [RedirectAddr (POX)](https://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) .  <br/> |
|redirectUrl  <br/> |[Reenviar sua solicitação para uma nova URL](#bk_ResendRequest) para a URL no elemento [RedirectUrl (POX)](https://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) .  <br/> |
   
Neste exemplo, o elemento **Action** tem um valor de "redirectAddr", que indica que uma nova solicitação deve ser enviada com o novo endereço de email contido no elemento **redirectAddr** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <Account>
      <Action>redirectAddr</Action>
      <RedirectAddr>elvin@mail.contoso.com</RedirectAddr>
    </Account>
  </Response>
</Autodiscover>
```

## <a name="handling-redirect-errors"></a>Tratamento de erros de redirecionamento
<a name="bk_HandlingRedirects"> </a>

Você pode manipular cenários de erro de redirecionamento de duas maneiras:
  
- Reiniciando a descoberta automática com um novo endereço de email.
    
- Reenviando sua solicitação para uma nova URL.
    
Os dois cenários exigem algumas validações antes de prosseguir.
  
### <a name="restarting-autodiscover-with-a-new-email-address"></a>Reiniciando a descoberta automática com um novo endereço de email
<a name="bk_RestartAutodiscover"> </a>

Ao obter um novo endereço de email em uma resposta de redirecionamento de descoberta automática, primeiro verifique se o novo endereço de email fornecido na resposta de erro de redirecionamento não é o mesmo endereço que você enviou na solicitação que resultou no erro. Se for, você não deve reiniciar a descoberta automática e, em vez disso, considere a URL que gerou a resposta para ser inválida.
  
Se o novo endereço de email for diferente, descarte sua lista existente de possíveis URLs de ponto de extremidade de descoberta automática e gere uma nova lista com base no novo endereço de email.
  
### <a name="resending-your-request-to-a-new-url"></a>Reenviar sua solicitação para uma nova URL
<a name="bk_ResendRequest"> </a>

Ao obter uma nova URL em uma resposta de redirecionamento de descoberta automática, você deve primeiro validar a URL da seguinte maneira:
  
- Verifique se a URL é uma URL HTTPS.
    
- Verifique se você não recebeu um erro desta URL com o endereço de email atual antes.
    
- Se aplicável ao seu aplicativo, informe o usuário sobre o redirecionamento e obtenha suas permissões para seguir o redirecionamento.
    
- Envie uma solicitação para a URL e [Verifique se o certificado SSL apresentado pelo servidor é válido](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).
    
Se a URL passar na validação, reenvie a solicitação para essa nova URL.
  
## <a name="see-also"></a>Confira também


- [Descoberta Automática do Exchange](autodiscover-for-exchange.md)
    
- [Localizar os pontos de extremidade de Descoberta Automática usando pesquisa do SCP no Exchange](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)
    
- [ErrorCode (POX)](https://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)
    

