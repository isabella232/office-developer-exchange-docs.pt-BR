---
title: IncludeUnsearchableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9a9bd2dc-f5b9-4b82-a6a0-f643d2951080
description: O elemento IncludeUnsearchableItems Especifica se é necessário incluir os itens que não podem ser pesquisados.
ms.openlocfilehash: 4c6b9b3752330bf914c9901d2e8f69e93546fec6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823907"
---
# <a name="includeunsearchableitems"></a><span data-ttu-id="06ecf-103">IncludeUnsearchableItems</span><span class="sxs-lookup"><span data-stu-id="06ecf-103">IncludeUnsearchableItems</span></span>

<span data-ttu-id="06ecf-104">O elemento **IncludeUnsearchableItems** Especifica se é necessário incluir os itens que não podem ser pesquisados.</span><span class="sxs-lookup"><span data-stu-id="06ecf-104">The **IncludeUnsearchableItems** element specifies whether to include items that cannot be searched.</span></span> 
  
```XML
<IncludeUnsearchableItems>true | false</IncludeUnsearchableItems>
```

 <span data-ttu-id="06ecf-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="06ecf-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06ecf-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="06ecf-106">Attributes and elements</span></span>

<span data-ttu-id="06ecf-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="06ecf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06ecf-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="06ecf-108">Attributes</span></span>

<span data-ttu-id="06ecf-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="06ecf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06ecf-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="06ecf-110">Child elements</span></span>

<span data-ttu-id="06ecf-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="06ecf-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="06ecf-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="06ecf-112">Parent elements</span></span>

|<span data-ttu-id="06ecf-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="06ecf-113">**Element**</span></span>|<span data-ttu-id="06ecf-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="06ecf-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06ecf-115">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="06ecf-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="06ecf-116">Especifica uma solicitação para pesquisar por palavra-chave estatísticas de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="06ecf-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="06ecf-117">Text value</span><span class="sxs-lookup"><span data-stu-id="06ecf-117">Text value</span></span>

<span data-ttu-id="06ecf-118">Um valor de texto de **true** para o elemento **IncludeUnsearchableItems** indica que as estatísticas não são incluídas para itens que não são pesquisáveis.</span><span class="sxs-lookup"><span data-stu-id="06ecf-118">A text value of **true** for the **IncludeUnsearchableItems** element indicates that statistics are not included for items that are not searchable.</span></span> <span data-ttu-id="06ecf-119">Um valor **false** indica que as estatísticas estão incluídas para itens que não são pesquisáveis.</span><span class="sxs-lookup"><span data-stu-id="06ecf-119">A value of **false** indicates that statistics are included for items that are not searchable.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="06ecf-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="06ecf-120">Remarks</span></span>

<span data-ttu-id="06ecf-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="06ecf-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="06ecf-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="06ecf-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06ecf-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="06ecf-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06ecf-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="06ecf-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="06ecf-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="06ecf-125">Schema Name</span></span>  <br/> |<span data-ttu-id="06ecf-126">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="06ecf-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="06ecf-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="06ecf-127">Validation File</span></span>  <br/> |<span data-ttu-id="06ecf-128">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="06ecf-128">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="06ecf-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="06ecf-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="06ecf-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="06ecf-130">See also</span></span>



- [<span data-ttu-id="06ecf-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="06ecf-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

