---
title: GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f4f958ed-9cf4-4ebf-9b01-e2df9a7cbd63
description: O elemento GetPasswordExpirationDate define uma solicitação para obter a data de expiração da senha de uma conta de email. Esse elemento é o elemento base da operação GetPasswordExpirationDate.
ms.openlocfilehash: e5c74cc773438780fad0448cd2ae449dae07738f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520511"
---
# <a name="getpasswordexpirationdate"></a>GetPasswordExpirationDate

O **elemento GetPasswordExpirationDate** define uma solicitação para obter a data de expiração da senha de uma conta de email. Esse elemento é o elemento base da operação [GetPasswordExpirationDate.](getpasswordexpirationdate-operation.md) 
  
```XML
<GetPasswordExpirationDate>
    <MailboxSmtpAddress/>
</GetPasswordExpirationDate>
```

 **GetPasswordExpirationDateType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Nome do elemento**|**Descrição**|
|:-----|:-----|
|[MailboxSmtpAddress](mailboxsmtpaddress.md) <br/> |Representa o endereço de email da conta de email para a qual a data de expiração da senha deve ser retornada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetPasswordExpirationDate](getpasswordexpirationdate-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

