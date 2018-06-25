---
title: Operação de SetPlayOnPhoneDialString (serviço web de Unificação de mensagens)
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
description: A operação SetPlayOnPhoneDialString define a sequência de discagem para usar como o padrão para a operação PlayOnPhone (serviço web de Unificação de mensagens) e a operação de PlayOnPhoneGreeting (serviço web de Unificação de mensagens).
ms.openlocfilehash: 0d1a879784740777e5eab0cbd5f85e59a6479461
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825446"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a><span data-ttu-id="44d35-103">Operação de SetPlayOnPhoneDialString (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="44d35-103">SetPlayOnPhoneDialString operation (UM web service)</span></span>

<span data-ttu-id="44d35-104">A operação SetPlayOnPhoneDialString define a sequência de discagem para usar como o padrão para a [operação PlayOnPhone (serviço web de Unificação de mensagens)](playonphone-operation-um-web-service.md) e a [operação PlayOnPhoneGreeting (serviço web de Unificação de mensagens)](playonphonegreeting-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="44d35-104">The SetPlayOnPhoneDialString operation sets the dial string to use as the default for the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and the [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span>
  
## <a name="setplayonphonedialstring-request-example"></a><span data-ttu-id="44d35-105">Exemplo de solicitação de SetPlayOnPhoneDialString</span><span class="sxs-lookup"><span data-stu-id="44d35-105">SetPlayOnPhoneDialString request example</span></span>

### <a name="description"></a><span data-ttu-id="44d35-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="44d35-106">Description</span></span>

<span data-ttu-id="44d35-107">O exemplo a seguir de uma solicitação de SetPlayOnPhoneDialString mostra como uma solicitação para definir a sequência de discagem padrão para uma caixa de correio de formulário.</span><span class="sxs-lookup"><span data-stu-id="44d35-107">The following example of a SetPlayOnPhoneDialString request shows how to form a request to set the default dial string for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="44d35-108">Código</span><span class="sxs-lookup"><span data-stu-id="44d35-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetPlayOnPhoneDialString xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <dialString>12345</dialString>
    </SetPlayOnPhoneDialString>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setplayonphonedialstring-response-example"></a><span data-ttu-id="44d35-109">Exemplo de resposta bem-sucedida SetPlayOnPhoneDialString</span><span class="sxs-lookup"><span data-stu-id="44d35-109">Successful SetPlayOnPhoneDialString response example</span></span>

### <a name="description"></a><span data-ttu-id="44d35-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="44d35-110">Description</span></span>

<span data-ttu-id="44d35-111">O exemplo a seguir de uma resposta SetPlayOnePhoneDialString mostra uma resposta à solicitação de SetPlayOnPhoneDialString.</span><span class="sxs-lookup"><span data-stu-id="44d35-111">The following example of a SetPlayOnePhoneDialString response shows a response to the SetPlayOnPhoneDialString request.</span></span>
  
### <a name="code"></a><span data-ttu-id="44d35-112">Código</span><span class="sxs-lookup"><span data-stu-id="44d35-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetPlayOnPhoneDialStringResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="44d35-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="44d35-113">See also</span></span>



[<span data-ttu-id="44d35-114">SetPlayOnPhoneDialString (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="44d35-114">SetPlayOnPhoneDialString (UM web service)</span></span>](setplayonphonedialstring-um-web-service.md)
  
[<span data-ttu-id="44d35-115">SetPlayOnPhoneDialStringResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="44d35-115">SetPlayOnPhoneDialStringResponse (UM web service)</span></span>](setplayonphonedialstringresponse-um-web-service.md)
  
[<span data-ttu-id="44d35-116">dialString (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="44d35-116">dialString (UM web service)</span></span>](dialstring-um-web-service.md)

