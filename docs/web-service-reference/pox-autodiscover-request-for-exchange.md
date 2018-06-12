---
title: Solicitação de descoberta automática POX para Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: A solicitação de descoberta automática contém uma consulta para a configuração de acesso de cliente do usuário.
ms.openlocfilehash: 48d6c30946e75936ed93a6f4507d8a8d3ae47d40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824865"
---
# <a name="pox-autodiscover-request-for-exchange"></a>Solicitação de descoberta automática POX para Exchange

A solicitação de descoberta automática contém uma consulta para a configuração de acesso de cliente do usuário.
  
## <a name="autodiscover-request-example"></a>Exemplo de solicitação de descoberta automática

### <a name="description"></a>Descrição

O exemplo XML a seguir mostra o corpo de uma solicitação de descoberta automática.
  
### <a name="code"></a>Código

```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a>Cabeçalhos de solicitação

Os seguintes cabeçalhos HTTP são opcionais ao enviar solicitações de descoberta automática.
  
**Tabela 1. Cabeçalhos de solicitação HTTP**

|**Header**|**Descrição**|
|:-----|:-----|
|X-MapiHttpCapability  <br/> |Se presente e definida como "1", indica que o cliente está solicitando informações que podem ser usadas para conectar ao servidor por meio do protocolo MAPI/HTTP. Este cabeçalho é aplicável a clientes que implementam o protocolo MAPI/HTTP.  <br/> |
|X-ClientCanHandle  <br/> |Este cabeçalho contém uma lista delimitada por vírgula dos recursos que o cliente oferece suporte. Os valores possíveis são especificados na tabela 2.  <br/> |
   
**Tabela 2. Valores de cabeçalho X-ClientCanHandle**

|**X-ClientCanHandle valor (diferenciam maiusculas e minúsculas)**|**Versão mínima do servidor**|**Descrição**|
|:-----|:-----|:-----|
|Negociar  <br/> |15.00.0995.014  <br/> |Se este valor estiver presente, o servidor retornará um valor igual a "Negociar" no elemento [AuthPackage (POX)](authpackage-pox.md) se o servidor está configurado para aceitar a autenticação negociar. Se este valor não estiver presente, o servidor não retornará um valor igual a "Negociar" no elemento **AuthPackage** .  <br/> |
|ExHttpInfo  <br/> |15.00.0995.014  <br/> |Se este valor estiver presente, o servidor retornará um elemento de [Protocolo POX ()](protocol-pox.md) com um elemento de [Tipo POX ()](type-pox.md) definido como "EXHTTP" se o servidor está configurado para aceitar conexões de RPC/HTTP. Se este valor não estiver presente, o servidor não retornará um elemento de **protocolo** com um elemento de **tipo** definido como "EXHTTP".  <br/> |
   
### <a name="request-elements"></a>Elementos de solicitação

Os seguintes elementos são usados no corpo da solicitação:
  
- [Descoberta automática (POX)](autodiscover-pox.md)
    
- [Solicitação (POX)](request-pox.md)
    
- [AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md)
    
- [EMailAddress POX)](emailaddress-pox.md)
    
> [!NOTE]
> O elemento [LegacyDN POX ()](legacydn-pox.md) pode ser usado no lugar do elemento [EMailAddress POX ()](emailaddress-pox.md) . 
  
### <a name="version-differences"></a>Diferenças de versão

O cabeçalho X-MapiHttpCapability está disponível no Office 365, Exchange Online e versões do Exchange, começando com o build 15.00.0847.032 (Exchange Server 2013 SP1) no local.
  
O cabeçalho X-ClientCanHandle está disponível no Office 365, Exchange Online e versões do Exchange, começando com o build 15.00.0995.014 no local.
  
## <a name="see-also"></a>Confira também



[Resposta de descoberta automática POX para Exchange](pox-autodiscover-response-for-exchange.md)


[Referência do serviço web POX descoberta automática do Exchange](pox-autodiscover-web-service-reference-for-exchange.md)
  
[Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

