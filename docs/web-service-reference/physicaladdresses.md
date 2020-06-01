---
title: PhysicalAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhysicalAddresses
api_type:
- schema
ms.assetid: 5276c5f2-9e08-43af-a0b2-da4ff1dcae2d
description: O elemento PhysicalAddresses contém uma coleção de endereços físicos associados a um contato.
ms.openlocfilehash: b609abed481359fa6562f41a551645eb613ddfa0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468877"
---
# <a name="physicaladdresses"></a><span data-ttu-id="95355-103">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="95355-103">PhysicalAddresses</span></span>

<span data-ttu-id="95355-104">O elemento **PhysicalAddresses** contém uma coleção de endereços físicos associados a um contato.</span><span class="sxs-lookup"><span data-stu-id="95355-104">The **PhysicalAddresses** element contains a collection of physical addresses that are associated with a contact.</span></span> 
  
```xml
<PhysicalAddresses>
   <Entry/>
</PhysicalAddresses>
```

 <span data-ttu-id="95355-105">**PhysicalAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="95355-105">**PhysicalAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95355-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="95355-106">Attributes and elements</span></span>

<span data-ttu-id="95355-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="95355-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95355-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="95355-108">Attributes</span></span>

<span data-ttu-id="95355-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="95355-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95355-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="95355-110">Child elements</span></span>

|<span data-ttu-id="95355-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="95355-111">**Element**</span></span>|<span data-ttu-id="95355-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="95355-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95355-113">Entrada (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="95355-113">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md) <br/> |<span data-ttu-id="95355-114">Descreve um único endereço físico para um item de contato.</span><span class="sxs-lookup"><span data-stu-id="95355-114">Describes a single physical address for a contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="95355-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="95355-115">Parent elements</span></span>

|<span data-ttu-id="95355-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="95355-116">**Element**</span></span>|<span data-ttu-id="95355-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="95355-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95355-118">Contato</span><span class="sxs-lookup"><span data-stu-id="95355-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="95355-119">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="95355-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="95355-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="95355-120">Remarks</span></span>

<span data-ttu-id="95355-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="95355-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95355-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="95355-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95355-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="95355-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="95355-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="95355-124">Schema name</span></span>  <br/> |<span data-ttu-id="95355-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="95355-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="95355-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="95355-126">Validation file</span></span>  <br/> |<span data-ttu-id="95355-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="95355-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="95355-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="95355-128">Can be empty</span></span>  <br/> |<span data-ttu-id="95355-129">False</span><span class="sxs-lookup"><span data-stu-id="95355-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="95355-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="95355-130">See also</span></span>



- [<span data-ttu-id="95355-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="95355-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="95355-132">Criando contatos (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="95355-132">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="95355-133">Atualizando contatos</span><span class="sxs-lookup"><span data-stu-id="95355-133">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="95355-134">Excluindo contatos</span><span class="sxs-lookup"><span data-stu-id="95355-134">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

