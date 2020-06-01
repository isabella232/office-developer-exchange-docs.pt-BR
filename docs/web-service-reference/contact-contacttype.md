---
title: Contato (ContactType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f7119b7-f5b4-484d-a7de-fa74836d9aee
description: O elemento Contact especifica um contato no repositório unificado de contatos.
ms.openlocfilehash: e8ebc28456f8bfc26f5d790ac9ff278930041ea0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461517"
---
# <a name="contact-contacttype"></a><span data-ttu-id="f5170-103">Contato (ContactType)</span><span class="sxs-lookup"><span data-stu-id="f5170-103">Contact (ContactType)</span></span>

<span data-ttu-id="f5170-104">O elemento **Contact** especifica um contato no repositório unificado de contatos.</span><span class="sxs-lookup"><span data-stu-id="f5170-104">The **Contact** element specifies a contact in the Unified Contact Store.</span></span> 
  
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

 <span data-ttu-id="f5170-105">**ContactType**</span><span class="sxs-lookup"><span data-stu-id="f5170-105">**ContactType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f5170-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f5170-106">Attributes and elements</span></span>

<span data-ttu-id="f5170-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f5170-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5170-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f5170-108">Attributes</span></span>

<span data-ttu-id="f5170-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5170-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f5170-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f5170-110">Child elements</span></span>

|<span data-ttu-id="f5170-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f5170-111">**Element**</span></span>|<span data-ttu-id="f5170-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f5170-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5170-113">PersonName</span><span class="sxs-lookup"><span data-stu-id="f5170-113">PersonName</span></span>](personname.md) <br/> |<span data-ttu-id="f5170-114">Especifica o nome de um indivíduo.</span><span class="sxs-lookup"><span data-stu-id="f5170-114">Specifies the name of an individual.</span></span>  <br/> |
|[<span data-ttu-id="f5170-115">BusinessName</span><span class="sxs-lookup"><span data-stu-id="f5170-115">BusinessName</span></span>](businessname.md) <br/> |<span data-ttu-id="f5170-116">Especifica o nome de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="f5170-116">Specifies the name of a business.</span></span>  <br/> |
|[<span data-ttu-id="f5170-117">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="f5170-117">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="f5170-118">Representa uma coleção de números de telefone de um contato.</span><span class="sxs-lookup"><span data-stu-id="f5170-118">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
|[<span data-ttu-id="f5170-119">URLs</span><span class="sxs-lookup"><span data-stu-id="f5170-119">Urls</span></span>](urls.md) <br/> |<span data-ttu-id="f5170-120">Especifica uma matriz de URLs para uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="f5170-120">Specifies an array of URLs for a persona.</span></span>  <br/> |
|[<span data-ttu-id="f5170-121">EmailAddresses (ArrayOfExtractedEmailAddresses)</span><span class="sxs-lookup"><span data-stu-id="f5170-121">EmailAddresses (ArrayOfExtractedEmailAddresses)</span></span>](emailaddresses-arrayofextractedemailaddresses.md) <br/> |<span data-ttu-id="f5170-122">Especifica uma matriz de endereços de email extraídos.</span><span class="sxs-lookup"><span data-stu-id="f5170-122">Specifies an array of extracted email addresses.</span></span>  <br/> |
|[<span data-ttu-id="f5170-123">Endereços (ArrayOfAddressesType)</span><span class="sxs-lookup"><span data-stu-id="f5170-123">Addresses (ArrayOfAddressesType)</span></span>](addresses-arrayofaddressestype.md) <br/> |<span data-ttu-id="f5170-124">Especifica uma matriz de elementos de **endereço** .</span><span class="sxs-lookup"><span data-stu-id="f5170-124">Specifies an array of **Address** elements.</span></span>  <br/> |
|[<span data-ttu-id="f5170-125">Contactstring</span><span class="sxs-lookup"><span data-stu-id="f5170-125">ContactString</span></span>](contactstring.md) <br/> |<span data-ttu-id="f5170-126">Especifica o nome de exibição de um contato.</span><span class="sxs-lookup"><span data-stu-id="f5170-126">Specifies the display name of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f5170-127">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f5170-127">Parent elements</span></span>

|<span data-ttu-id="f5170-128">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f5170-128">**Element**</span></span>|<span data-ttu-id="f5170-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f5170-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5170-130">Contatos (ArrayOfContactsType)</span><span class="sxs-lookup"><span data-stu-id="f5170-130">Contacts (ArrayOfContactsType)</span></span>](contacts-arrayofcontactstype.md) <br/> |<span data-ttu-id="f5170-131">Especifica uma matriz de contatos.</span><span class="sxs-lookup"><span data-stu-id="f5170-131">Specifies an array of contacts.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f5170-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="f5170-132">Remarks</span></span>

<span data-ttu-id="f5170-133">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f5170-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f5170-134">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5170-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f5170-135">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f5170-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f5170-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="f5170-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f5170-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f5170-137">Schema Name</span></span>  <br/> |<span data-ttu-id="f5170-138">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="f5170-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="f5170-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f5170-139">Validation File</span></span>  <br/> |<span data-ttu-id="f5170-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f5170-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f5170-141">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f5170-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f5170-142">Também consulte</span><span class="sxs-lookup"><span data-stu-id="f5170-142">See also</span></span>



- [<span data-ttu-id="f5170-143">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f5170-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

