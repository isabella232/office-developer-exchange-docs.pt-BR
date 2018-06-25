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
description: O elemento PhysicalAddresses contém uma coleção de endereços físicos que estão associados um contato.
ms.openlocfilehash: d4d5232312c735e389e9f5b0dbcb74f8614b6906
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824814"
---
# <a name="physicaladdresses"></a><span data-ttu-id="aebc2-103">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="aebc2-103">PhysicalAddresses</span></span>

<span data-ttu-id="aebc2-104">O elemento **PhysicalAddresses** contém uma coleção de endereços físicos que estão associados um contato.</span><span class="sxs-lookup"><span data-stu-id="aebc2-104">The **PhysicalAddresses** element contains a collection of physical addresses that are associated with a contact.</span></span> 
  
```xml
<PhysicalAddresses>
   <Entry/>
</PhysicalAddresses>
```

 <span data-ttu-id="aebc2-105">**PhysicalAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="aebc2-105">**PhysicalAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aebc2-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="aebc2-106">Attributes and elements</span></span>

<span data-ttu-id="aebc2-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="aebc2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aebc2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="aebc2-108">Attributes</span></span>

<span data-ttu-id="aebc2-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aebc2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aebc2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="aebc2-110">Child elements</span></span>

|<span data-ttu-id="aebc2-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aebc2-111">**Element**</span></span>|<span data-ttu-id="aebc2-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aebc2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aebc2-113">Entrada (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="aebc2-113">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md) <br/> |<span data-ttu-id="aebc2-114">Descreve um único endereço físico para um item de contato.</span><span class="sxs-lookup"><span data-stu-id="aebc2-114">Describes a single physical address for a contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aebc2-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="aebc2-115">Parent elements</span></span>

|<span data-ttu-id="aebc2-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aebc2-116">**Element**</span></span>|<span data-ttu-id="aebc2-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aebc2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aebc2-118">Contato</span><span class="sxs-lookup"><span data-stu-id="aebc2-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="aebc2-119">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="aebc2-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aebc2-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="aebc2-120">Remarks</span></span>

<span data-ttu-id="aebc2-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="aebc2-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aebc2-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="aebc2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aebc2-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="aebc2-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aebc2-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="aebc2-124">Schema name</span></span>  <br/> |<span data-ttu-id="aebc2-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="aebc2-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="aebc2-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="aebc2-126">Validation file</span></span>  <br/> |<span data-ttu-id="aebc2-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aebc2-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aebc2-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="aebc2-128">Can be empty</span></span>  <br/> |<span data-ttu-id="aebc2-129">False</span><span class="sxs-lookup"><span data-stu-id="aebc2-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aebc2-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="aebc2-130">See also</span></span>



- [<span data-ttu-id="aebc2-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="aebc2-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="aebc2-132">Criação de contatos (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="aebc2-132">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="aebc2-133">Atualizar contatos</span><span class="sxs-lookup"><span data-stu-id="aebc2-133">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="aebc2-134">Excluindo contatos</span><span class="sxs-lookup"><span data-stu-id="aebc2-134">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

