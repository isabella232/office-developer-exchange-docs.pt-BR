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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457890"
---
# <a name="getpasswordexpirationdate-operation"></a><span data-ttu-id="30167-103">Operação GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="30167-103">GetPasswordExpirationDate operation</span></span>

<span data-ttu-id="30167-104">A operação **GetPasswordExpirationDate** fornece a data de expiração da senha da conta de email do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="30167-104">The **GetPasswordExpirationDate** operation provides the email account password expiration date for the current user.</span></span> 
  
<span data-ttu-id="30167-105">Essa operação foi introduzida no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="30167-105">This operation was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a><span data-ttu-id="30167-106">Cabeçalhos SOAP de operação GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="30167-106">GetPasswordExpirationDate operation SOAP headers</span></span>

<span data-ttu-id="30167-107">A operação **GetPasswordExpirationDate** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="30167-107">The **GetPasswordExpirationDate** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="30167-108">**Header**</span><span class="sxs-lookup"><span data-stu-id="30167-108">**Header**</span></span>|<span data-ttu-id="30167-109">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="30167-109">**Element**</span></span>|<span data-ttu-id="30167-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="30167-110">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="30167-111">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="30167-111">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="30167-112">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="30167-112">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="30167-113">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="30167-113">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="30167-114">Isso se aplica a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="30167-114">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="30167-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="30167-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="30167-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="30167-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="30167-117">Identifica o esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="30167-117">Identifies the schema for the operation request.</span></span> <span data-ttu-id="30167-118">Isso se aplica a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="30167-118">This is applicable to a request.</span></span> <span data-ttu-id="30167-119">Isso se aplica a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="30167-119">This is applicable to a request.</span></span>  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a><span data-ttu-id="30167-120">Exemplo de solicitação de operação GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="30167-120">GetPasswordExpirationDate operation request example</span></span>

### <a name="description"></a><span data-ttu-id="30167-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="30167-121">Description</span></span>

<span data-ttu-id="30167-122">O exemplo a seguir de uma solicitação de operação do **GetPasswordExpirationDate** mostra como obter a data de expiração da senha de uma conta de email.</span><span class="sxs-lookup"><span data-stu-id="30167-122">The following example of a **GetPasswordExpirationDate** operation request shows how to get the password expiration date for an email account.</span></span> 
  
### <a name="code"></a><span data-ttu-id="30167-123">Código</span><span class="sxs-lookup"><span data-stu-id="30167-123">Code</span></span>

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

### <a name="request-elements"></a><span data-ttu-id="30167-124">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="30167-124">Request elements</span></span>

<span data-ttu-id="30167-125">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="30167-125">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="30167-126">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="30167-126">GetPasswordExpirationDate</span></span>](getpasswordexpirationdate.md)
    
- [<span data-ttu-id="30167-127">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="30167-127">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a><span data-ttu-id="30167-128">Resposta de operação GetPasswordExpirationDate bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="30167-128">Successful GetPasswordExpirationDate operation response</span></span>

<span data-ttu-id="30167-129">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="30167-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="30167-130">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="30167-130">GetPasswordExpirationDateResponse</span></span>](getpasswordexpirationdateresponse.md)
    
- [<span data-ttu-id="30167-131">PasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="30167-131">PasswordExpirationDate</span></span>](passwordexpirationdate.md)
    

