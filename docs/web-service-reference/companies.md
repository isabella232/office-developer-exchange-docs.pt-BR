---
title: Empresas
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Companies
api_type:
- schema
ms.assetid: 5d9ea76f-e14d-4424-8842-0c3cc3305119
description: O elemento de empresas representa a coleção de empresas que estão associados um contato ou uma tarefa.
ms.openlocfilehash: 5b8ac20d4a02017881f941d12380fe29078f51cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751400"
---
# <a name="companies"></a><span data-ttu-id="b5887-103">Empresas</span><span class="sxs-lookup"><span data-stu-id="b5887-103">Companies</span></span>

<span data-ttu-id="b5887-104">O elemento de **empresas** representa a coleção de empresas que estão associados um contato ou uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="b5887-104">The **Companies** element represents the collection of companies that are associated with a contact or task.</span></span> 
  
```xml
<Companies>
   <String/>
</Companies>
```

 <span data-ttu-id="b5887-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="b5887-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b5887-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b5887-106">Attributes and elements</span></span>

<span data-ttu-id="b5887-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b5887-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5887-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b5887-108">Attributes</span></span>

<span data-ttu-id="b5887-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b5887-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b5887-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b5887-110">Child elements</span></span>

|<span data-ttu-id="b5887-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b5887-111">**Element**</span></span>|<span data-ttu-id="b5887-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b5887-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b5887-113">String</span><span class="sxs-lookup"><span data-stu-id="b5887-113">String</span></span>](string.md) <br/> |<span data-ttu-id="b5887-114">Representa o nome de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="b5887-114">Represents the name of a company.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b5887-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b5887-115">Parent elements</span></span>

|<span data-ttu-id="b5887-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b5887-116">**Element**</span></span>|<span data-ttu-id="b5887-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b5887-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b5887-118">Contato</span><span class="sxs-lookup"><span data-stu-id="b5887-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="b5887-119">Representa um contato no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5887-119">Represents a contact in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b5887-120">Task</span><span class="sxs-lookup"><span data-stu-id="b5887-120">Task</span></span>](task.md) <br/> |<span data-ttu-id="b5887-121">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5887-121">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b5887-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="b5887-122">Remarks</span></span>

<span data-ttu-id="b5887-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="b5887-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b5887-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b5887-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b5887-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="b5887-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b5887-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b5887-126">Schema name</span></span>  <br/> |<span data-ttu-id="b5887-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b5887-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="b5887-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b5887-128">Validation file</span></span>  <br/> |<span data-ttu-id="b5887-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b5887-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b5887-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b5887-130">Can be empty</span></span>  <br/> |<span data-ttu-id="b5887-131">False</span><span class="sxs-lookup"><span data-stu-id="b5887-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b5887-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="b5887-132">See also</span></span>



- [<span data-ttu-id="b5887-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b5887-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

