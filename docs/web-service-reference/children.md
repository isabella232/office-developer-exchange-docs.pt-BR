---
title: Children
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Children
api_type:
- schema
ms.assetid: ceaffddd-f9bc-43ea-b348-a20fdade738f
description: O elemento filho contém os nomes dos filhos de um contato.
ms.openlocfilehash: 9b1e06529fcf74850755daefc299242cfbf81f1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751388"
---
# <a name="children"></a><span data-ttu-id="7a306-103">Children</span><span class="sxs-lookup"><span data-stu-id="7a306-103">Children</span></span>

<span data-ttu-id="7a306-104">O elemento **filho** contém os nomes dos filhos de um contato.</span><span class="sxs-lookup"><span data-stu-id="7a306-104">The **Children** element contains the names of a contact's children.</span></span> 
  
```xml
<Children>
   <String/>
</Children>
```

 <span data-ttu-id="7a306-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="7a306-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a306-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7a306-106">Attributes and elements</span></span>

<span data-ttu-id="7a306-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7a306-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a306-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7a306-108">Attributes</span></span>

<span data-ttu-id="7a306-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7a306-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a306-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7a306-110">Child elements</span></span>

|<span data-ttu-id="7a306-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7a306-111">**Element**</span></span>|<span data-ttu-id="7a306-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7a306-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a306-113">String</span><span class="sxs-lookup"><span data-stu-id="7a306-113">String</span></span>](string.md) <br/> |<span data-ttu-id="7a306-114">Contém o nome do filho de um contato.</span><span class="sxs-lookup"><span data-stu-id="7a306-114">Contains the name of a contact's child.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7a306-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7a306-115">Parent elements</span></span>

|<span data-ttu-id="7a306-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7a306-116">**Element**</span></span>|<span data-ttu-id="7a306-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7a306-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a306-118">Contato</span><span class="sxs-lookup"><span data-stu-id="7a306-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="7a306-119">Representa um contato no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a306-119">Represents a contact in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7a306-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="7a306-120">Remarks</span></span>

<span data-ttu-id="7a306-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="7a306-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a306-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7a306-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a306-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="7a306-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7a306-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7a306-124">Schema name</span></span>  <br/> |<span data-ttu-id="7a306-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7a306-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="7a306-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7a306-126">Validation file</span></span>  <br/> |<span data-ttu-id="7a306-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7a306-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7a306-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="7a306-128">Can be empty</span></span>  <br/> |<span data-ttu-id="7a306-129">False</span><span class="sxs-lookup"><span data-stu-id="7a306-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a306-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="7a306-130">See also</span></span>



- [<span data-ttu-id="7a306-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7a306-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

