---
title: IsModerated
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsModerated
api_type:
- schema
ms.assetid: a7562256-feb9-41a1-857e-b5d41cbed680
description: O elemento IsModerated indica se a caixa de correio do destinatário está sendo moderada.
ms.openlocfilehash: 8db234f9706bb8187978a76f745323749d7a640a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824055"
---
# <a name="ismoderated"></a><span data-ttu-id="1907a-103">IsModerated</span><span class="sxs-lookup"><span data-stu-id="1907a-103">IsModerated</span></span>

<span data-ttu-id="1907a-104">O elemento **IsModerated** indica se a caixa de correio do destinatário está sendo moderada.</span><span class="sxs-lookup"><span data-stu-id="1907a-104">The **IsModerated** element indicates whether the recipient's mailbox is being moderated.</span></span> 
  
```XML
<IsModerated>true | false</IsModerated>
```

 <span data-ttu-id="1907a-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="1907a-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1907a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1907a-106">Attributes and elements</span></span>

<span data-ttu-id="1907a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1907a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1907a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1907a-108">Attributes</span></span>

<span data-ttu-id="1907a-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1907a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1907a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1907a-110">Child elements</span></span>

<span data-ttu-id="1907a-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1907a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1907a-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1907a-112">Parent elements</span></span>

|<span data-ttu-id="1907a-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1907a-113">**Element**</span></span>|<span data-ttu-id="1907a-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1907a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1907a-115">Dicas de email</span><span class="sxs-lookup"><span data-stu-id="1907a-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="1907a-116">Representa os valores para os vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="1907a-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1907a-117">Text value</span><span class="sxs-lookup"><span data-stu-id="1907a-117">Text value</span></span>

<span data-ttu-id="1907a-118">O valor de texto para esse elemento é **true** se a caixa de correio do destinatário moderada.</span><span class="sxs-lookup"><span data-stu-id="1907a-118">The text value for this element is **true** if the recipient's mailbox is being moderated.</span></span> <span data-ttu-id="1907a-119">O valor é **false** se a caixa de correio do destinatário não está sendo moderada.</span><span class="sxs-lookup"><span data-stu-id="1907a-119">The value is **false** if the recipient's mailbox is not being moderated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1907a-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="1907a-120">Remarks</span></span>

<span data-ttu-id="1907a-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1907a-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1907a-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1907a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1907a-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="1907a-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1907a-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1907a-124">Schema Name</span></span>  <br/> |<span data-ttu-id="1907a-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1907a-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="1907a-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1907a-126">Validation File</span></span>  <br/> |<span data-ttu-id="1907a-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1907a-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1907a-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1907a-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="1907a-129">False</span><span class="sxs-lookup"><span data-stu-id="1907a-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1907a-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="1907a-130">See also</span></span>



- [<span data-ttu-id="1907a-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1907a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

