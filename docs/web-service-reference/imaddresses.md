---
title: Imendereços
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ImAddresses
api_type:
- schema
ms.assetid: 29f614a7-7fe6-47fa-b5f2-8feff106aa99
description: O elemento ImAddresses representa uma coleção de endereços de mensagens instantâneas para um contato.
ms.openlocfilehash: 24ff74d29c918d71116e25e097878b6e4e0a8ead
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460425"
---
# <a name="imaddresses"></a><span data-ttu-id="51007-103">Imendereços</span><span class="sxs-lookup"><span data-stu-id="51007-103">ImAddresses</span></span>

<span data-ttu-id="51007-104">O elemento **ImAddresses** representa uma coleção de endereços de mensagens instantâneas para um contato.</span><span class="sxs-lookup"><span data-stu-id="51007-104">The **ImAddresses** element represents a collection of instant messaging addresses for a contact.</span></span> 
  
```xml
<ImAddresses>
   <Entry/>
</ImAddresses>
```

 <span data-ttu-id="51007-105">**ImAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="51007-105">**ImAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="51007-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="51007-106">Attributes and elements</span></span>

<span data-ttu-id="51007-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="51007-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="51007-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="51007-108">Attributes</span></span>

<span data-ttu-id="51007-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="51007-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="51007-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="51007-110">Child elements</span></span>

|<span data-ttu-id="51007-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="51007-111">**Element**</span></span>|<span data-ttu-id="51007-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="51007-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51007-113">Entrada (IMAddress)</span><span class="sxs-lookup"><span data-stu-id="51007-113">Entry (IMAddress)</span></span>](entry-imaddress.md) <br/> |<span data-ttu-id="51007-114">Representa um endereço de mensagens instantâneas para um contato.</span><span class="sxs-lookup"><span data-stu-id="51007-114">Represents an instant messaging address for a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="51007-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="51007-115">Parent elements</span></span>

|<span data-ttu-id="51007-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="51007-116">**Element**</span></span>|<span data-ttu-id="51007-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="51007-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51007-118">Contato</span><span class="sxs-lookup"><span data-stu-id="51007-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="51007-119">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="51007-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="51007-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="51007-120">Remarks</span></span>

<span data-ttu-id="51007-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="51007-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="51007-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="51007-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="51007-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="51007-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="51007-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="51007-124">Schema name</span></span>  <br/> |<span data-ttu-id="51007-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="51007-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="51007-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="51007-126">Validation file</span></span>  <br/> |<span data-ttu-id="51007-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="51007-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="51007-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="51007-128">Can be empty</span></span>  <br/> |<span data-ttu-id="51007-129">False</span><span class="sxs-lookup"><span data-stu-id="51007-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="51007-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="51007-130">See also</span></span>



- [<span data-ttu-id="51007-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="51007-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

