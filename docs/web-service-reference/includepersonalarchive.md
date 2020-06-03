---
title: IncludePersonalArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b373bb1a-6b1d-4959-98a1-4c4ea62973bc
description: O elemento IncludePersonalArchive especifica se é para incluir o arquivo morto pessoal na pesquisa.
ms.openlocfilehash: a25dd45bc0717af8f949d14b88793af3821ca69f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458247"
---
# <a name="includepersonalarchive"></a><span data-ttu-id="907b1-103">IncludePersonalArchive</span><span class="sxs-lookup"><span data-stu-id="907b1-103">IncludePersonalArchive</span></span>

<span data-ttu-id="907b1-104">O elemento **IncludePersonalArchive** especifica se é para incluir o arquivo morto pessoal na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="907b1-104">The **IncludePersonalArchive** element specifies whether to include the personal archive in the search.</span></span> 
  
```XML
<IncludePersonalArchive>true | false</IncludePersonalArchive>
```

 <span data-ttu-id="907b1-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="907b1-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="907b1-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="907b1-106">Attributes and elements</span></span>

<span data-ttu-id="907b1-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="907b1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="907b1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="907b1-108">Attributes</span></span>

<span data-ttu-id="907b1-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="907b1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="907b1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="907b1-110">Child elements</span></span>

<span data-ttu-id="907b1-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="907b1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="907b1-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="907b1-112">Parent elements</span></span>

|<span data-ttu-id="907b1-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="907b1-113">**Element**</span></span>|<span data-ttu-id="907b1-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="907b1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="907b1-115">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="907b1-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="907b1-116">Especifica uma solicitação para pesquisar estatísticas de caixa de correio por palavra-chave.</span><span class="sxs-lookup"><span data-stu-id="907b1-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="907b1-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="907b1-117">Text value</span></span>

<span data-ttu-id="907b1-118">Um valor de texto **true** para o elemento **IncludePersonalArchive** indica que o arquivo morto pessoal está incluído na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="907b1-118">A text value of **true** for the **IncludePersonalArchive** element indicates that the personal archive is included in the search.</span></span> <span data-ttu-id="907b1-119">Um valor **false** indica que o arquivo morto pessoal não está incluído na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="907b1-119">A value of **false** indicates that the personal archive is not included in the search.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="907b1-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="907b1-120">Remarks</span></span>

<span data-ttu-id="907b1-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="907b1-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="907b1-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="907b1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="907b1-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="907b1-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="907b1-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="907b1-124">Schema Name</span></span>  <br/> |<span data-ttu-id="907b1-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="907b1-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="907b1-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="907b1-126">Validation File</span></span>  <br/> |<span data-ttu-id="907b1-127">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="907b1-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="907b1-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="907b1-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="907b1-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="907b1-129">See also</span></span>



- [<span data-ttu-id="907b1-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="907b1-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

