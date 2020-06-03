---
title: Operação SetPlayOnPhoneDialString (serviço Web da UM)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: a68479f2-d900-4dd8-a5ce-dbea8247e841
description: A operação SetPlayOnPhoneDialString define a cadeia de caracteres de discagem a ser usada como padrão para a operação PlayOnPhone (serviço Web da UM) e a operação PlayOnPhoneGreeting (serviço Web da UM).
ms.openlocfilehash: 7df806eedc2d6d037394f31ec4ccbfe28aaf3372
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458639"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a><span data-ttu-id="73332-103">Operação SetPlayOnPhoneDialString (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="73332-103">SetPlayOnPhoneDialString operation (UM web service)</span></span>

<span data-ttu-id="73332-104">A operação SetPlayOnPhoneDialString define a cadeia de caracteres de discagem a ser usada como padrão para a [operação PlayOnPhone (serviço Web da um)](playonphone-operation-um-web-service.md) e a [operação PlayOnPhoneGreeting (serviço Web da um)](playonphonegreeting-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="73332-104">The SetPlayOnPhoneDialString operation sets the dial string to use as the default for the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and the [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span>
  
## <a name="setplayonphonedialstring-request-example"></a><span data-ttu-id="73332-105">Exemplo de solicitação SetPlayOnPhoneDialString</span><span class="sxs-lookup"><span data-stu-id="73332-105">SetPlayOnPhoneDialString request example</span></span>

### <a name="description"></a><span data-ttu-id="73332-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="73332-106">Description</span></span>

<span data-ttu-id="73332-107">O exemplo a seguir de uma solicitação SetPlayOnPhoneDialString mostra como formar uma solicitação para definir a cadeia de caracteres de discagem padrão para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="73332-107">The following example of a SetPlayOnPhoneDialString request shows how to form a request to set the default dial string for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="73332-108">Código</span><span class="sxs-lookup"><span data-stu-id="73332-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetPlayOnPhoneDialString xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <dialString>12345</dialString>
    </SetPlayOnPhoneDialString>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setplayonphonedialstring-response-example"></a><span data-ttu-id="73332-109">Exemplo de resposta SetPlayOnPhoneDialString bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="73332-109">Successful SetPlayOnPhoneDialString response example</span></span>

### <a name="description"></a><span data-ttu-id="73332-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="73332-110">Description</span></span>

<span data-ttu-id="73332-111">O exemplo a seguir de uma resposta SetPlayOnePhoneDialString mostra uma resposta à solicitação SetPlayOnPhoneDialString.</span><span class="sxs-lookup"><span data-stu-id="73332-111">The following example of a SetPlayOnePhoneDialString response shows a response to the SetPlayOnPhoneDialString request.</span></span>
  
### <a name="code"></a><span data-ttu-id="73332-112">Código</span><span class="sxs-lookup"><span data-stu-id="73332-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetPlayOnPhoneDialStringResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="73332-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="73332-113">See also</span></span>



[<span data-ttu-id="73332-114">SetPlayOnPhoneDialString (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="73332-114">SetPlayOnPhoneDialString (UM web service)</span></span>](setplayonphonedialstring-um-web-service.md)
  
[<span data-ttu-id="73332-115">SetPlayOnPhoneDialStringResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="73332-115">SetPlayOnPhoneDialStringResponse (UM web service)</span></span>](setplayonphonedialstringresponse-um-web-service.md)
  
[<span data-ttu-id="73332-116">dialstring (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="73332-116">dialString (UM web service)</span></span>](dialstring-um-web-service.md)

