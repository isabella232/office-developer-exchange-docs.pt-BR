---
title: GetImItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 455e5709-6c06-49fd-bfb2-403fc912287c
description: O elemento de solicitação de GetImItems define uma solicitação para obter mais informações sobre os grupos especificados de mensagens instantâneos e personagens contatos de mensagens instantâneas.
ms.openlocfilehash: ff7d520dde44fac6e9278633c1ad46b07b38d6c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752523"
---
# <a name="getimitems"></a><span data-ttu-id="5dcc5-103">GetImItems</span><span class="sxs-lookup"><span data-stu-id="5dcc5-103">GetImItems</span></span>

<span data-ttu-id="5dcc5-104">O elemento de solicitação de **GetImItems** define uma solicitação para obter mais informações sobre os grupos especificados de mensagens instantâneos e personagens contatos de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="5dcc5-104">The **GetImItems** request element defines a request to get information about the specified instant messaging groups and instant messaging contact personas.</span></span> 
  
```XML
<GetImItems>
   <ContactIds/>
   <GroupIds/>
   <ExtendedProperties/>
</GetImItems>
```

 <span data-ttu-id="5dcc5-105">**GetImItemsType**</span><span class="sxs-lookup"><span data-stu-id="5dcc5-105">**GetImItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5dcc5-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5dcc5-106">Attributes and elements</span></span>

<span data-ttu-id="5dcc5-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5dcc5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5dcc5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5dcc5-108">Attributes</span></span>

<span data-ttu-id="5dcc5-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5dcc5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5dcc5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5dcc5-110">Child elements</span></span>

<span data-ttu-id="5dcc5-111">[ContactIds](contactids.md) | [IDs de grupo](groupids.md) | [ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)</span><span class="sxs-lookup"><span data-stu-id="5dcc5-111">[ContactIds](contactids.md) | [GroupIds](groupids.md) | [ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5dcc5-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5dcc5-112">Parent elements</span></span>

<span data-ttu-id="5dcc5-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5dcc5-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5dcc5-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="5dcc5-114">Remarks</span></span>

<span data-ttu-id="5dcc5-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5dcc5-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5dcc5-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5dcc5-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5dcc5-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5dcc5-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5dcc5-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="5dcc5-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5dcc5-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5dcc5-119">Schema name</span></span>  <br/> |<span data-ttu-id="5dcc5-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="5dcc5-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5dcc5-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5dcc5-121">Validation file</span></span>  <br/> |<span data-ttu-id="5dcc5-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5dcc5-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5dcc5-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5dcc5-123">Can be empty</span></span>  <br/> ||
   

