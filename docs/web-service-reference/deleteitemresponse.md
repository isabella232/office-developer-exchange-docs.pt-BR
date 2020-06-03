---
title: DeleteItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemResponse
api_type:
- schema
ms.assetid: 86463d66-fe47-4a19-a81b-e24841e816ab
description: O elemento DeleteItemResponse define uma resposta a uma única solicitação de DeleteItem.
ms.openlocfilehash: 6aad30077e8867486012dd34bb1def97accffc2b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529193"
---
# <a name="deleteitemresponse"></a><span data-ttu-id="dd87d-103">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="dd87d-103">DeleteItemResponse</span></span>

<span data-ttu-id="dd87d-104">O elemento **DeleteItemResponse** define uma resposta a uma única solicitação de DeleteItem.</span><span class="sxs-lookup"><span data-stu-id="dd87d-104">The **DeleteItemResponse** element defines a response to a single DeleteItem request.</span></span> 
  
```xml
<DeleteItemResponse>
   <ResponseMessages/>
</DeleteItemResponse>
```

 <span data-ttu-id="dd87d-105">**DeleteItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="dd87d-105">**DeleteItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd87d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="dd87d-106">Attributes and elements</span></span>

<span data-ttu-id="dd87d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dd87d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd87d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="dd87d-108">Attributes</span></span>

<span data-ttu-id="dd87d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd87d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd87d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dd87d-110">Child elements</span></span>

|<span data-ttu-id="dd87d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dd87d-111">**Element**</span></span>|<span data-ttu-id="dd87d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dd87d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd87d-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dd87d-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="dd87d-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="dd87d-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dd87d-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dd87d-115">Parent elements</span></span>

<span data-ttu-id="dd87d-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd87d-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dd87d-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="dd87d-117">Remarks</span></span>

<span data-ttu-id="dd87d-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="dd87d-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd87d-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="dd87d-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd87d-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="dd87d-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dd87d-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dd87d-121">Schema Name</span></span>  <br/> |<span data-ttu-id="dd87d-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="dd87d-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dd87d-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dd87d-123">Validation File</span></span>  <br/> |<span data-ttu-id="dd87d-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dd87d-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dd87d-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="dd87d-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd87d-126">False</span><span class="sxs-lookup"><span data-stu-id="dd87d-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd87d-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="dd87d-127">See also</span></span>

- [<span data-ttu-id="dd87d-128">Operação DeleteItem</span><span class="sxs-lookup"><span data-stu-id="dd87d-128">DeleteItem operation</span></span>](deleteitem-operation.md)  
- [<span data-ttu-id="dd87d-129">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="dd87d-129">DeleteItem</span></span>](deleteitem.md)
- [<span data-ttu-id="dd87d-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="dd87d-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

