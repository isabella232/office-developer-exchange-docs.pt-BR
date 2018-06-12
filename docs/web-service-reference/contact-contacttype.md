---
title: Contato (ContactType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f7119b7-f5b4-484d-a7de-fa74836d9aee
description: O elemento de contato Especifica um contato no repositório unificado de contatos.
ms.openlocfilehash: f1593da78a46851c7db43abc567eb66c0c74e0f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751436"
---
# <a name="contact-contacttype"></a><span data-ttu-id="2b139-103">Contato (ContactType)</span><span class="sxs-lookup"><span data-stu-id="2b139-103">Contact (ContactType)</span></span>

<span data-ttu-id="2b139-104">O elemento **Contatos** Especifica um contato no repositório unificado de contatos.</span><span class="sxs-lookup"><span data-stu-id="2b139-104">The **Contact** element specifies a contact in the Unified Contact Store.</span></span> 
  
```XML
<Contact>
    <PersonName></PersonName>
    <BusinessName></BusinessName>
    <PhoneNumbers></PhoneNumbers>
    <Urls></Urls>
    <EmailAddresses></EmailAddresses>
    <Addresses></Addesses>    <ContactString></ContactString
</Contact>
```

 <span data-ttu-id="2b139-105">**ContactType**</span><span class="sxs-lookup"><span data-stu-id="2b139-105">**ContactType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b139-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2b139-106">Attributes and elements</span></span>

<span data-ttu-id="2b139-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2b139-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b139-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2b139-108">Attributes</span></span>

<span data-ttu-id="2b139-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2b139-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b139-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2b139-110">Child elements</span></span>

|<span data-ttu-id="2b139-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2b139-111">**Element**</span></span>|<span data-ttu-id="2b139-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2b139-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b139-113">PersonName</span><span class="sxs-lookup"><span data-stu-id="2b139-113">PersonName</span></span>](personname.md) <br/> |<span data-ttu-id="2b139-114">Especifica o nome de um indivíduo.</span><span class="sxs-lookup"><span data-stu-id="2b139-114">Specifies the name of an individual.</span></span>  <br/> |
|[<span data-ttu-id="2b139-115">BusinessName</span><span class="sxs-lookup"><span data-stu-id="2b139-115">BusinessName</span></span>](businessname.md) <br/> |<span data-ttu-id="2b139-116">Especifica o nome de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="2b139-116">Specifies the name of a business.</span></span>  <br/> |
|[<span data-ttu-id="2b139-117">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="2b139-117">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="2b139-118">Representa uma coleção de números de telefone de um contato.</span><span class="sxs-lookup"><span data-stu-id="2b139-118">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
|[<span data-ttu-id="2b139-119">URLs</span><span class="sxs-lookup"><span data-stu-id="2b139-119">Urls</span></span>](urls.md) <br/> |<span data-ttu-id="2b139-120">Especifica uma matriz de URLs para uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="2b139-120">Specifies an array of URLs for a persona.</span></span>  <br/> |
|[<span data-ttu-id="2b139-121">EmailAddresses (ArrayOfExtractedEmailAddresses)</span><span class="sxs-lookup"><span data-stu-id="2b139-121">EmailAddresses (ArrayOfExtractedEmailAddresses)</span></span>](emailaddresses-arrayofextractedemailaddresses.md) <br/> |<span data-ttu-id="2b139-122">Especifica uma matriz de endereços de email extraídos.</span><span class="sxs-lookup"><span data-stu-id="2b139-122">Specifies an array of extracted email addresses.</span></span>  <br/> |
|[<span data-ttu-id="2b139-123">Endereços (ArrayOfAddressesType)</span><span class="sxs-lookup"><span data-stu-id="2b139-123">Addresses (ArrayOfAddressesType)</span></span>](addresses-arrayofaddressestype.md) <br/> |<span data-ttu-id="2b139-124">Especifica uma matriz de elementos de **endereço** .</span><span class="sxs-lookup"><span data-stu-id="2b139-124">Specifies an array of **Address** elements.</span></span>  <br/> |
|[<span data-ttu-id="2b139-125">ContactString</span><span class="sxs-lookup"><span data-stu-id="2b139-125">ContactString</span></span>](contactstring.md) <br/> |<span data-ttu-id="2b139-126">Especifica o nome de exibição de um contato.</span><span class="sxs-lookup"><span data-stu-id="2b139-126">Specifies the display name of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2b139-127">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2b139-127">Parent elements</span></span>

|<span data-ttu-id="2b139-128">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2b139-128">**Element**</span></span>|<span data-ttu-id="2b139-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2b139-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b139-130">Contatos (ArrayOfContactsType)</span><span class="sxs-lookup"><span data-stu-id="2b139-130">Contacts (ArrayOfContactsType)</span></span>](contacts-arrayofcontactstype.md) <br/> |<span data-ttu-id="2b139-131">Especifica uma matriz de contatos.</span><span class="sxs-lookup"><span data-stu-id="2b139-131">Specifies an array of contacts.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2b139-132">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="2b139-132">Remarks</span></span>

<span data-ttu-id="2b139-133">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2b139-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2b139-134">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b139-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b139-135">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2b139-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b139-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="2b139-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2b139-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2b139-137">Schema Name</span></span>  <br/> |<span data-ttu-id="2b139-138">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="2b139-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="2b139-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2b139-139">Validation File</span></span>  <br/> |<span data-ttu-id="2b139-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2b139-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2b139-141">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="2b139-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2b139-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="2b139-142">See also</span></span>



- [<span data-ttu-id="2b139-143">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2b139-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

