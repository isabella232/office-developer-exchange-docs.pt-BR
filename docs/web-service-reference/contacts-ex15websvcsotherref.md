---
title: Contatos
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contacts
api_type:
- schema
ms.assetid: 0cc67cdf-9707-45e7-92c6-fa83a016cdbe
description: O elemento Contacts contém uma lista de contatos que estão associados a uma tarefa.
ms.openlocfilehash: c2b7bbadd494081a3e47b7b6c489218fab31d574
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458387"
---
# <a name="contacts"></a><span data-ttu-id="e22d3-103">Contatos</span><span class="sxs-lookup"><span data-stu-id="e22d3-103">Contacts</span></span>

<span data-ttu-id="e22d3-104">O elemento **Contacts** contém uma lista de contatos que estão associados a uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="e22d3-104">The **Contacts** element contains a list of contacts that are associated with a task.</span></span> 
  
```xml
<Contacts>
   <String/>
</Contacts>
```

 <span data-ttu-id="e22d3-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="e22d3-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e22d3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e22d3-106">Attributes and elements</span></span>

<span data-ttu-id="e22d3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e22d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e22d3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e22d3-108">Attributes</span></span>

<span data-ttu-id="e22d3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e22d3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e22d3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e22d3-110">Child elements</span></span>

|<span data-ttu-id="e22d3-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e22d3-111">**Element**</span></span>|<span data-ttu-id="e22d3-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e22d3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e22d3-113">String</span><span class="sxs-lookup"><span data-stu-id="e22d3-113">String</span></span>](string.md) <br/> |<span data-ttu-id="e22d3-114">Representa uma lista separada por vírgulas de nomes de contato.</span><span class="sxs-lookup"><span data-stu-id="e22d3-114">Represents a comma-separated list of contact names.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e22d3-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e22d3-115">Parent elements</span></span>

|<span data-ttu-id="e22d3-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e22d3-116">**Element**</span></span>|<span data-ttu-id="e22d3-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e22d3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e22d3-118">Tarefa</span><span class="sxs-lookup"><span data-stu-id="e22d3-118">Task</span></span>](task.md) <br/> |<span data-ttu-id="e22d3-119">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e22d3-119">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e22d3-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="e22d3-120">Remarks</span></span>

<span data-ttu-id="e22d3-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="e22d3-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e22d3-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e22d3-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e22d3-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="e22d3-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e22d3-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e22d3-124">Schema name</span></span>  <br/> |<span data-ttu-id="e22d3-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e22d3-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="e22d3-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e22d3-126">Validation file</span></span>  <br/> |<span data-ttu-id="e22d3-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e22d3-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e22d3-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e22d3-128">Can be empty</span></span>  <br/> |<span data-ttu-id="e22d3-129">False</span><span class="sxs-lookup"><span data-stu-id="e22d3-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e22d3-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="e22d3-130">See also</span></span>



- [<span data-ttu-id="e22d3-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e22d3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

