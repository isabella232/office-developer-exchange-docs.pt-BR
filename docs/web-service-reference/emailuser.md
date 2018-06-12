---
title: EmailUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc8133ff-c34e-4921-bb56-06e79aee0a8a
description: O elemento EmailUser Especifica um destinatário de email.
ms.openlocfilehash: e724b3996d37a42527ec1183cef9bb6b312b8c93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752034"
---
# <a name="emailuser"></a><span data-ttu-id="8b0a5-103">EmailUser</span><span class="sxs-lookup"><span data-stu-id="8b0a5-103">EmailUser</span></span>

<span data-ttu-id="8b0a5-104">O elemento **EmailUser** Especifica um destinatário de email.</span><span class="sxs-lookup"><span data-stu-id="8b0a5-104">The **EmailUser** element specifies an email recipient.</span></span> 
  
```XML
<EmailUser>
    <Name/>
    <UserId/>
</EmailUser>
```

 <span data-ttu-id="8b0a5-105">**EmailUserType**</span><span class="sxs-lookup"><span data-stu-id="8b0a5-105">**EmailUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b0a5-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8b0a5-106">Attributes and elements</span></span>

<span data-ttu-id="8b0a5-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8b0a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b0a5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8b0a5-108">Attributes</span></span>

<span data-ttu-id="8b0a5-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8b0a5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b0a5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8b0a5-110">Child elements</span></span>

|<span data-ttu-id="8b0a5-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8b0a5-111">**Element**</span></span>|<span data-ttu-id="8b0a5-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8b0a5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b0a5-113">Nome (string)</span><span class="sxs-lookup"><span data-stu-id="8b0a5-113">Name (string)</span></span>](name-string.md) <br/> |<span data-ttu-id="8b0a5-114">Especifica o nome de um usuário de email ou um nome de refinador de pesquisa ou chave.</span><span class="sxs-lookup"><span data-stu-id="8b0a5-114">Specifies a search refiner name or key or the name of an email user.</span></span>  <br/> |
|[<span data-ttu-id="8b0a5-115">UserId (string)</span><span class="sxs-lookup"><span data-stu-id="8b0a5-115">UserId (string)</span></span>](userid-string.md) <br/> |<span data-ttu-id="8b0a5-116">Especifica o identificador de usuário de um usuário de email.</span><span class="sxs-lookup"><span data-stu-id="8b0a5-116">Specifies the user identifier of an email user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8b0a5-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8b0a5-117">Parent elements</span></span>

|<span data-ttu-id="8b0a5-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8b0a5-118">**Element**</span></span>|<span data-ttu-id="8b0a5-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8b0a5-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b0a5-120">Participantes</span><span class="sxs-lookup"><span data-stu-id="8b0a5-120">Attendees</span></span>](attendees.md) <br/> |<span data-ttu-id="8b0a5-121">Especifica os destinatários de um convite para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="8b0a5-121">Specifies the recipients of an invitation to a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8b0a5-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="8b0a5-122">Remarks</span></span>

<span data-ttu-id="8b0a5-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8b0a5-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8b0a5-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b0a5-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b0a5-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8b0a5-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b0a5-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="8b0a5-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8b0a5-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8b0a5-127">Schema Name</span></span>  <br/> |<span data-ttu-id="8b0a5-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="8b0a5-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="8b0a5-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8b0a5-129">Validation File</span></span>  <br/> |<span data-ttu-id="8b0a5-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8b0a5-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8b0a5-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="8b0a5-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8b0a5-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="8b0a5-132">See also</span></span>



- [<span data-ttu-id="8b0a5-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8b0a5-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

