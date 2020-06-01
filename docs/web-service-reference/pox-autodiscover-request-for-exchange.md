---
title: Solicitação de descoberta automática do POX para o Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: A solicitação de descoberta automática contém uma consulta para a configuração de acesso do cliente de um usuário.
ms.openlocfilehash: b2138f9813c7b75aef9afb90089b9b874aac7532
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461664"
---
# <a name="pox-autodiscover-request-for-exchange"></a>Solicitação de descoberta automática do POX para o Exchange

A solicitação de descoberta automática contém uma consulta para a configuração de acesso do cliente de um usuário.
  
## <a name="autodiscover-request-example"></a>Exemplo de solicitação de descoberta automática

### <a name="description"></a>Descrição

O exemplo de XML a seguir mostra um corpo de solicitação de descoberta automática.
  
### <a name="code"></a>Código

```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a>Cabeçalhos de solicitação

Os seguintes cabeçalhos HTTP são opcionais ao enviar solicitações de descoberta automática.
  
**Tabela 1. Cabeçalhos de solicitação HTTP**

|**Header**|**Descrição**|
|:-----|:-----|
|X-MapiHttpCapability  <br/> |Se presente e definido como "1", indica que o cliente está solicitando informações que podem ser usadas para se conectar ao servidor usando o protocolo MAPI/HTTP. Esse cabeçalho é aplicável aos clientes que implementam o protocolo MAPI/HTTP.  <br/> |
|X-ClientCanHandle  <br/> |Este cabeçalho contém uma lista delimitada por vírgulas de recursos aos quais o cliente oferece suporte. Os valores possíveis são especificados na tabela 2.  <br/> |
   
**Tabela 2. Valores de cabeçalho X-ClientCanHandle**

|**Valor X-ClientCanHandle (não diferencia maiúsculas de minúsculas)**|**Versão mínima do servidor**|**Descrição**|
|:-----|:-----|:-----|
|Negocia  <br/> |15.00.0995.014  <br/> |Se esse valor estiver presente, o servidor retornará um valor de "Negotiate" no elemento [AuthPackage (POX)](authpackage-pox.md) se o servidor estiver configurado para aceitar a autenticação de negociação. Se esse valor não estiver presente, o servidor não retornará um valor de "Negotiate" no elemento **AuthPackage** .  <br/> |
|ExHttpInfo  <br/> |15.00.0995.014  <br/> |Se esse valor estiver presente, o servidor retornará um elemento de [protocolo (POX)](protocol-pox.md) com um [tipo (POX)](type-pox.md) definido como "exhttp" se o servidor estiver configurado para aceitar conexões RPC/http. Se esse valor não estiver presente, o servidor não retornará um elemento de **protocolo** com um elemento **Type** definido como "exhttp".  <br/> |
   
### <a name="request-elements"></a>Elementos Request

Os seguintes elementos são usados no corpo da solicitação:
  
- [Descoberta automática (POX)](autodiscover-pox.md)
    
- [Solicitação (POX)](request-pox.md)
    
- [AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md)
    
- [EMailAddress (POX)](emailaddress-pox.md)
    
> [!NOTE]
> O elemento [LegacyDN (POX)](legacydn-pox.md) pode ser usado no lugar do elemento [EMailAddress (POX)](emailaddress-pox.md) . 
  
### <a name="version-differences"></a>Diferenças de versão

O cabeçalho X-MapiHttpCapability está disponível no Office 365, no Exchange Online e nas versões locais do Exchange a partir do Build 15.00.0847.032 (Exchange Server 2013 SP1).
  
O cabeçalho X-ClientCanHandle está disponível no Office 365, no Exchange Online e nas versões locais do Exchange a partir do Build 15.00.0995.014.
  
## <a name="see-also"></a>Também consulte



[Resposta de descoberta automática do POX para o Exchange](pox-autodiscover-response-for-exchange.md)


[Referência de serviço Web de descoberta automática do POX para o Exchange](pox-autodiscover-web-service-reference-for-exchange.md)
  
[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

