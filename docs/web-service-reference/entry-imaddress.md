---
title: Entrada (IMAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: ee444170-7353-4e86-86c6-d7300a2f1777
description: O elemento ENTRY representa um endereço de mensagens instantâneas (IM) para um contato.
ms.openlocfilehash: b6cc37447eb0f231e9e852a6c3cd64d6e1f3a89f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460698"
---
# <a name="entry-imaddress"></a><span data-ttu-id="fe8ff-103">Entrada (IMAddress)</span><span class="sxs-lookup"><span data-stu-id="fe8ff-103">Entry (IMAddress)</span></span>

<span data-ttu-id="fe8ff-104">O elemento **entry** representa um endereço de mensagens instantâneas (IM) para um contato.</span><span class="sxs-lookup"><span data-stu-id="fe8ff-104">The **Entry** element represents an instant messaging (IM) address for a contact.</span></span> 
  
```xml
<Entry Key=""/>
```

 <span data-ttu-id="fe8ff-105">**ImAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="fe8ff-105">**ImAddressDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fe8ff-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fe8ff-106">Attributes and elements</span></span>

<span data-ttu-id="fe8ff-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fe8ff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fe8ff-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fe8ff-108">Attributes</span></span>

|<span data-ttu-id="fe8ff-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="fe8ff-109">**Attribute**</span></span>|<span data-ttu-id="fe8ff-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fe8ff-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fe8ff-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="fe8ff-111">**Key**</span></span> <br/> | <span data-ttu-id="fe8ff-112">Identifica o endereço de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="fe8ff-112">Identifies the IM address.</span></span><br/><br/><span data-ttu-id="fe8ff-113">Estes são os valores possíveis para este atributo:</span><span class="sxs-lookup"><span data-stu-id="fe8ff-113">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="fe8ff-114">- ImAddress1</span><span class="sxs-lookup"><span data-stu-id="fe8ff-114">-  ImAddress1</span></span>  <br/><span data-ttu-id="fe8ff-115">- ImAddress2</span><span class="sxs-lookup"><span data-stu-id="fe8ff-115">-  ImAddress2</span></span>  <br/><span data-ttu-id="fe8ff-116">- ImAddress3</span><span class="sxs-lookup"><span data-stu-id="fe8ff-116">-  ImAddress3</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fe8ff-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fe8ff-117">Child elements</span></span>

<span data-ttu-id="fe8ff-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fe8ff-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fe8ff-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fe8ff-119">Parent elements</span></span>

|<span data-ttu-id="fe8ff-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fe8ff-120">**Element**</span></span>|<span data-ttu-id="fe8ff-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fe8ff-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe8ff-122">Imendereços</span><span class="sxs-lookup"><span data-stu-id="fe8ff-122">ImAddresses</span></span>](imaddresses.md) <br/> |<span data-ttu-id="fe8ff-123">Representa uma coleção de endereços de mensagens instantâneas de um contato.</span><span class="sxs-lookup"><span data-stu-id="fe8ff-123">Represents a collection of IM addresses for a contact.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fe8ff-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="fe8ff-124">Text value</span></span>

<span data-ttu-id="fe8ff-125">Um valor de texto que representa o endereço de IM será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="fe8ff-125">A text value that represents the IM address is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fe8ff-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="fe8ff-126">Remarks</span></span>

<span data-ttu-id="fe8ff-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="fe8ff-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fe8ff-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fe8ff-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fe8ff-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="fe8ff-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fe8ff-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fe8ff-130">Schema name</span></span>  <br/> |<span data-ttu-id="fe8ff-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="fe8ff-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="fe8ff-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fe8ff-132">Validation file</span></span>  <br/> |<span data-ttu-id="fe8ff-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fe8ff-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fe8ff-134">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="fe8ff-134">Can be empty</span></span>  <br/> |<span data-ttu-id="fe8ff-135">False</span><span class="sxs-lookup"><span data-stu-id="fe8ff-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fe8ff-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="fe8ff-136">See also</span></span>

- [<span data-ttu-id="fe8ff-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fe8ff-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="fe8ff-138">Criando contatos (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="fe8ff-138">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="fe8ff-139">Atualizando contatos</span><span class="sxs-lookup"><span data-stu-id="fe8ff-139">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="fe8ff-140">Excluindo contatos</span><span class="sxs-lookup"><span data-stu-id="fe8ff-140">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

