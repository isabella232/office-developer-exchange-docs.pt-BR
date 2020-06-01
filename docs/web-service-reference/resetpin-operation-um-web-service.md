---
title: Operação ResetPIN (serviço Web da UM)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- ResetPIN
api_type:
- schema
ms.assetid: c0f14a15-3389-4311-8bac-f87930c5f5d4
description: A operação ResetPIN altera o PIN (TUI senha) para um novo valor aleatório.
ms.openlocfilehash: 8de64ce7a47e9c426f8eb9298e1ca00508fb616c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44465489"
---
# <a name="resetpin-operation-um-web-service"></a><span data-ttu-id="a022a-103">Operação ResetPIN (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="a022a-103">ResetPIN operation (UM web service)</span></span>

<span data-ttu-id="a022a-104">A operação ResetPIN altera o PIN (TUI senha) para um novo valor aleatório.</span><span class="sxs-lookup"><span data-stu-id="a022a-104">The ResetPIN operation changes the PIN (TUI password) to a new random value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a022a-105">Comentários</span><span class="sxs-lookup"><span data-stu-id="a022a-105">Remarks</span></span>

<span data-ttu-id="a022a-106">A operação ResetPIN cria um novo PIN com base nas políticas de PIN.</span><span class="sxs-lookup"><span data-stu-id="a022a-106">The ResetPIN operation creates a new PIN based on the PIN policies.</span></span> <span data-ttu-id="a022a-107">Se a operação for bem-sucedida, uma mensagem de email que contenha o novo PIN será enviada para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a022a-107">If the operation is successful, an e-mail message that contains the new PIN is sent to the mailbox of the user.</span></span> <span data-ttu-id="a022a-108">Se a operação falhar, ela gerará uma exceção que contém informações sobre a falha.</span><span class="sxs-lookup"><span data-stu-id="a022a-108">If the operation fails, it will throw an exception that contains information about the failure.</span></span>
  
## <a name="resetpin-request-example"></a><span data-ttu-id="a022a-109">Exemplo de solicitação ResetPIN</span><span class="sxs-lookup"><span data-stu-id="a022a-109">ResetPIN request example</span></span>

### <a name="description"></a><span data-ttu-id="a022a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a022a-110">Description</span></span>

<span data-ttu-id="a022a-111">O exemplo a seguir de uma solicitação ResetPIN mostra como formar uma solicitação para redefinir o PIN de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a022a-111">The following example of a ResetPIN request shows how to form a request to reset the PIN for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="a022a-112">Código</span><span class="sxs-lookup"><span data-stu-id="a022a-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a><span data-ttu-id="a022a-113">Exemplo de resposta ResetPIN bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="a022a-113">Successful ResetPIN response example</span></span>

### <a name="description"></a><span data-ttu-id="a022a-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="a022a-114">Description</span></span>

<span data-ttu-id="a022a-115">O exemplo a seguir de uma resposta ResetPIN mostra uma resposta à solicitação ResetPIN.</span><span class="sxs-lookup"><span data-stu-id="a022a-115">The following example of a ResetPIN response shows a response to the ResetPIN request.</span></span>
  
### <a name="code"></a><span data-ttu-id="a022a-116">Código</span><span class="sxs-lookup"><span data-stu-id="a022a-116">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="a022a-117">Também consulte</span><span class="sxs-lookup"><span data-stu-id="a022a-117">See also</span></span>



[<span data-ttu-id="a022a-118">ResetPIN (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="a022a-118">ResetPIN (UM web service)</span></span>](resetpin-um-web-service.md)
  
[<span data-ttu-id="a022a-119">ResetPINResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="a022a-119">ResetPINResponse (UM web service)</span></span>](resetpinresponse-um-web-service.md)

