---
title: FilterHtmlContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FilterHtmlContent
api_type:
- schema
ms.assetid: 2f9358a0-de1d-4544-9aa0-d9f6519f3b5f
description: O elemento FilterHtmlContent especifica se o conteúdo HTML potencialmente não seguro é filtrado de um item ou anexo.
ms.openlocfilehash: 28e3be86b550c3f330fbb6846b64732b5674304d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462672"
---
# <a name="filterhtmlcontent"></a><span data-ttu-id="bec78-103">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="bec78-103">FilterHtmlContent</span></span>

<span data-ttu-id="bec78-104">O elemento **FilterHtmlContent** especifica se o conteúdo HTML potencialmente não seguro é filtrado de um item ou anexo.</span><span class="sxs-lookup"><span data-stu-id="bec78-104">The **FilterHtmlContent** element specifies whether potentially unsafe HTML content is filtered from an item or attachment.</span></span> 
  
```xml
<FilterHtmlContent>true or false</FilterHtmlContent>
```

 <span data-ttu-id="bec78-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="bec78-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bec78-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="bec78-106">Attributes and elements</span></span>

<span data-ttu-id="bec78-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bec78-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bec78-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="bec78-108">Attributes</span></span>

<span data-ttu-id="bec78-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bec78-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bec78-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bec78-110">Child elements</span></span>

<span data-ttu-id="bec78-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bec78-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bec78-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bec78-112">Parent elements</span></span>

|<span data-ttu-id="bec78-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bec78-113">**Element**</span></span>|<span data-ttu-id="bec78-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bec78-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bec78-115">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="bec78-115">AttachmentShape</span></span>](attachmentshape.md) <br/> | <span data-ttu-id="bec78-116">Identifica propriedades adicionais para retornar em uma resposta a uma solicitação [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="bec78-116">Identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/><br/>  <span data-ttu-id="bec78-117">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="bec78-117">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/GetAttachment/AttachmentShape` <br/> |
|[<span data-ttu-id="bec78-118">Shape</span><span class="sxs-lookup"><span data-stu-id="bec78-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="bec78-119">Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="bec78-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> <br/> <span data-ttu-id="bec78-120">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="bec78-120">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetItem/ItemShape`<br/> <br/>  `/FindItem/ItemShape`<br/> <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bec78-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="bec78-121">Text value</span></span>

<span data-ttu-id="bec78-122">Esse elemento pode ser **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="bec78-122">This element can be either **true** or **false**.</span></span> <span data-ttu-id="bec78-123">O valor padrão é **false**.</span><span class="sxs-lookup"><span data-stu-id="bec78-123">The default value is **false**.</span></span> <span data-ttu-id="bec78-124">Este é um tipo de dados Boolean.</span><span class="sxs-lookup"><span data-stu-id="bec78-124">This is a Boolean data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bec78-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="bec78-125">Remarks</span></span>

<span data-ttu-id="bec78-126">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="bec78-126">This element is optional.</span></span>
  
<span data-ttu-id="bec78-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange Server com a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="bec78-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bec78-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="bec78-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bec78-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="bec78-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bec78-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bec78-130">Schema Name</span></span>  <br/> |<span data-ttu-id="bec78-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="bec78-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="bec78-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bec78-132">Validation File</span></span>  <br/> |<span data-ttu-id="bec78-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bec78-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bec78-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="bec78-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="bec78-135">False</span><span class="sxs-lookup"><span data-stu-id="bec78-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bec78-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="bec78-136">See also</span></span>

- [<span data-ttu-id="bec78-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bec78-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

