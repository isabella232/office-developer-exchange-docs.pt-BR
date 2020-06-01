---
title: ConvertIdResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertIdResponse
api_type:
- schema
ms.assetid: ac1f044f-04a4-42ef-b762-cac5cd37894d
description: O elemento ConvertIdResponse contém uma resposta a uma solicitação convertid. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 690f0f2109dfc36dd8f359b7cef1e65beb47fc6e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452521"
---
# <a name="convertidresponse"></a><span data-ttu-id="fcbf2-104">ConvertIdResponse</span><span class="sxs-lookup"><span data-stu-id="fcbf2-104">ConvertIdResponse</span></span>

<span data-ttu-id="fcbf2-105">O elemento **ConvertIdResponse** contém uma resposta a uma solicitação convertid.</span><span class="sxs-lookup"><span data-stu-id="fcbf2-105">The **ConvertIdResponse** element contains a response to a ConvertId request.</span></span> <span data-ttu-id="fcbf2-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="fcbf2-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ConvertIdResponse>
   <ResponseMessages/>
</ConvertIdResponse>
```

 <span data-ttu-id="fcbf2-107">**ConvertIdResponseType**</span><span class="sxs-lookup"><span data-stu-id="fcbf2-107">**ConvertIdResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fcbf2-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fcbf2-108">Attributes and elements</span></span>

<span data-ttu-id="fcbf2-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fcbf2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fcbf2-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="fcbf2-110">Attributes</span></span>

<span data-ttu-id="fcbf2-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fcbf2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fcbf2-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fcbf2-112">Child elements</span></span>

|<span data-ttu-id="fcbf2-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fcbf2-113">**Element**</span></span>|<span data-ttu-id="fcbf2-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fcbf2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fcbf2-115">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fcbf2-115">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="fcbf2-116">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fcbf2-116">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fcbf2-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fcbf2-117">Parent elements</span></span>

<span data-ttu-id="fcbf2-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fcbf2-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fcbf2-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="fcbf2-119">Remarks</span></span>

<span data-ttu-id="fcbf2-120">As mensagens de resposta que estão contidas no elemento [ResponseMessages](responsemessages.md) serão instâncias de ConvertIdResponseMessageType.</span><span class="sxs-lookup"><span data-stu-id="fcbf2-120">The response messages that are contained within the [ResponseMessages](responsemessages.md) element will be instances of ConvertIdResponseMessageType.</span></span> 
  
<span data-ttu-id="fcbf2-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="fcbf2-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fcbf2-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fcbf2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fcbf2-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="fcbf2-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fcbf2-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fcbf2-124">Schema Name</span></span>  <br/> |<span data-ttu-id="fcbf2-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="fcbf2-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fcbf2-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fcbf2-126">Validation File</span></span>  <br/> |<span data-ttu-id="fcbf2-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fcbf2-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fcbf2-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fcbf2-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="fcbf2-129">False</span><span class="sxs-lookup"><span data-stu-id="fcbf2-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fcbf2-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="fcbf2-130">See also</span></span>



[<span data-ttu-id="fcbf2-131">Operação convertid</span><span class="sxs-lookup"><span data-stu-id="fcbf2-131">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="fcbf2-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fcbf2-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="fcbf2-133">Convertendo identificadores</span><span class="sxs-lookup"><span data-stu-id="fcbf2-133">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

