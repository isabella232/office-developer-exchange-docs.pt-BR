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
ms.openlocfilehash: 60bbcfb45e52dc92140d03cdd24a251ea84217b1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465671"
---
# <a name="msexchangecertificate"></a><span data-ttu-id="38231-103">MSExchangeCertificate</span><span class="sxs-lookup"><span data-stu-id="38231-103">MSExchangeCertificate</span></span>

<span data-ttu-id="38231-104">O elemento **MSExchangeCertificate** contém um valor que codifica o certificado do Microsoft Exchange de um contato.</span><span class="sxs-lookup"><span data-stu-id="38231-104">The **MSExchangeCertificate** element contains a value that encodes the Microsoft Exchange certificate of a contact.</span></span> 
  
```XML
<MSExchangeCertificate/>
```

 <span data-ttu-id="38231-105">**ArrayOfBinaryType**</span><span class="sxs-lookup"><span data-stu-id="38231-105">**ArrayOfBinaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38231-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="38231-106">Attributes and elements</span></span>

<span data-ttu-id="38231-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="38231-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38231-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="38231-108">Attributes</span></span>

<span data-ttu-id="38231-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38231-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38231-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="38231-110">Child elements</span></span>

|<span data-ttu-id="38231-111">**Nome do elemento**</span><span class="sxs-lookup"><span data-stu-id="38231-111">**Element name**</span></span>|<span data-ttu-id="38231-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="38231-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38231-113">Base64Binary</span><span class="sxs-lookup"><span data-stu-id="38231-113">Base64Binary</span></span>](base64binary.md) <br/> |<span data-ttu-id="38231-114">Contém um valor codificado em base64.</span><span class="sxs-lookup"><span data-stu-id="38231-114">Contains a Base64-encoded value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="38231-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="38231-115">Parent elements</span></span>

|<span data-ttu-id="38231-116">**Nome do elemento**</span><span class="sxs-lookup"><span data-stu-id="38231-116">**Element name**</span></span>|<span data-ttu-id="38231-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="38231-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38231-118">Contato</span><span class="sxs-lookup"><span data-stu-id="38231-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="38231-119">Representa um item de contato no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="38231-119">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="38231-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="38231-120">Text value</span></span>

<span data-ttu-id="38231-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="38231-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="38231-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="38231-122">Remarks</span></span>

<span data-ttu-id="38231-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="38231-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="38231-124">Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="38231-124">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="38231-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="38231-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38231-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="38231-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="38231-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="38231-127">Schema name</span></span>  <br/> |<span data-ttu-id="38231-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="38231-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="38231-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="38231-129">Validation file</span></span>  <br/> |<span data-ttu-id="38231-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="38231-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="38231-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="38231-131">Can be empty</span></span>  <br/> |<span data-ttu-id="38231-132">False</span><span class="sxs-lookup"><span data-stu-id="38231-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38231-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="38231-133">See also</span></span>



- [<span data-ttu-id="38231-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="38231-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="38231-135">Criando contatos (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="38231-135">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

