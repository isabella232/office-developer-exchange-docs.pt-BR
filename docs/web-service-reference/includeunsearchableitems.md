---
title: IncludeUnsearchableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9a9bd2dc-f5b9-4b82-a6a0-f643d2951080
description: O elemento IncludeUnsearchableItems especifica se é para incluir itens que não podem ser pesquisados.
ms.openlocfilehash: 19fe450f5b1647be2df75138dbe67dd9e1c05c21
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465699"
---
# <a name="includeunsearchableitems"></a><span data-ttu-id="53e44-103">IncludeUnsearchableItems</span><span class="sxs-lookup"><span data-stu-id="53e44-103">IncludeUnsearchableItems</span></span>

<span data-ttu-id="53e44-104">O elemento **IncludeUnsearchableItems** especifica se é para incluir itens que não podem ser pesquisados.</span><span class="sxs-lookup"><span data-stu-id="53e44-104">The **IncludeUnsearchableItems** element specifies whether to include items that cannot be searched.</span></span> 
  
```XML
<IncludeUnsearchableItems>true | false</IncludeUnsearchableItems>
```

 <span data-ttu-id="53e44-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="53e44-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="53e44-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="53e44-106">Attributes and elements</span></span>

<span data-ttu-id="53e44-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="53e44-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="53e44-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="53e44-108">Attributes</span></span>

<span data-ttu-id="53e44-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="53e44-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="53e44-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="53e44-110">Child elements</span></span>

<span data-ttu-id="53e44-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="53e44-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="53e44-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="53e44-112">Parent elements</span></span>

|<span data-ttu-id="53e44-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="53e44-113">**Element**</span></span>|<span data-ttu-id="53e44-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="53e44-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="53e44-115">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="53e44-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="53e44-116">Especifica uma solicitação para pesquisar estatísticas de caixa de correio por palavra-chave.</span><span class="sxs-lookup"><span data-stu-id="53e44-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="53e44-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="53e44-117">Text value</span></span>

<span data-ttu-id="53e44-118">Um valor de texto **true** para o elemento **IncludeUnsearchableItems** indica que as estatísticas não estão incluídas para itens que não podem ser pesquisados.</span><span class="sxs-lookup"><span data-stu-id="53e44-118">A text value of **true** for the **IncludeUnsearchableItems** element indicates that statistics are not included for items that are not searchable.</span></span> <span data-ttu-id="53e44-119">Um valor **false** indica que as estatísticas são incluídas para os itens que não podem ser pesquisados.</span><span class="sxs-lookup"><span data-stu-id="53e44-119">A value of **false** indicates that statistics are included for items that are not searchable.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="53e44-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="53e44-120">Remarks</span></span>

<span data-ttu-id="53e44-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="53e44-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="53e44-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="53e44-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="53e44-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="53e44-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="53e44-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="53e44-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="53e44-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="53e44-125">Schema Name</span></span>  <br/> |<span data-ttu-id="53e44-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="53e44-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="53e44-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="53e44-127">Validation File</span></span>  <br/> |<span data-ttu-id="53e44-128">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="53e44-128">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="53e44-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="53e44-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="53e44-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="53e44-130">See also</span></span>



- [<span data-ttu-id="53e44-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="53e44-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

