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
description: O elemento FilterHtmlContent Especifica se o conteúdo potencialmente não seguro de HTML é filtrado de um item ou de um anexo.
ms.openlocfilehash: db181eff9586061d728a5e4ef55a78f4955b5713
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752253"
---
# <a name="filterhtmlcontent"></a><span data-ttu-id="69ac9-103">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="69ac9-103">FilterHtmlContent</span></span>

<span data-ttu-id="69ac9-104">O elemento **FilterHtmlContent** Especifica se o conteúdo potencialmente não seguro de HTML é filtrado de um item ou de um anexo.</span><span class="sxs-lookup"><span data-stu-id="69ac9-104">The **FilterHtmlContent** element specifies whether potentially unsafe HTML content is filtered from an item or attachment.</span></span> 
  
```xml
<FilterHtmlContent>true or false</FilterHtmlContent>
```

 <span data-ttu-id="69ac9-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="69ac9-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="69ac9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="69ac9-106">Attributes and elements</span></span>

<span data-ttu-id="69ac9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="69ac9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69ac9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="69ac9-108">Attributes</span></span>

<span data-ttu-id="69ac9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="69ac9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69ac9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="69ac9-110">Child elements</span></span>

<span data-ttu-id="69ac9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="69ac9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="69ac9-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="69ac9-112">Parent elements</span></span>

|<span data-ttu-id="69ac9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="69ac9-113">**Element**</span></span>|<span data-ttu-id="69ac9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="69ac9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69ac9-115">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="69ac9-115">AttachmentShape</span></span>](attachmentshape.md) <br/> | <span data-ttu-id="69ac9-116">Identifica as propriedades adicionais para retornar em resposta a uma solicitação de [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="69ac9-116">Identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/><br/>  <span data-ttu-id="69ac9-117">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="69ac9-117">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/GetAttachment/AttachmentShape` <br/> |
|[<span data-ttu-id="69ac9-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="69ac9-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="69ac9-119">Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="69ac9-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> <br/> <span data-ttu-id="69ac9-120">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="69ac9-120">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetItem/ItemShape`<br/> <br/>  `/FindItem/ItemShape`<br/> <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="69ac9-121">Text value</span><span class="sxs-lookup"><span data-stu-id="69ac9-121">Text value</span></span>

<span data-ttu-id="69ac9-122">Esse elemento pode ser **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="69ac9-122">This element can be either **true** or **false**.</span></span> <span data-ttu-id="69ac9-123">O valor padrão é **false**.</span><span class="sxs-lookup"><span data-stu-id="69ac9-123">The default value is **false**.</span></span> <span data-ttu-id="69ac9-124">Este é um tipo de dados Boolean.</span><span class="sxs-lookup"><span data-stu-id="69ac9-124">This is a Boolean data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="69ac9-125">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="69ac9-125">Remarks</span></span>

<span data-ttu-id="69ac9-126">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="69ac9-126">This element is optional.</span></span>
  
<span data-ttu-id="69ac9-127">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server com a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="69ac9-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69ac9-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="69ac9-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69ac9-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="69ac9-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="69ac9-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="69ac9-130">Schema Name</span></span>  <br/> |<span data-ttu-id="69ac9-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="69ac9-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="69ac9-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="69ac9-132">Validation File</span></span>  <br/> |<span data-ttu-id="69ac9-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="69ac9-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="69ac9-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="69ac9-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="69ac9-135">False</span><span class="sxs-lookup"><span data-stu-id="69ac9-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69ac9-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="69ac9-136">See also</span></span>

- [<span data-ttu-id="69ac9-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="69ac9-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

