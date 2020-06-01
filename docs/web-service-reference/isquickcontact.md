---
title: IsQuickContact
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1c9542d6-ef72-4743-828a-bb671e783836
description: O elemento IsQuickContact especifica um valor Boolean que indica se o contato subjacente é um contato rápido.
ms.openlocfilehash: a8944be111a8dcbe914601ffc4e31794422d58aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44441573"
---
# <a name="isquickcontact"></a><span data-ttu-id="649f2-103">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="649f2-103">IsQuickContact</span></span>

<span data-ttu-id="649f2-104">O elemento **IsQuickContact** especifica um valor Boolean que indica se o contato subjacente é um contato rápido.</span><span class="sxs-lookup"><span data-stu-id="649f2-104">The **IsQuickContact** element specifies a Boolean value that indicates whether the underlying contact is a quick contact.</span></span> 
  
```XML
<IsQuickContact>true | false</IsQuickContact>
```

 <span data-ttu-id="649f2-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="649f2-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="649f2-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="649f2-106">Attributes and elements</span></span>

<span data-ttu-id="649f2-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="649f2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="649f2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="649f2-108">Attributes</span></span>

<span data-ttu-id="649f2-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="649f2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="649f2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="649f2-110">Child elements</span></span>

<span data-ttu-id="649f2-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="649f2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="649f2-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="649f2-112">Parent elements</span></span>

|<span data-ttu-id="649f2-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="649f2-113">**Element**</span></span>|<span data-ttu-id="649f2-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="649f2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="649f2-115">Atribuição (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="649f2-115">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="649f2-116">Especifica uma instância em uma matriz de atributos para um elemento **persona** .</span><span class="sxs-lookup"><span data-stu-id="649f2-116">Specifies an instance in an array of attributes for a **Persona** element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="649f2-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="649f2-117">Text value</span></span>

<span data-ttu-id="649f2-118">Um valor de texto **true** para o elemento **IsQuickContact** indica que o contato é um contato rápido.</span><span class="sxs-lookup"><span data-stu-id="649f2-118">A text value of **true** for the **IsQuickContact** element indicates that the contact is a quick contact.</span></span> <span data-ttu-id="649f2-119">Um valor **false** indica que o contato não é um contato rápido.</span><span class="sxs-lookup"><span data-stu-id="649f2-119">A value of **false** indicates that the contact is not a quick contact.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="649f2-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="649f2-120">Remarks</span></span>

<span data-ttu-id="649f2-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="649f2-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="649f2-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="649f2-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="649f2-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="649f2-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="649f2-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="649f2-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="649f2-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="649f2-125">Schema Name</span></span>  <br/> |<span data-ttu-id="649f2-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="649f2-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="649f2-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="649f2-127">Validation File</span></span>  <br/> |<span data-ttu-id="649f2-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="649f2-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="649f2-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="649f2-129">Can Be Empty</span></span>  <br/> |<span data-ttu-id="649f2-130">falso</span><span class="sxs-lookup"><span data-stu-id="649f2-130">false</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="649f2-131">Também consulte</span><span class="sxs-lookup"><span data-stu-id="649f2-131">See also</span></span>



- [<span data-ttu-id="649f2-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="649f2-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

