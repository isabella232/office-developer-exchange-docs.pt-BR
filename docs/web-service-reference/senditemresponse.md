---
title: SendItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItemResponse
api_type:
- schema
ms.assetid: 26ac41c7-57d9-473e-ab7a-bae93e1d2aba
description: O elemento de SendItemResponse define uma resposta a uma solicitação de SendItem.
ms.openlocfilehash: 41f450e1d4c95f7ba389adcaa2ed7e18ea74d61c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2018
ms.locfileid: "19825339"
---
# <a name="senditemresponse"></a><span data-ttu-id="2cef9-103">SendItemResponse</span><span class="sxs-lookup"><span data-stu-id="2cef9-103">SendItemResponse</span></span>

<span data-ttu-id="2cef9-104">O elemento de **SendItemResponse** define uma resposta a uma solicitação de SendItem.</span><span class="sxs-lookup"><span data-stu-id="2cef9-104">The **SendItemResponse** element defines a response to a SendItem request.</span></span> 
  
```xml
<SendItemResponse>
   <ResponseMessages/>
</SendItemResponse>
```

 <span data-ttu-id="2cef9-105">**SendItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="2cef9-105">**SendItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2cef9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2cef9-106">Attributes and elements</span></span>

<span data-ttu-id="2cef9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2cef9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2cef9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2cef9-108">Attributes</span></span>

<span data-ttu-id="2cef9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2cef9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2cef9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2cef9-110">Child elements</span></span>

|<span data-ttu-id="2cef9-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2cef9-111">**Element**</span></span>|<span data-ttu-id="2cef9-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2cef9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cef9-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2cef9-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="2cef9-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2cef9-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2cef9-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2cef9-115">Parent elements</span></span>

<span data-ttu-id="2cef9-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2cef9-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2cef9-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="2cef9-117">Remarks</span></span>

<span data-ttu-id="2cef9-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="2cef9-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2cef9-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2cef9-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2cef9-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="2cef9-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2cef9-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2cef9-121">Schema name</span></span>  <br/> |<span data-ttu-id="2cef9-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="2cef9-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2cef9-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2cef9-123">Validation file</span></span>  <br/> |<span data-ttu-id="2cef9-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2cef9-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2cef9-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="2cef9-125">Can be empty</span></span>  <br/> |<span data-ttu-id="2cef9-126">False</span><span class="sxs-lookup"><span data-stu-id="2cef9-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2cef9-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="2cef9-127">See also</span></span>



[<span data-ttu-id="2cef9-128">Operação SendItem</span><span class="sxs-lookup"><span data-stu-id="2cef9-128">SendItem operation</span></span>](senditem-operation.md)
  
[<span data-ttu-id="2cef9-129">SendItem</span><span class="sxs-lookup"><span data-stu-id="2cef9-129">SendItem</span></span>](senditem.md)


- [<span data-ttu-id="2cef9-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2cef9-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

