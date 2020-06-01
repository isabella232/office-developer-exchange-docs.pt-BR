---
title: AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: adbffbfc-e436-4620-acfc-5dfd41a88cb8
description: O elemento AddDistributionGroupToImList define uma solicitação para adicionar uma lista de distribuição a uma lista de mensagens instantâneas.
ms.openlocfilehash: 90a84b23678fb0740158f601967905a8847286fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460376"
---
# <a name="adddistributiongrouptoimlist"></a><span data-ttu-id="6b4ce-103">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="6b4ce-103">AddDistributionGroupToImList</span></span>

<span data-ttu-id="6b4ce-104">O elemento **AddDistributionGroupToImList** define uma solicitação para adicionar uma lista de distribuição a uma lista de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="6b4ce-104">The **AddDistributionGroupToImList** element defines a request to add a distribution list to an instant message list.</span></span> 
  
```XML
<AddDistributionGroupToImList>
   <SmtpAddress/>
   <DisplayName/>
</AddDistributionGroupToImList>
```

 <span data-ttu-id="6b4ce-105">**AddDistributionGroupToImListType**</span><span class="sxs-lookup"><span data-stu-id="6b4ce-105">**AddDistributionGroupToImListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b4ce-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6b4ce-106">Attributes and elements</span></span>

<span data-ttu-id="6b4ce-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6b4ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b4ce-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6b4ce-108">Attributes</span></span>

<span data-ttu-id="6b4ce-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b4ce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b4ce-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6b4ce-110">Child elements</span></span>

<span data-ttu-id="6b4ce-111">[SmtpAddress](smtpaddress.md)  |  [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)</span><span class="sxs-lookup"><span data-stu-id="6b4ce-111">[SmtpAddress](smtpaddress.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6b4ce-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6b4ce-112">Parent elements</span></span>

<span data-ttu-id="6b4ce-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b4ce-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6b4ce-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="6b4ce-114">Remarks</span></span>

<span data-ttu-id="6b4ce-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6b4ce-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6b4ce-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b4ce-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b4ce-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6b4ce-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b4ce-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="6b4ce-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6b4ce-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6b4ce-119">Schema name</span></span>  <br/> |<span data-ttu-id="6b4ce-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6b4ce-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6b4ce-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6b4ce-121">Validation file</span></span>  <br/> |<span data-ttu-id="6b4ce-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6b4ce-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6b4ce-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="6b4ce-123">Can be empty</span></span>  <br/> |<span data-ttu-id="6b4ce-124">falso</span><span class="sxs-lookup"><span data-stu-id="6b4ce-124">false</span></span>  <br/> |
   

