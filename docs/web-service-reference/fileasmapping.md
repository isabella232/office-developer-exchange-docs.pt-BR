---
title: FileAsMapping
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAsMapping
api_type:
- schema
ms.assetid: 2c98e7c6-09b0-47b3-bbf7-8c4ef9510280
description: O elemento de FileAsMapping define como construir o que é exibido para um contato.
ms.openlocfilehash: 1ba0ae0daa56a72c29d8c0ccad64e3edae5f0b84
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752254"
---
# <a name="fileasmapping"></a><span data-ttu-id="63b92-103">FileAsMapping</span><span class="sxs-lookup"><span data-stu-id="63b92-103">FileAsMapping</span></span>

<span data-ttu-id="63b92-104">O elemento de **FileAsMapping** define como construir o que é exibido para um contato.</span><span class="sxs-lookup"><span data-stu-id="63b92-104">The **FileAsMapping** element defines how to construct what is displayed for a contact.</span></span> 
  
```xml
<FileAsMapping/>
```

 <span data-ttu-id="63b92-105">**FileAsMappingType**</span><span class="sxs-lookup"><span data-stu-id="63b92-105">**FileAsMappingType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="63b92-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="63b92-106">Attributes and elements</span></span>

<span data-ttu-id="63b92-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="63b92-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63b92-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="63b92-108">Attributes</span></span>

<span data-ttu-id="63b92-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="63b92-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63b92-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="63b92-110">Child elements</span></span>

<span data-ttu-id="63b92-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="63b92-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="63b92-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="63b92-112">Parent elements</span></span>

|<span data-ttu-id="63b92-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="63b92-113">**Element**</span></span>|<span data-ttu-id="63b92-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="63b92-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63b92-115">Contato</span><span class="sxs-lookup"><span data-stu-id="63b92-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="63b92-116">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="63b92-116">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="63b92-117">Text value</span><span class="sxs-lookup"><span data-stu-id="63b92-117">Text value</span></span>

<span data-ttu-id="63b92-118">O valor de texto para esse elemento é restrito a um dos valores de cadeia de caracteres a seguir:</span><span class="sxs-lookup"><span data-stu-id="63b92-118">The text value for this element is restricted to one of the following string values:</span></span>
  
- <span data-ttu-id="63b92-119">None</span><span class="sxs-lookup"><span data-stu-id="63b92-119">None</span></span>
    
- <span data-ttu-id="63b92-120">LastCommaFirst</span><span class="sxs-lookup"><span data-stu-id="63b92-120">LastCommaFirst</span></span>
    
- <span data-ttu-id="63b92-121">FirstSpaceLast</span><span class="sxs-lookup"><span data-stu-id="63b92-121">FirstSpaceLast</span></span>
    
- <span data-ttu-id="63b92-122">Empresa</span><span class="sxs-lookup"><span data-stu-id="63b92-122">Company</span></span>
    
- <span data-ttu-id="63b92-123">LastCommaFirstCompany</span><span class="sxs-lookup"><span data-stu-id="63b92-123">LastCommaFirstCompany</span></span>
    
- <span data-ttu-id="63b92-124">CompanyLastFirst</span><span class="sxs-lookup"><span data-stu-id="63b92-124">CompanyLastFirst</span></span>
    
- <span data-ttu-id="63b92-125">SobrenomeNome</span><span class="sxs-lookup"><span data-stu-id="63b92-125">LastFirst</span></span>
    
- <span data-ttu-id="63b92-126">LastFirstCompany</span><span class="sxs-lookup"><span data-stu-id="63b92-126">LastFirstCompany</span></span>
    
- <span data-ttu-id="63b92-127">CompanyLastCommaFirst</span><span class="sxs-lookup"><span data-stu-id="63b92-127">CompanyLastCommaFirst</span></span>
    
- <span data-ttu-id="63b92-128">LastFirstSuffix</span><span class="sxs-lookup"><span data-stu-id="63b92-128">LastFirstSuffix</span></span>
    
- <span data-ttu-id="63b92-129">LastSpaceFirstCompany</span><span class="sxs-lookup"><span data-stu-id="63b92-129">LastSpaceFirstCompany</span></span>
    
- <span data-ttu-id="63b92-130">CompanyLastSpaceFirst</span><span class="sxs-lookup"><span data-stu-id="63b92-130">CompanyLastSpaceFirst</span></span>
    
- <span data-ttu-id="63b92-131">LastSpaceFirst</span><span class="sxs-lookup"><span data-stu-id="63b92-131">LastSpaceFirst</span></span>
    
- <span data-ttu-id="63b92-132">DisplayName</span><span class="sxs-lookup"><span data-stu-id="63b92-132">DisplayName</span></span>
    
- <span data-ttu-id="63b92-133">FirstName</span><span class="sxs-lookup"><span data-stu-id="63b92-133">FirstName</span></span>
    
- <span data-ttu-id="63b92-134">LastFirstMiddleSuffix</span><span class="sxs-lookup"><span data-stu-id="63b92-134">LastFirstMiddleSuffix</span></span>
    
- <span data-ttu-id="63b92-135">LastName</span><span class="sxs-lookup"><span data-stu-id="63b92-135">LastName</span></span>
    
- <span data-ttu-id="63b92-136">Vazia</span><span class="sxs-lookup"><span data-stu-id="63b92-136">Empty</span></span>
    
## <a name="remarks"></a><span data-ttu-id="63b92-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="63b92-137">Remarks</span></span>

<span data-ttu-id="63b92-138">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="63b92-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63b92-139">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="63b92-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63b92-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="63b92-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="63b92-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="63b92-141">Schema name</span></span>  <br/> |<span data-ttu-id="63b92-142">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="63b92-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="63b92-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="63b92-143">Validation file</span></span>  <br/> |<span data-ttu-id="63b92-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="63b92-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="63b92-145">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="63b92-145">Can be empty</span></span>  <br/> |<span data-ttu-id="63b92-146">False</span><span class="sxs-lookup"><span data-stu-id="63b92-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63b92-147">Ver também</span><span class="sxs-lookup"><span data-stu-id="63b92-147">See also</span></span>



- [<span data-ttu-id="63b92-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="63b92-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="63b92-149">Criação de contatos (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="63b92-149">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="63b92-150">Atualizar contatos</span><span class="sxs-lookup"><span data-stu-id="63b92-150">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="63b92-151">Excluindo contatos</span><span class="sxs-lookup"><span data-stu-id="63b92-151">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

