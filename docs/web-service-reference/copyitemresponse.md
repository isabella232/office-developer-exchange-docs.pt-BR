---
title: CopyItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItemResponse
api_type:
- schema
ms.assetid: ae402bc1-4589-45e0-a929-f368c916a7e4
description: O elemento de CopyItemResponse define uma resposta a uma solicitação de CopyItem.
ms.openlocfilehash: b460a3f5a176e0cee03443ceff62742602e8df03
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751553"
---
# <a name="copyitemresponse"></a><span data-ttu-id="0cdc8-103">CopyItemResponse</span><span class="sxs-lookup"><span data-stu-id="0cdc8-103">CopyItemResponse</span></span>

<span data-ttu-id="0cdc8-104">O elemento de **CopyItemResponse** define uma resposta a uma solicitação de CopyItem.</span><span class="sxs-lookup"><span data-stu-id="0cdc8-104">The **CopyItemResponse** element defines a response to a CopyItem request.</span></span> 
  
```xml
<CopyItemResponse>
   <ResponseMessages/>
</CopyItemResponse>
```

 <span data-ttu-id="0cdc8-105">**CopyItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="0cdc8-105">**CopyItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0cdc8-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0cdc8-106">Attributes and elements</span></span>

<span data-ttu-id="0cdc8-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0cdc8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0cdc8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0cdc8-108">Attributes</span></span>

<span data-ttu-id="0cdc8-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0cdc8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0cdc8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0cdc8-110">Child elements</span></span>

|<span data-ttu-id="0cdc8-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0cdc8-111">**Element**</span></span>|<span data-ttu-id="0cdc8-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0cdc8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0cdc8-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0cdc8-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0cdc8-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0cdc8-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0cdc8-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0cdc8-115">Parent elements</span></span>

<span data-ttu-id="0cdc8-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0cdc8-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0cdc8-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="0cdc8-117">Remarks</span></span>

<span data-ttu-id="0cdc8-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="0cdc8-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0cdc8-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0cdc8-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0cdc8-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="0cdc8-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0cdc8-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0cdc8-121">Schema name</span></span>  <br/> |<span data-ttu-id="0cdc8-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0cdc8-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0cdc8-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0cdc8-123">Validation file</span></span>  <br/> |<span data-ttu-id="0cdc8-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0cdc8-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0cdc8-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0cdc8-125">Can be empty</span></span>  <br/> |<span data-ttu-id="0cdc8-126">False</span><span class="sxs-lookup"><span data-stu-id="0cdc8-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0cdc8-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="0cdc8-127">See also</span></span>



[<span data-ttu-id="0cdc8-128">Operação CopyItem</span><span class="sxs-lookup"><span data-stu-id="0cdc8-128">CopyItem operation</span></span>](copyitem-operation.md)
  
[<span data-ttu-id="0cdc8-129">CopyItem</span><span class="sxs-lookup"><span data-stu-id="0cdc8-129">CopyItem</span></span>](copyitem.md)


- [<span data-ttu-id="0cdc8-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0cdc8-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

