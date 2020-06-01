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
description: O elemento MaxChangesReturned descreve o número máximo de alterações que podem ser retornadas em uma resposta de sincronização.
ms.openlocfilehash: caf96b6e95f2e63d0e544ead26fbea18cd637861
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460082"
---
# <a name="maxchangesreturned"></a><span data-ttu-id="8ed80-103">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="8ed80-103">MaxChangesReturned</span></span>

<span data-ttu-id="8ed80-104">O elemento **MaxChangesReturned** descreve o número máximo de alterações que podem ser retornadas em uma resposta de sincronização.</span><span class="sxs-lookup"><span data-stu-id="8ed80-104">The **MaxChangesReturned** element describes the maximum number of changes that can be returned in a synchronization response.</span></span> 
  
[<span data-ttu-id="8ed80-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="8ed80-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="8ed80-106">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="8ed80-106">MaxChangesReturned</span></span>](maxchangesreturned.md)
  
```xml
<MaxChangesReturned/>
```

 <span data-ttu-id="8ed80-107">**int**</span><span class="sxs-lookup"><span data-stu-id="8ed80-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8ed80-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8ed80-108">Attributes and elements</span></span>

<span data-ttu-id="8ed80-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8ed80-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ed80-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="8ed80-110">Attributes</span></span>

<span data-ttu-id="8ed80-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ed80-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ed80-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8ed80-112">Child elements</span></span>

<span data-ttu-id="8ed80-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8ed80-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8ed80-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8ed80-114">Parent elements</span></span>

|<span data-ttu-id="8ed80-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8ed80-115">**Element**</span></span>|<span data-ttu-id="8ed80-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8ed80-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ed80-117">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="8ed80-117">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="8ed80-118">Define uma solicitação para sincronizar itens em uma pasta do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8ed80-118">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8ed80-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="8ed80-119">Text value</span></span>

<span data-ttu-id="8ed80-120">O valor de texto representa um inteiro que descreve o número máximo de itens retornados em uma única chamada de sincronização.</span><span class="sxs-lookup"><span data-stu-id="8ed80-120">The text value represents an integer that describes the maximum number of items that are returned in a single synchronization call.</span></span> <span data-ttu-id="8ed80-121">O valor deve estar entre 1 e 512, inclusive.</span><span class="sxs-lookup"><span data-stu-id="8ed80-121">The value must be between 1 and 512, inclusive.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8ed80-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="8ed80-122">Remarks</span></span>

<span data-ttu-id="8ed80-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="8ed80-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8ed80-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8ed80-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ed80-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="8ed80-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8ed80-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8ed80-126">Schema name</span></span>  <br/> |<span data-ttu-id="8ed80-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8ed80-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="8ed80-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8ed80-128">Validation file</span></span>  <br/> |<span data-ttu-id="8ed80-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8ed80-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8ed80-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="8ed80-130">Can be empty</span></span>  <br/> |<span data-ttu-id="8ed80-131">False</span><span class="sxs-lookup"><span data-stu-id="8ed80-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8ed80-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="8ed80-132">See also</span></span>



[<span data-ttu-id="8ed80-133">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="8ed80-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="8ed80-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8ed80-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

