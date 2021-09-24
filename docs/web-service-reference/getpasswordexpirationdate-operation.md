---
title: Operação GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b0297458-58fb-4e5d-bb47-0cd17155e106
description: A operação GetPasswordExpirationDate fornece a data de expiração da senha da conta de email para o usuário atual.
ms.openlocfilehash: 07928fd3e6fca410a292d6cd74f1240d8e81c42f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524235"
---
# <a name="getpasswordexpirationdate-operation"></a>Operação GetPasswordExpirationDate

A **operação GetPasswordExpirationDate** fornece a data de expiração da senha da conta de email para o usuário atual. 
  
Essa operação foi introduzida no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a>Headers soap da operação GetPasswordExpirationDate

A **operação GetPasswordExpirationDate** pode usar os headers SOAP listados na tabela a seguir. 
  
|**Header**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido na RFC 3066, "Marcas para a Identificação de Idiomas", a ser usada para acessar a caixa de correio. Isso é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica o esquema da solicitação de operação. Isso é aplicável a uma solicitação. Isso é aplicável a uma solicitação.  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a>Exemplo de solicitação de operação GetPasswordExpirationDate

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de operação **GetPasswordExpirationDate** mostra como obter a data de expiração da senha para uma conta de email. 
  
### <a name="code"></a>Código

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
  </soap:Header>
  <soap:Body>
    <tns:GetPasswordExpirationDate>
      <tns:MailboxSmtpAddress>user1@DTZMZX-dom.extest.microsoft.com</tns:MailboxSmtpAddress>
    </tns:GetPasswordExpirationDate>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a>Elementos request

Os seguintes elementos são usados na solicitação:
  
- [GetPasswordExpirationDate](getpasswordexpirationdate.md)
    
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a>Resposta bem-sucedida da operação GetPasswordExpirationDate

Os seguintes elementos são usados na resposta:
  
- [GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md)
    
- [PasswordExpirationDate](passwordexpirationdate.md)
    

