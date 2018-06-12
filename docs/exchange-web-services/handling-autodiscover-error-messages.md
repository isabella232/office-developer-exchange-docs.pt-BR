---
title: Manipulação de mensagens de erro de descoberta automática
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: e5939ec2-1100-4174-8a88-5a6e09b60b23
description: Saiba mais sobre os diferentes tipos de erros de descoberta automática e o que fazer com eles.
ms.openlocfilehash: fcafc799f4d35e92159d2913845474ecf7bc5657
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750666"
---
# <a name="handling-autodiscover-error-messages"></a>Manipulação de mensagens de erro de descoberta automática

Saiba mais sobre os diferentes tipos de erros de descoberta automática e o que fazer com eles.
  
Descoberta automática permite que seus aplicativos recuperar informações de configuração automaticamente, e ele funciona bem. No entanto, nem sempre tudo de acordo com o plano. Vejamos os erros comuns que podem ocorrer e como você pode tratá-los para minimizar a necessidade de avisar o usuário configurar manualmente o cliente.
  
## <a name="http-status-errors"></a>Erros de status HTTP
<a name="bk_HttpErrors"> </a>

O primeiro tipo de erro que você pode encontrar ao enviar solicitações de descoberta automática é o status HTTP. Se o status HTTP em sua resposta for algo diferente de 200 (Okey), a carga de resposta não contém a resposta da descoberta automática que estava procurando. Para manter a simplicidade, podemos pode agrupar os códigos de status de não-200 em três categorias.
  
**Tabela 1. Códigos de status HTTP**

|**Código de status**|**Tipo de erro**|**Lidar com …**|
|:-----|:-----|:-----|
|301 ou 302  <br/> |Erro de redirecionamento  <br/> |Reenvie sua solicitação para o URI contido no cabeçalho da resposta "Local" HTTP. Para obter detalhes, consulte [redirecionar de tratamento de erros](#bk_HandlingRedirects).  <br/> |
|401  <br/> |Erro não autorizado  <br/> |Porque o [processo de descoberta automática](autodiscover-for-exchange.md) envolve a tentativa de várias URLs possíveis, você poderia obter isso em um URL apenas para ter uma próxima aceitar suas credenciais. Por esse motivo, você não deve considerar um erro 401 único para indicar que as credenciais são inválidas. No entanto, se você receber 401 erros de várias URLs, você deseja solicitar ao usuário a redigitar sua senha (se possível).  <br/> |
|Qualquer outro status de não-200  <br/> |Erro de ponto de extremidade inválido do descoberta automática  <br/> |Considere a URL que retorna qualquer outro código de status de não-200 para ser inválido e continuar a tentar a próxima URL na sua lista.  <br/> |
   
## <a name="autodiscover-errors"></a>Erros de descoberta automática
<a name="bk_AutodiscoverErrors"> </a>

Mesmo se você receber um código de status 200 (Okey) após o envio de uma solicitação de descoberta automática, isso não significa que o servidor enviadas as informações que necessárias. O status de 200 significa apenas que você tenha uma resposta de descoberta automática e essa resposta pode conter um erro dentro da carga. O local das informações de erro será diferente, dependendo se o formato é SOAP ou POX.
  
### <a name="soap-autodiscover-errors"></a>Erros de descoberta automática do SOAP

Para descoberta automática de SOAP, a resposta pode conter um ou mais elementos [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) , em diferentes locais. Normalmente, você pode esperar um como um elemento filho do elemento de [Resposta (SOAP)](http://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) e outro como um filho do elemento cada [Resposta SOAP ()](http://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) na resposta. Você também pode encontrar um como um filho do elemento [UserSettingError (SOAP)](http://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) , caso haja algum. O contexto do erro depende de onde o elemento **ErrorCode** está localizado, da seguinte maneira: 
  
- Como um elemento filho do elemento de **resposta** , o elemento **ErrorCode** representa um erro que se aplica a toda a solicitação. 
    
- Como um filho do elemento de **resposta** , ela representa um erro dizendo que se aplica apenas ao usuário específico. 
    
- Como um filho de um elemento **UserSettingError** , ela representa um erro que se aplica a uma configuração específica que foi solicitada. 
    
Vamos dar uma olhada em um exemplo de uma resposta. Neste exemplo, o elemento **ErrorCode** sob o elemento de **resposta** tem o valor "NoError", que indica o sucesso geral. No entanto, o elemento **ErrorCode** sob o elemento de **resposta** tem um valor igual a "RedirectAddress", que indica que ocorreu um erro para esse usuário. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
    xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>14</h:MajorVersion>
      <h:MinorVersion>3</h:MinorVersion>
      <h:MajorBuildNumber>136</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2010_SP2</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
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

O artigo [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) contém uma lista completa dos erros possíveis. A maioria delas indica um erro irreparável, mas alguns garantem manipulação especial. 
  
**Tabela 2. Valores de Autodisover ErrorCode SOAP**

|**Valor ErrorCode**|**Lidar com …**|
|:-----|:-----|
|RedirectAddress  <br/> |[Reiniciando Autodiscover com um novo endereço de email](#bk_RestartAutodiscover) com o endereço de email no elemento [RedirectTarget (SOAP)](http://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) .  <br/> |
|RedirectUrl  <br/> |[Reenvio sua solicitação para uma nova URL](#bk_ResendRequest) para a URL no elemento **RedirectTarget** .  <br/> |
|ServerBusy  <br/> |Repita essa URL após um pequeno atraso. Você pode esperar um determinado período de tempo ou simplesmente se mudar essa URL ao final da sua lista de URLs para tentar. Se você receber esse erro várias vezes, a partir de uma URL, você deve considerar a URL seja inválido.  <br/> |
   
### <a name="pox-autodiscover-errors"></a>Erros de descoberta automática POX

O serviço Descoberta automática de POX relata os erros de um pouco diferente. Erros não recuperável estão contidos no elemento [Erro POX ()](http://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) . O artigo [ErrorCode POX ()](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) contém uma lista completa dos códigos de erro possíveis. 
  
Erros de redirecionamento estão contidos no elemento [Action POX ()](http://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) . Qualquer valor do elemento **Action** diferente de "configurações" indica um erro de redirecionamento. 
  
**Tabela 3. Valores de Autodisover ErrorCode POX**

|**Valor de ação**|**Lidar com …**|
|:-----|:-----|
|redirectAddr  <br/> |[Reiniciando Autodiscover com um novo endereço de email](#bk_RestartAutodiscover) com o endereço de email no elemento [RedirectAddr POX ()](http://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) .  <br/> |
|redirectUrl  <br/> |[Reenvio sua solicitação para uma nova URL](#bk_ResendRequest) para a URL no elemento [RedirectUrl POX ()](http://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) .  <br/> |
   
Neste exemplo, o elemento **Action** tem um valor igual a "redirectAddr", que indica que uma nova solicitação deve ser enviada com o novo endereço de email contido no elemento **RedirectAddr** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <Account>
      <Action>redirectAddr</Action>
      <RedirectAddr>elvin@mail.contoso.com</RedirectAddr>
    </Account>
  </Response>
</Autodiscover>
```

## <a name="handling-redirect-errors"></a>Tratamento de erros de redirecionamento
<a name="bk_HandlingRedirects"> </a>

Você pode manipular os cenários de erro de redirecionamento de duas maneiras:
  
- Reiniciando descoberta automática com um novo endereço de email.
    
- Por reenvio sua solicitação para uma nova URL.
    
Ambos os cenários exigem alguma validação antes de continuar.
  
### <a name="restarting-autodiscover-with-a-new-email-address"></a>Reiniciando descoberta automática com um novo endereço de email
<a name="bk_RestartAutodiscover"> </a>

Quando você obtém um novo endereço de email em uma descoberta automática para redirecionar a resposta, primeiro verifique se o novo endereço de email que foi fornecido na resposta de erro do redirecionamento não é o mesmo endereço que você enviados na solicitação que causou o erro. Se for, não deve reiniciar a descoberta automática e em vez disso, considere a URL que gerou a resposta para ser inválido.
  
Se o novo endereço de email for diferente, descartar sua lista de possíveis URLs de ponto de extremidade de descoberta automática existentes e gerar uma nova lista com base no novo endereço de email.
  
### <a name="resending-your-request-to-a-new-url"></a>Reenvio sua solicitação para uma nova URL
<a name="bk_ResendRequest"> </a>

Quando você receber uma nova URL em uma resposta de redirecionamento de descoberta automática, você deve primeiro validar a URL da seguinte maneira:
  
- Verifique se a URL é uma URL HTTPS.
    
- Verifique se que você não tiver recebido um erro dessa URL com o endereço de email atual antes.
    
- Se aplicável ao seu aplicativo, informar ao usuário sobre o redirecionamento e obtenha sua permissão para seguir o redirecionamento.
    
- Envie uma solicitação para a URL e [Verifique se o certificado SSL apresentado pelo servidor é válido](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).
    
Se a URL passa a validação, reenvie a solicitação para esta nova URL.
  
## <a name="see-also"></a>Confira também


- [Descoberta Automática do Exchange](autodiscover-for-exchange.md)
    
- [Encontrar os pontos de extremidade de descoberta automática usando pesquisa do SCP no Exchange](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)
    
- [ErrorCode POX)](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)
    

