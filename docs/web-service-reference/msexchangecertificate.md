---
title: MSExchangeCertificate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c514f22f-be3e-4cad-ac56-bdff6bafcee6
description: O elemento MSExchangeCertificate contém um valor que codifica o certificado do Microsoft Exchange de um contato.
ms.openlocfilehash: 8d07198012485b5c6d22e1fb4721890bf9a5eb39
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824498"
---
# <a name="msexchangecertificate"></a><span data-ttu-id="0fcbf-103">MSExchangeCertificate</span><span class="sxs-lookup"><span data-stu-id="0fcbf-103">MSExchangeCertificate</span></span>

<span data-ttu-id="0fcbf-104">O elemento **MSExchangeCertificate** contém um valor que codifica o certificado do Microsoft Exchange de um contato.</span><span class="sxs-lookup"><span data-stu-id="0fcbf-104">The **MSExchangeCertificate** element contains a value that encodes the Microsoft Exchange certificate of a contact.</span></span> 
  
```XML
<MSExchangeCertificate/>
```

 <span data-ttu-id="0fcbf-105">**ArrayOfBinaryType**</span><span class="sxs-lookup"><span data-stu-id="0fcbf-105">**ArrayOfBinaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0fcbf-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0fcbf-106">Attributes and elements</span></span>

<span data-ttu-id="0fcbf-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0fcbf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0fcbf-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0fcbf-108">Attributes</span></span>

<span data-ttu-id="0fcbf-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0fcbf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0fcbf-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0fcbf-110">Child elements</span></span>

|<span data-ttu-id="0fcbf-111">**Nome do elemento**</span><span class="sxs-lookup"><span data-stu-id="0fcbf-111">**Element name**</span></span>|<span data-ttu-id="0fcbf-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0fcbf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fcbf-113">Base64Binary</span><span class="sxs-lookup"><span data-stu-id="0fcbf-113">Base64Binary</span></span>](base64binary.md) <br/> |<span data-ttu-id="0fcbf-114">Contém um valor codificado na Base64.</span><span class="sxs-lookup"><span data-stu-id="0fcbf-114">Contains a Base64-encoded value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0fcbf-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0fcbf-115">Parent elements</span></span>

|<span data-ttu-id="0fcbf-116">**Nome do elemento**</span><span class="sxs-lookup"><span data-stu-id="0fcbf-116">**Element name**</span></span>|<span data-ttu-id="0fcbf-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0fcbf-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fcbf-118">Contato</span><span class="sxs-lookup"><span data-stu-id="0fcbf-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="0fcbf-119">Representa um item de contato no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0fcbf-119">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0fcbf-120">Text value</span><span class="sxs-lookup"><span data-stu-id="0fcbf-120">Text value</span></span>

<span data-ttu-id="0fcbf-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0fcbf-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0fcbf-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="0fcbf-122">Remarks</span></span>

<span data-ttu-id="0fcbf-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0fcbf-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="0fcbf-124">Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="0fcbf-124">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0fcbf-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0fcbf-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0fcbf-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="0fcbf-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0fcbf-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0fcbf-127">Schema name</span></span>  <br/> |<span data-ttu-id="0fcbf-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0fcbf-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="0fcbf-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0fcbf-129">Validation file</span></span>  <br/> |<span data-ttu-id="0fcbf-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0fcbf-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0fcbf-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0fcbf-131">Can be empty</span></span>  <br/> |<span data-ttu-id="0fcbf-132">False</span><span class="sxs-lookup"><span data-stu-id="0fcbf-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0fcbf-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="0fcbf-133">See also</span></span>



- [<span data-ttu-id="0fcbf-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0fcbf-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="0fcbf-135">Criação de contatos (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="0fcbf-135">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

