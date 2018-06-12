---
title: Operação de ResetPIN (serviço web de Unificação de mensagens)
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
description: A operação ResetPIN altera o PIN (senha TUI) para um novo valor aleatório.
ms.openlocfilehash: e6417b86ce17c0d34fe857cf1209a18972cbef63
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825146"
---
# <a name="resetpin-operation-um-web-service"></a><span data-ttu-id="97b44-103">Operação de ResetPIN (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="97b44-103">ResetPIN operation (UM web service)</span></span>

<span data-ttu-id="97b44-104">A operação ResetPIN altera o PIN (senha TUI) para um novo valor aleatório.</span><span class="sxs-lookup"><span data-stu-id="97b44-104">The ResetPIN operation changes the PIN (TUI password) to a new random value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="97b44-105">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="97b44-105">Remarks</span></span>

<span data-ttu-id="97b44-106">A operação ResetPIN cria um novo PIN baseado nas diretivas de PIN.</span><span class="sxs-lookup"><span data-stu-id="97b44-106">The ResetPIN operation creates a new PIN based on the PIN policies.</span></span> <span data-ttu-id="97b44-107">Se a operação for bem-sucedida, uma mensagem de email que contém o novo PIN é enviada à caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="97b44-107">If the operation is successful, an e-mail message that contains the new PIN is sent to the mailbox of the user.</span></span> <span data-ttu-id="97b44-108">Se a operação falhar, ele lançará uma exceção que contém informações sobre a falha.</span><span class="sxs-lookup"><span data-stu-id="97b44-108">If the operation fails, it will throw an exception that contains information about the failure.</span></span>
  
## <a name="resetpin-request-example"></a><span data-ttu-id="97b44-109">Exemplo de solicitação de ResetPIN</span><span class="sxs-lookup"><span data-stu-id="97b44-109">ResetPIN request example</span></span>

### <a name="description"></a><span data-ttu-id="97b44-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="97b44-110">Description</span></span>

<span data-ttu-id="97b44-111">O exemplo a seguir de uma solicitação de ResetPIN mostra como uma solicitação para redefinir o PIN para uma caixa de correio de formulário.</span><span class="sxs-lookup"><span data-stu-id="97b44-111">The following example of a ResetPIN request shows how to form a request to reset the PIN for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="97b44-112">Código</span><span class="sxs-lookup"><span data-stu-id="97b44-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a><span data-ttu-id="97b44-113">Exemplo de resposta bem-sucedida ResetPIN</span><span class="sxs-lookup"><span data-stu-id="97b44-113">Successful ResetPIN response example</span></span>

### <a name="description"></a><span data-ttu-id="97b44-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="97b44-114">Description</span></span>

<span data-ttu-id="97b44-115">O exemplo a seguir de uma resposta ResetPIN mostra uma resposta à solicitação de ResetPIN.</span><span class="sxs-lookup"><span data-stu-id="97b44-115">The following example of a ResetPIN response shows a response to the ResetPIN request.</span></span>
  
### <a name="code"></a><span data-ttu-id="97b44-116">Código</span><span class="sxs-lookup"><span data-stu-id="97b44-116">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="97b44-117">Confira também</span><span class="sxs-lookup"><span data-stu-id="97b44-117">See also</span></span>



[<span data-ttu-id="97b44-118">ResetPIN (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="97b44-118">ResetPIN (UM web service)</span></span>](resetpin-um-web-service.md)
  
[<span data-ttu-id="97b44-119">ResetPINResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="97b44-119">ResetPINResponse (UM web service)</span></span>](resetpinresponse-um-web-service.md)

