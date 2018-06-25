---
title: Operação GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0297458-58fb-4e5d-bb47-0cd17155e106
description: A operação GetPasswordExpirationDate fornece a data de expiração de senha de conta de email para o usuário atual.
ms.openlocfilehash: c57942c88b09a910e2d529a12ea279bb2da5d693
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752584"
---
# <a name="getpasswordexpirationdate-operation"></a>Operação GetPasswordExpirationDate

A operação **GetPasswordExpirationDate** fornece a data de expiração de senha de conta de email para o usuário atual. 
  
Essa operação foi introduzida no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a>Cabeçalhos SOAP GetPasswordExpirationDate operação

A operação **GetPasswordExpirationDate** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir. 
  
|**Header**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio. Isso é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica o esquema para a solicitação de operação. Isso é aplicável a uma solicitação. Isso é aplicável a uma solicitação.  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a>Exemplo de solicitação de operação GetPasswordExpirationDate

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de operação **GetPasswordExpirationDate** mostra como obter a data de expiração de senha para uma conta de email. 
  
### <a name="code"></a>Código

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
  </soap:Header>
  <soap:Body>
    <tns:GetPasswordExpirationDate>
      <tns:MailboxSmtpAddress>user1@DTZMZX-dom.extest.microsoft.com</tns:MailboxSmtpAddress>
    </tns:GetPasswordExpirationDate>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a>Elementos de solicitação

Os seguintes elementos são usados na solicitação:
  
- [GetPasswordExpirationDate](getpasswordexpirationdate.md)
    
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a>Resposta de operação GetPasswordExpirationDate bem-sucedida

Os seguintes elementos são usados na resposta:
  
- [GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md)
    
- [PasswordExpirationDate](passwordexpirationdate.md)
    

