---
title: GetSearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 949871f7-0d10-498e-84aa-f0652f1193be
description: O elemento GetSearchableMailboxes contém uma solicitação para obter uma lista de caixas de correio que o cliente tem permissão para executar uma pesquisa de descoberta eletrônica.
ms.openlocfilehash: a327f8766e53e9f1fae6928179d5a4b8e3d044a8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530187"
---
# <a name="getsearchablemailboxes"></a><span data-ttu-id="d57ef-103">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="d57ef-103">GetSearchableMailboxes</span></span>

<span data-ttu-id="d57ef-104">O elemento **GetSearchableMailboxes** contém uma solicitação para obter uma lista de caixas de correio que o cliente tem permissão para executar uma pesquisa de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="d57ef-104">The **GetSearchableMailboxes** element contains a request to get a list of mailboxes that the client has permission to perform an eDiscovery search.</span></span> 
  
```XML
<GetSearchableMailboxes>
   <SearchFilter/>
   <ExpandGroupMembership/>
</GetSearchableMailboxes>
```

 <span data-ttu-id="d57ef-105">**GetSearchableMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="d57ef-105">**GetSearchableMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d57ef-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d57ef-106">Attributes and elements</span></span>

<span data-ttu-id="d57ef-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d57ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d57ef-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d57ef-108">Attributes</span></span>

<span data-ttu-id="d57ef-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d57ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d57ef-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d57ef-110">Child elements</span></span>

<span data-ttu-id="d57ef-111">[SearchFilter](searchfilter.md)  |  [ExpandGroupMembership](expandgroupmembership.md)</span><span class="sxs-lookup"><span data-stu-id="d57ef-111">[SearchFilter](searchfilter.md) | [ExpandGroupMembership](expandgroupmembership.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d57ef-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d57ef-112">Parent elements</span></span>

<span data-ttu-id="d57ef-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d57ef-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d57ef-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="d57ef-114">Remarks</span></span>

<span data-ttu-id="d57ef-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d57ef-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d57ef-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d57ef-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d57ef-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d57ef-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d57ef-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="d57ef-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d57ef-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d57ef-119">Schema name</span></span>  <br/> |<span data-ttu-id="d57ef-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d57ef-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d57ef-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d57ef-121">Validation file</span></span>  <br/> |<span data-ttu-id="d57ef-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d57ef-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d57ef-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d57ef-123">Can be empty</span></span>  <br/> ||
   

