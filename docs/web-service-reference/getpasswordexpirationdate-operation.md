---
title: Operação GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0297458-58fb-4e5d-bb47-0cd17155e106
description: A operação GetPasswordExpirationDate fornece a data de expiração da senha da conta de email do usuário atual.
ms.openlocfilehash: 4184092cf98161e4c2f74446cef5439722ae71a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457890"
---
# <a name="getpasswordexpirationdate-operation"></a>Operação GetPasswordExpirationDate

A operação **GetPasswordExpirationDate** fornece a data de expiração da senha da conta de email do usuário atual. 
  
Essa operação foi introduzida no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a>Cabeçalhos SOAP de operação GetPasswordExpirationDate

A operação **GetPasswordExpirationDate** pode usar os cabeçalhos SOAP listados na tabela a seguir. 
  
|**Header**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio. Isso se aplica a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica o esquema para a solicitação de operação. Isso se aplica a uma solicitação. Isso se aplica a uma solicitação.  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a>Exemplo de solicitação de operação GetPasswordExpirationDate

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de operação do **GetPasswordExpirationDate** mostra como obter a data de expiração da senha de uma conta de email. 
  
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

### <a name="request-elements"></a>Elementos Request

Os seguintes elementos são usados na solicitação:
  
- [GetPasswordExpirationDate](getpasswordexpirationdate.md)
    
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a>Resposta de operação GetPasswordExpirationDate bem-sucedida

Os seguintes elementos são usados na resposta:
  
- [GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md)
    
- [PasswordExpirationDate](passwordexpirationdate.md)
    

