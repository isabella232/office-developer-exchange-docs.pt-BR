---
title: UnsubscribeResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnsubscribeResponse
api_type:
- schema
ms.assetid: 125e0326-6522-42cd-b20e-6977e6fde249
description: O elemento UnsubscribeResponse define uma resposta a uma solicitação de cancelamento de assinatura.
ms.openlocfilehash: 1a8ddf93499acb7aa369ec9e91a7106e5cb4bd53
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467197"
---
# <a name="unsubscriberesponse"></a><span data-ttu-id="aaeed-103">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="aaeed-103">UnsubscribeResponse</span></span>

<span data-ttu-id="aaeed-104">O elemento **UnsubscribeResponse** define uma resposta a uma solicitação de cancelamento de assinatura.</span><span class="sxs-lookup"><span data-stu-id="aaeed-104">The **UnsubscribeResponse** element defines a response to an Unsubscribe request.</span></span> 
  
```xml
<UnsubscribeResponse>
   <ResponseMessages/>
</UnsubscribeResponse>
```

 <span data-ttu-id="aaeed-105">**UnsubscribeResponseType**</span><span class="sxs-lookup"><span data-stu-id="aaeed-105">**UnsubscribeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aaeed-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="aaeed-106">Attributes and elements</span></span>

<span data-ttu-id="aaeed-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="aaeed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aaeed-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="aaeed-108">Attributes</span></span>

<span data-ttu-id="aaeed-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aaeed-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aaeed-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="aaeed-110">Child elements</span></span>

|<span data-ttu-id="aaeed-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aaeed-111">**Element**</span></span>|<span data-ttu-id="aaeed-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aaeed-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aaeed-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="aaeed-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="aaeed-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="aaeed-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aaeed-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="aaeed-115">Parent elements</span></span>

<span data-ttu-id="aaeed-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aaeed-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aaeed-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="aaeed-117">Remarks</span></span>

<span data-ttu-id="aaeed-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="aaeed-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aaeed-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="aaeed-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aaeed-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="aaeed-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aaeed-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="aaeed-121">Schema name</span></span>  <br/> |<span data-ttu-id="aaeed-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="aaeed-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aaeed-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="aaeed-123">Validation file</span></span>  <br/> |<span data-ttu-id="aaeed-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="aaeed-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aaeed-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="aaeed-125">Can be empty</span></span>  <br/> |<span data-ttu-id="aaeed-126">False</span><span class="sxs-lookup"><span data-stu-id="aaeed-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aaeed-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="aaeed-127">See also</span></span>



- [<span data-ttu-id="aaeed-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="aaeed-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

