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
description: O elemento de entrada representa um endereço (IM) para um contato de mensagens instantâneas.
ms.openlocfilehash: 77de059cef470dde90ab0b929845cb260b4b867c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752093"
---
# <a name="entry-imaddress"></a><span data-ttu-id="98732-103">Entrada (IMAddress)</span><span class="sxs-lookup"><span data-stu-id="98732-103">Entry (IMAddress)</span></span>

<span data-ttu-id="98732-104">O elemento de **entrada** representa um endereço (IM) para um contato de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="98732-104">The **Entry** element represents an instant messaging (IM) address for a contact.</span></span> 
  
```xml
<Entry Key=""/>
```

 <span data-ttu-id="98732-105">**ImAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="98732-105">**ImAddressDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98732-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="98732-106">Attributes and elements</span></span>

<span data-ttu-id="98732-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="98732-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98732-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="98732-108">Attributes</span></span>

|<span data-ttu-id="98732-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="98732-109">**Attribute**</span></span>|<span data-ttu-id="98732-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="98732-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="98732-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="98732-111">**Key**</span></span> <br/> | <span data-ttu-id="98732-112">Identifica o endereço de mensagens Instantâneas.</span><span class="sxs-lookup"><span data-stu-id="98732-112">Identifies the IM address.</span></span><br/><br/><span data-ttu-id="98732-113">Estes são os valores possíveis para este atributo:</span><span class="sxs-lookup"><span data-stu-id="98732-113">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="98732-114">-ImAddress1</span><span class="sxs-lookup"><span data-stu-id="98732-114">-  ImAddress1</span></span>  <br/><span data-ttu-id="98732-115">-ImAddress2</span><span class="sxs-lookup"><span data-stu-id="98732-115">-  ImAddress2</span></span>  <br/><span data-ttu-id="98732-116">-ImAddress3</span><span class="sxs-lookup"><span data-stu-id="98732-116">-  ImAddress3</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="98732-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="98732-117">Child elements</span></span>

<span data-ttu-id="98732-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="98732-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="98732-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="98732-119">Parent elements</span></span>

|<span data-ttu-id="98732-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="98732-120">**Element**</span></span>|<span data-ttu-id="98732-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="98732-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98732-122">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="98732-122">ImAddresses</span></span>](imaddresses.md) <br/> |<span data-ttu-id="98732-123">Representa uma coleção de endereços de mensagem Instantânea para um contato.</span><span class="sxs-lookup"><span data-stu-id="98732-123">Represents a collection of IM addresses for a contact.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="98732-124">Text value</span><span class="sxs-lookup"><span data-stu-id="98732-124">Text value</span></span>

<span data-ttu-id="98732-125">Se este elemento for usado, será necessário um valor de texto que representa o endereço de mensagens Instantâneas.</span><span class="sxs-lookup"><span data-stu-id="98732-125">A text value that represents the IM address is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="98732-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="98732-126">Remarks</span></span>

<span data-ttu-id="98732-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="98732-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="98732-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="98732-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98732-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="98732-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="98732-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="98732-130">Schema name</span></span>  <br/> |<span data-ttu-id="98732-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="98732-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="98732-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="98732-132">Validation file</span></span>  <br/> |<span data-ttu-id="98732-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="98732-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="98732-134">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="98732-134">Can be empty</span></span>  <br/> |<span data-ttu-id="98732-135">False</span><span class="sxs-lookup"><span data-stu-id="98732-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="98732-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="98732-136">See also</span></span>

- [<span data-ttu-id="98732-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="98732-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="98732-138">Criação de contatos (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="98732-138">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="98732-139">Atualizar contatos</span><span class="sxs-lookup"><span data-stu-id="98732-139">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="98732-140">Excluindo contatos</span><span class="sxs-lookup"><span data-stu-id="98732-140">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

