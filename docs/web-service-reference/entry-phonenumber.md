---
title: Entrada (PhoneNumber)
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
ms.assetid: e3d0a4d5-8af8-4607-aa2e-ef3111b63b55
description: O elemento ENTRY representa um número de telefone para um contato.
ms.openlocfilehash: 62f7091bb750dc7ca74b1e5637a437e2cdad4f1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459634"
---
# <a name="entry-phonenumber"></a><span data-ttu-id="ff1d6-103">Entrada (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="ff1d6-103">Entry (PhoneNumber)</span></span>

<span data-ttu-id="ff1d6-104">O elemento **entry** representa um número de telefone para um contato.</span><span class="sxs-lookup"><span data-stu-id="ff1d6-104">The **Entry** element represents a telephone number for a contact.</span></span> 
  
```xml
<Entry Key=""/>
```

 <span data-ttu-id="ff1d6-105">**PhoneNumberDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="ff1d6-105">**PhoneNumberDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff1d6-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ff1d6-106">Attributes and elements</span></span>

<span data-ttu-id="ff1d6-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ff1d6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff1d6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ff1d6-108">Attributes</span></span>

|<span data-ttu-id="ff1d6-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="ff1d6-109">**Attribute**</span></span>|<span data-ttu-id="ff1d6-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ff1d6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ff1d6-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="ff1d6-111">**Key**</span></span> <br/> | <span data-ttu-id="ff1d6-112">Identifica o número de telefone.</span><span class="sxs-lookup"><span data-stu-id="ff1d6-112">Identifies the telephone number.</span></span> <span data-ttu-id="ff1d6-113">O atributo chave é do tipo **PhoneNumberKeyType**.</span><span class="sxs-lookup"><span data-stu-id="ff1d6-113">The Key attribute is of type **PhoneNumberKeyType**.</span></span><br/><br/> <span data-ttu-id="ff1d6-114">Estes são os valores possíveis para este atributo:</span><span class="sxs-lookup"><span data-stu-id="ff1d6-114">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="ff1d6-115">- AssistantPhone</span><span class="sxs-lookup"><span data-stu-id="ff1d6-115">-  AssistantPhone</span></span>  <br/><span data-ttu-id="ff1d6-116">- BusinessFax</span><span class="sxs-lookup"><span data-stu-id="ff1d6-116">-  BusinessFax</span></span>  <br/><span data-ttu-id="ff1d6-117">- BusinessPhone</span><span class="sxs-lookup"><span data-stu-id="ff1d6-117">-  BusinessPhone</span></span>  <br/><span data-ttu-id="ff1d6-118">- BusinessPhone2</span><span class="sxs-lookup"><span data-stu-id="ff1d6-118">-  BusinessPhone2</span></span>  <br/><span data-ttu-id="ff1d6-119">– Retorno de chamada</span><span class="sxs-lookup"><span data-stu-id="ff1d6-119">-  Callback</span></span>  <br/><span data-ttu-id="ff1d6-120">- CarPhone</span><span class="sxs-lookup"><span data-stu-id="ff1d6-120">-  CarPhone</span></span>  <br/><span data-ttu-id="ff1d6-121">- CompanyMainPhone</span><span class="sxs-lookup"><span data-stu-id="ff1d6-121">-  CompanyMainPhone</span></span>  <br/><span data-ttu-id="ff1d6-122">- HomeFax</span><span class="sxs-lookup"><span data-stu-id="ff1d6-122">-  HomeFax</span></span>  <br/><span data-ttu-id="ff1d6-123">-HomePhone</span><span class="sxs-lookup"><span data-stu-id="ff1d6-123">-  HomePhone</span></span>  <br/><span data-ttu-id="ff1d6-124">- HomePhone2</span><span class="sxs-lookup"><span data-stu-id="ff1d6-124">-  HomePhone2</span></span>  <br/><span data-ttu-id="ff1d6-125">-ISDN</span><span class="sxs-lookup"><span data-stu-id="ff1d6-125">-  Isdn</span></span>  <br/><span data-ttu-id="ff1d6-126">-MobilePhone</span><span class="sxs-lookup"><span data-stu-id="ff1d6-126">-  MobilePhone</span></span>  <br/><span data-ttu-id="ff1d6-127">-OtherFax</span><span class="sxs-lookup"><span data-stu-id="ff1d6-127">-  OtherFax</span></span>  <br/><span data-ttu-id="ff1d6-128">-OtherTelephone</span><span class="sxs-lookup"><span data-stu-id="ff1d6-128">-  OtherTelephone</span></span>  <br/><span data-ttu-id="ff1d6-129">-Pager</span><span class="sxs-lookup"><span data-stu-id="ff1d6-129">-  Pager</span></span>  <br/><span data-ttu-id="ff1d6-130">- PrimaryPhone</span><span class="sxs-lookup"><span data-stu-id="ff1d6-130">-  PrimaryPhone</span></span>  <br/><span data-ttu-id="ff1d6-131">- RadioPhone</span><span class="sxs-lookup"><span data-stu-id="ff1d6-131">-  RadioPhone</span></span>  <br/><span data-ttu-id="ff1d6-132">-Telex</span><span class="sxs-lookup"><span data-stu-id="ff1d6-132">-  Telex</span></span>  <br/><span data-ttu-id="ff1d6-133">- TtyTddPhone</span><span class="sxs-lookup"><span data-stu-id="ff1d6-133">-  TtyTddPhone</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ff1d6-134">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ff1d6-134">Child elements</span></span>

<span data-ttu-id="ff1d6-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ff1d6-135">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ff1d6-136">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ff1d6-136">Parent elements</span></span>

|<span data-ttu-id="ff1d6-137">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ff1d6-137">**Element**</span></span>|<span data-ttu-id="ff1d6-138">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ff1d6-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff1d6-139">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="ff1d6-139">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="ff1d6-140">Representa uma coleção de números de telefone de um contato.</span><span class="sxs-lookup"><span data-stu-id="ff1d6-140">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ff1d6-141">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ff1d6-141">Text value</span></span>

<span data-ttu-id="ff1d6-142">Um valor de texto que representa um número de telefone será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="ff1d6-142">A text value that represents a telephone number is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ff1d6-143">Comentários</span><span class="sxs-lookup"><span data-stu-id="ff1d6-143">Remarks</span></span>

<span data-ttu-id="ff1d6-144">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="ff1d6-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff1d6-145">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ff1d6-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff1d6-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="ff1d6-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ff1d6-147">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ff1d6-147">Schema name</span></span>  <br/> |<span data-ttu-id="ff1d6-148">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ff1d6-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="ff1d6-149">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ff1d6-149">Validation file</span></span>  <br/> |<span data-ttu-id="ff1d6-150">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ff1d6-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ff1d6-151">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ff1d6-151">Can be empty</span></span>  <br/> |<span data-ttu-id="ff1d6-152">False</span><span class="sxs-lookup"><span data-stu-id="ff1d6-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff1d6-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="ff1d6-153">See also</span></span>

- [<span data-ttu-id="ff1d6-154">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ff1d6-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="ff1d6-155">Criando contatos (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="ff1d6-155">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [<span data-ttu-id="ff1d6-156">Atualizando contatos</span><span class="sxs-lookup"><span data-stu-id="ff1d6-156">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="ff1d6-157">Excluindo contatos</span><span class="sxs-lookup"><span data-stu-id="ff1d6-157">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

