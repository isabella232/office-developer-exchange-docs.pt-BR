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
description: O elemento de empresas representa a coleção de empresas que estão associadas a um contato ou a uma tarefa.
ms.openlocfilehash: eda2b92f3ca874aeeceef6a0935a49a98af0ec39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461447"
---
# <a name="companies"></a><span data-ttu-id="54d90-103">Empresas</span><span class="sxs-lookup"><span data-stu-id="54d90-103">Companies</span></span>

<span data-ttu-id="54d90-104">O elemento de **empresas** representa a coleção de empresas que estão associadas a um contato ou a uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="54d90-104">The **Companies** element represents the collection of companies that are associated with a contact or task.</span></span> 
  
```xml
<Companies>
   <String/>
</Companies>
```

 <span data-ttu-id="54d90-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="54d90-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54d90-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="54d90-106">Attributes and elements</span></span>

<span data-ttu-id="54d90-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="54d90-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54d90-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="54d90-108">Attributes</span></span>

<span data-ttu-id="54d90-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="54d90-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54d90-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="54d90-110">Child elements</span></span>

|<span data-ttu-id="54d90-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="54d90-111">**Element**</span></span>|<span data-ttu-id="54d90-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="54d90-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54d90-113">String</span><span class="sxs-lookup"><span data-stu-id="54d90-113">String</span></span>](string.md) <br/> |<span data-ttu-id="54d90-114">Representa o nome de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="54d90-114">Represents the name of a company.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54d90-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="54d90-115">Parent elements</span></span>

|<span data-ttu-id="54d90-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="54d90-116">**Element**</span></span>|<span data-ttu-id="54d90-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="54d90-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54d90-118">Contato</span><span class="sxs-lookup"><span data-stu-id="54d90-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="54d90-119">Representa um contato no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="54d90-119">Represents a contact in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="54d90-120">Tarefa</span><span class="sxs-lookup"><span data-stu-id="54d90-120">Task</span></span>](task.md) <br/> |<span data-ttu-id="54d90-121">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="54d90-121">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="54d90-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="54d90-122">Remarks</span></span>

<span data-ttu-id="54d90-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="54d90-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54d90-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="54d90-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54d90-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="54d90-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="54d90-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="54d90-126">Schema name</span></span>  <br/> |<span data-ttu-id="54d90-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="54d90-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="54d90-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="54d90-128">Validation file</span></span>  <br/> |<span data-ttu-id="54d90-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="54d90-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="54d90-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="54d90-130">Can be empty</span></span>  <br/> |<span data-ttu-id="54d90-131">False</span><span class="sxs-lookup"><span data-stu-id="54d90-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54d90-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="54d90-132">See also</span></span>



- [<span data-ttu-id="54d90-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="54d90-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

