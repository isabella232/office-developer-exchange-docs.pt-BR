---
title: EmailUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc8133ff-c34e-4921-bb56-06e79aee0a8a
description: O elemento EmailUser especifica um destinatário de email.
ms.openlocfilehash: c090106a536f4f40908d364cc3c9c43f6fe42beb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456532"
---
# <a name="emailuser"></a><span data-ttu-id="e2148-103">EmailUser</span><span class="sxs-lookup"><span data-stu-id="e2148-103">EmailUser</span></span>

<span data-ttu-id="e2148-104">O elemento **EmailUser** especifica um destinatário de email.</span><span class="sxs-lookup"><span data-stu-id="e2148-104">The **EmailUser** element specifies an email recipient.</span></span> 
  
```XML
<EmailUser>
    <Name/>
    <UserId/>
</EmailUser>
```

 <span data-ttu-id="e2148-105">**EmailUserType**</span><span class="sxs-lookup"><span data-stu-id="e2148-105">**EmailUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2148-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e2148-106">Attributes and elements</span></span>

<span data-ttu-id="e2148-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e2148-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2148-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e2148-108">Attributes</span></span>

<span data-ttu-id="e2148-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2148-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2148-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e2148-110">Child elements</span></span>

|<span data-ttu-id="e2148-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e2148-111">**Element**</span></span>|<span data-ttu-id="e2148-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e2148-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2148-113">Nome (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="e2148-113">Name (string)</span></span>](name-string.md) <br/> |<span data-ttu-id="e2148-114">Especifica um nome ou chave de refinador de pesquisa ou o nome de um usuário de email.</span><span class="sxs-lookup"><span data-stu-id="e2148-114">Specifies a search refiner name or key or the name of an email user.</span></span>  <br/> |
|[<span data-ttu-id="e2148-115">UserId (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="e2148-115">UserId (string)</span></span>](userid-string.md) <br/> |<span data-ttu-id="e2148-116">Especifica o identificador de usuário de um usuário de email.</span><span class="sxs-lookup"><span data-stu-id="e2148-116">Specifies the user identifier of an email user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e2148-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e2148-117">Parent elements</span></span>

|<span data-ttu-id="e2148-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e2148-118">**Element**</span></span>|<span data-ttu-id="e2148-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e2148-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2148-120">Participantes</span><span class="sxs-lookup"><span data-stu-id="e2148-120">Attendees</span></span>](attendees.md) <br/> |<span data-ttu-id="e2148-121">Especifica os destinatários de um convite para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="e2148-121">Specifies the recipients of an invitation to a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e2148-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="e2148-122">Remarks</span></span>

<span data-ttu-id="e2148-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e2148-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e2148-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2148-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2148-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e2148-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2148-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="e2148-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e2148-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e2148-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e2148-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="e2148-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="e2148-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e2148-129">Validation File</span></span>  <br/> |<span data-ttu-id="e2148-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e2148-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e2148-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e2148-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e2148-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="e2148-132">See also</span></span>



- [<span data-ttu-id="e2148-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e2148-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

