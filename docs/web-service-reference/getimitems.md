---
title: GetImItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 455e5709-6c06-49fd-bfb2-403fc912287c
description: O elemento de solicitação GetImItems define uma solicitação para obter informações sobre os grupos de mensagens instantâneas e as pessoas de contato de mensagens instantâneas especificadas.
ms.openlocfilehash: e3973cbbf800ffe91472b9c733c4d4a927b91c9f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456448"
---
# <a name="getimitems"></a><span data-ttu-id="4eeb3-103">GetImItems</span><span class="sxs-lookup"><span data-stu-id="4eeb3-103">GetImItems</span></span>

<span data-ttu-id="4eeb3-104">O elemento de solicitação **GetImItems** define uma solicitação para obter informações sobre os grupos de mensagens instantâneas e as pessoas de contato de mensagens instantâneas especificadas.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-104">The **GetImItems** request element defines a request to get information about the specified instant messaging groups and instant messaging contact personas.</span></span> 
  
```XML
<GetImItems>
   <ContactIds/>
   <GroupIds/>
   <ExtendedProperties/>
</GetImItems>
```

 <span data-ttu-id="4eeb3-105">**GetImItemsType**</span><span class="sxs-lookup"><span data-stu-id="4eeb3-105">**GetImItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4eeb3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4eeb3-106">Attributes and elements</span></span>

<span data-ttu-id="4eeb3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4eeb3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4eeb3-108">Attributes</span></span>

<span data-ttu-id="4eeb3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4eeb3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4eeb3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4eeb3-110">Child elements</span></span>

<span data-ttu-id="4eeb3-111">[ContactIds](contactids.md)  |  [GroupIds](groupids.md)  |  [ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)</span><span class="sxs-lookup"><span data-stu-id="4eeb3-111">[ContactIds](contactids.md) | [GroupIds](groupids.md) | [ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4eeb3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4eeb3-112">Parent elements</span></span>

<span data-ttu-id="4eeb3-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4eeb3-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4eeb3-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="4eeb3-114">Remarks</span></span>

<span data-ttu-id="4eeb3-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4eeb3-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4eeb3-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4eeb3-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4eeb3-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4eeb3-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="4eeb3-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4eeb3-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4eeb3-119">Schema name</span></span>  <br/> |<span data-ttu-id="4eeb3-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="4eeb3-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4eeb3-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4eeb3-121">Validation file</span></span>  <br/> |<span data-ttu-id="4eeb3-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4eeb3-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4eeb3-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4eeb3-123">Can be empty</span></span>  <br/> ||
   

