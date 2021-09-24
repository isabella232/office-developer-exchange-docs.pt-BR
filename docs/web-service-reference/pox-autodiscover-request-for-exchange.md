---
title: Solicitação de Descoberta Automática POX para Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: A solicitação descoberta automática contém uma consulta para a configuração de acesso para cliente de um usuário.
ms.openlocfilehash: 8a0960dcff21276baf723512befacc4eca35950f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523863"
---
# <a name="pox-autodiscover-request-for-exchange"></a>Solicitação de Descoberta Automática POX para Exchange

A solicitação descoberta automática contém uma consulta para a configuração de acesso para cliente de um usuário.
  
## <a name="autodiscover-request-example"></a>Exemplo de solicitação de descoberta automática

### <a name="description"></a>Descrição

O exemplo XML a seguir mostra um corpo da solicitação de Descoberta Automática.
  
### <a name="code"></a>Código

```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a>Headers de solicitação

Os seguintes cabeçalhos HTTP são opcionais ao enviar solicitações de Descoberta Automática.
  
**Tabela 1. Cabeçalhos de solicitação HTTP**

|**Header**|**Descrição**|
|:-----|:-----|
|X-MapiHttpCapability  <br/> |Se presente e definido como "1", indica que o cliente está solicitando informações que podem ser usadas para se conectar ao servidor usando o protocolo MAPI/HTTP. Esse cabeçalho é aplicável aos clientes que implementam o protocolo MAPI/HTTP.  <br/> |
|X-ClientCanHandle  <br/> |Esse header contém uma lista delimitada por vírgulas dos recursos que o cliente oferece suporte. Os valores possíveis são especificados na Tabela 2.  <br/> |
   
**Tabela 2. Valores de header X-ClientCanHandle**

|**Valor X-ClientCanHandle (sem maiúsculas de minúsculas)**|**Versão mínima do servidor**|**Descrição**|
|:-----|:-----|:-----|
|Negociar  <br/> |15.00.0995.014  <br/> |Se esse valor estiver presente, o servidor retornará um valor de "Negociar" no elemento [AuthPackage (POX)](authpackage-pox.md) se o servidor estiver configurado para aceitar a autenticação Negociar. Se esse valor não estiver presente, o servidor não retornará um valor de "Negociar" no **elemento AuthPackage.**  <br/> |
|ExHttpInfo  <br/> |15.00.0995.014  <br/> |Se esse valor estiver presente, o servidor retornará um elemento [Protocol (POX)](protocol-pox.md) com um elemento [Type (POX)](type-pox.md) definido como "EXHTTP" se o servidor estiver configurado para aceitar conexões RPC/HTTP. Se esse valor não estiver presente, o servidor não retornará um elemento **Protocol** com um elemento **Type** definido como "EXHTTP".  <br/> |
   
### <a name="request-elements"></a>Elementos request

Os seguintes elementos são usados no corpo da solicitação:
  
- [AutoDiscover (POX)](autodiscover-pox.md)
    
- [Request (POX)](request-pox.md)
    
- [AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md)
    
- [EMailAddress (POX)](emailaddress-pox.md)
    
> [!NOTE]
> O [elemento LegacyDN (POX)](legacydn-pox.md) pode ser usado no lugar do [elemento EMailAddress (POX).](emailaddress-pox.md) 
  
### <a name="version-differences"></a>Diferenças de versão

O header X-MapiHttpCapability está disponível nas versões Office 365, Exchange Online e local do Exchange a partir da com build 15.00.0847.032 (Exchange Server 2013 SP1).
  
O header X-ClientCanHandle está disponível em versões Office 365, Exchange Online e local do Exchange a partir da com build 15.00.0995.014.
  
## <a name="see-also"></a>Confira também



[Resposta de Descoberta Automática POX para Exchange](pox-autodiscover-response-for-exchange.md)


[Referência do serviço Web de Descoberta Automática POX para Exchange](pox-autodiscover-web-service-reference-for-exchange.md)
  
[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

