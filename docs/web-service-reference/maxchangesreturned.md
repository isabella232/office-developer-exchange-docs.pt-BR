---
title: MaxChangesReturned
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxChangesReturned
api_type:
- schema
ms.assetid: f471db84-a666-4dfa-9993-8ca9113a0384
description: O elemento MaxChangesReturned descreve o número máximo de alterações que pode ser retornado em uma resposta de sincronização.
ms.openlocfilehash: c3719b12b7e3e2f83a9454c7b68432b375d78614
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824395"
---
# <a name="maxchangesreturned"></a><span data-ttu-id="db0ba-103">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="db0ba-103">MaxChangesReturned</span></span>

<span data-ttu-id="db0ba-104">O elemento **MaxChangesReturned** descreve o número máximo de alterações que pode ser retornado em uma resposta de sincronização.</span><span class="sxs-lookup"><span data-stu-id="db0ba-104">The **MaxChangesReturned** element describes the maximum number of changes that can be returned in a synchronization response.</span></span> 
  
[<span data-ttu-id="db0ba-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="db0ba-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="db0ba-106">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="db0ba-106">MaxChangesReturned</span></span>](maxchangesreturned.md)
  
```xml
<MaxChangesReturned/>
```

 <span data-ttu-id="db0ba-107">**int**</span><span class="sxs-lookup"><span data-stu-id="db0ba-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db0ba-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="db0ba-108">Attributes and elements</span></span>

<span data-ttu-id="db0ba-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="db0ba-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db0ba-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="db0ba-110">Attributes</span></span>

<span data-ttu-id="db0ba-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="db0ba-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db0ba-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="db0ba-112">Child elements</span></span>

<span data-ttu-id="db0ba-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="db0ba-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="db0ba-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="db0ba-114">Parent elements</span></span>

|<span data-ttu-id="db0ba-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="db0ba-115">**Element**</span></span>|<span data-ttu-id="db0ba-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="db0ba-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db0ba-117">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="db0ba-117">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="db0ba-118">Define uma solicitação para sincronizar os itens em uma pasta de repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="db0ba-118">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="db0ba-119">Text value</span><span class="sxs-lookup"><span data-stu-id="db0ba-119">Text value</span></span>

<span data-ttu-id="db0ba-120">O valor de texto representa um número inteiro que descreve o número máximo de itens que são retornados em uma chamada única de sincronização.</span><span class="sxs-lookup"><span data-stu-id="db0ba-120">The text value represents an integer that describes the maximum number of items that are returned in a single synchronization call.</span></span> <span data-ttu-id="db0ba-121">O valor deve estar entre 1 e 512, inclusive.</span><span class="sxs-lookup"><span data-stu-id="db0ba-121">The value must be between 1 and 512, inclusive.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="db0ba-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="db0ba-122">Remarks</span></span>

<span data-ttu-id="db0ba-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="db0ba-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db0ba-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="db0ba-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db0ba-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="db0ba-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="db0ba-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="db0ba-126">Schema name</span></span>  <br/> |<span data-ttu-id="db0ba-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="db0ba-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="db0ba-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="db0ba-128">Validation file</span></span>  <br/> |<span data-ttu-id="db0ba-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="db0ba-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="db0ba-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="db0ba-130">Can be empty</span></span>  <br/> |<span data-ttu-id="db0ba-131">False</span><span class="sxs-lookup"><span data-stu-id="db0ba-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="db0ba-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="db0ba-132">See also</span></span>



[<span data-ttu-id="db0ba-133">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="db0ba-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="db0ba-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="db0ba-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

