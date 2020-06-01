---
title: UserSMIMECertificate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 66e6b4ba-368d-4469-bd47-e59441b7d64d
description: O elemento UserSMIMECertificate contém um valor que codifica o certificado SMIME de um contato.
ms.openlocfilehash: 7e2dbc6a9c8b04758ba99db036e237d8837850aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467652"
---
# <a name="usersmimecertificate"></a><span data-ttu-id="864fd-103">UserSMIMECertificate</span><span class="sxs-lookup"><span data-stu-id="864fd-103">UserSMIMECertificate</span></span>

<span data-ttu-id="864fd-104">O elemento **UserSMIMECertificate** contém um valor que codifica o certificado SMIME de um contato.</span><span class="sxs-lookup"><span data-stu-id="864fd-104">The **UserSMIMECertificate** element contains a value that encodes a contact's SMIME certificate.</span></span> 
  
```XML
<UserSMIMECertificate/>
```

 <span data-ttu-id="864fd-105">**ArrayOfBinaryType**</span><span class="sxs-lookup"><span data-stu-id="864fd-105">**ArrayOfBinaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="864fd-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="864fd-106">Attributes and elements</span></span>

<span data-ttu-id="864fd-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="864fd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="864fd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="864fd-108">Attributes</span></span>

<span data-ttu-id="864fd-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="864fd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="864fd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="864fd-110">Child elements</span></span>

|<span data-ttu-id="864fd-111">**Nome do elemento**</span><span class="sxs-lookup"><span data-stu-id="864fd-111">**Element name**</span></span>|<span data-ttu-id="864fd-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="864fd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="864fd-113">Base64Binary</span><span class="sxs-lookup"><span data-stu-id="864fd-113">Base64Binary</span></span>](base64binary.md) <br/> |<span data-ttu-id="864fd-114">Contém um valor codificado em base64.</span><span class="sxs-lookup"><span data-stu-id="864fd-114">Contains a Base64-encoded value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="864fd-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="864fd-115">Parent elements</span></span>

|<span data-ttu-id="864fd-116">**Nome do elemento**</span><span class="sxs-lookup"><span data-stu-id="864fd-116">**Element name**</span></span>|<span data-ttu-id="864fd-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="864fd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="864fd-118">Contato</span><span class="sxs-lookup"><span data-stu-id="864fd-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="864fd-119">Representa um item de contato no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="864fd-119">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="864fd-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="864fd-120">Text value</span></span>

<span data-ttu-id="864fd-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="864fd-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="864fd-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="864fd-122">Remarks</span></span>

<span data-ttu-id="864fd-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="864fd-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="864fd-124">Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="864fd-124">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="864fd-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="864fd-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="864fd-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="864fd-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="864fd-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="864fd-127">Schema name</span></span>  <br/> |<span data-ttu-id="864fd-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="864fd-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="864fd-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="864fd-129">Validation file</span></span>  <br/> |<span data-ttu-id="864fd-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="864fd-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="864fd-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="864fd-131">Can be empty</span></span>  <br/> |<span data-ttu-id="864fd-132">False</span><span class="sxs-lookup"><span data-stu-id="864fd-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="864fd-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="864fd-133">See also</span></span>



- [<span data-ttu-id="864fd-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="864fd-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="864fd-135">Criando contatos (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="864fd-135">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

