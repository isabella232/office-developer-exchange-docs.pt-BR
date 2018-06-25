---
title: UserMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1d47141c-3c3f-45b8-90c5-33a44adb34b2
description: O elemento UserMailbox identifica uma caixa de correio do usuário.
ms.openlocfilehash: 9f359a2b0ba315c236d4bf189c3de321417bd390
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837985"
---
# <a name="usermailbox"></a><span data-ttu-id="a1271-103">UserMailbox</span><span class="sxs-lookup"><span data-stu-id="a1271-103">UserMailbox</span></span>

<span data-ttu-id="a1271-104">O elemento **UserMailbox** identifica uma caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1271-104">The **UserMailbox** element identifies a user mailbox.</span></span> 
  
```XML
<UserMailbox Id="" IsArchive=""/>
```

 <span data-ttu-id="a1271-105">**UserMailboxType**</span><span class="sxs-lookup"><span data-stu-id="a1271-105">**UserMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a1271-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a1271-106">Attributes and elements</span></span>

<span data-ttu-id="a1271-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a1271-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1271-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a1271-108">Attributes</span></span>

|<span data-ttu-id="a1271-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="a1271-109">**Attribute**</span></span>|<span data-ttu-id="a1271-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a1271-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a1271-111">Id</span><span class="sxs-lookup"><span data-stu-id="a1271-111">Id</span></span>  <br/> |<span data-ttu-id="a1271-112">O valor de texto do atributo **Id** é o identificador da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a1271-112">The text value of the **Id** attribute is the identifier of the mailbox.</span></span>  <br/> |
|<span data-ttu-id="a1271-113">IsArchive</span><span class="sxs-lookup"><span data-stu-id="a1271-113">IsArchive</span></span>  <br/> |<span data-ttu-id="a1271-114">O valor de texto do atributo **IsArchive** indica se a caixa de correio é uma caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="a1271-114">The text value of the **IsArchive** attribute indicates whether the mailbox is an archive mailbox.</span></span> <span data-ttu-id="a1271-115">Um valor de texto de **true** para o atributo **IsArchive** indica que a caixa de correio é uma caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="a1271-115">A text value of **true** for the **IsArchive** attribute indicates that the mailbox is an archive mailbox.</span></span> <span data-ttu-id="a1271-116">Um valor **false** para o atributo **IsArchive** indica que a caixa de correio é uma caixa de correio principal.</span><span class="sxs-lookup"><span data-stu-id="a1271-116">A value of **false** for the **IsArchive** attribute indicates that the mailbox is a primary mailbox.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a1271-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a1271-117">Child elements</span></span>

<span data-ttu-id="a1271-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a1271-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a1271-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a1271-119">Parent elements</span></span>

<span data-ttu-id="a1271-120">[Caixas de correio (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) | [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)</span><span class="sxs-lookup"><span data-stu-id="a1271-120">[Mailboxes (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) | [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a1271-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="a1271-121">Remarks</span></span>

<span data-ttu-id="a1271-122">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a1271-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a1271-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1271-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1271-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a1271-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1271-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="a1271-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a1271-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a1271-126">Schema name</span></span>  <br/> |<span data-ttu-id="a1271-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a1271-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="a1271-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a1271-128">Validation file</span></span>  <br/> |<span data-ttu-id="a1271-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a1271-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a1271-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a1271-130">Can be empty</span></span>  <br/> |<span data-ttu-id="a1271-131">true</span><span class="sxs-lookup"><span data-stu-id="a1271-131">true</span></span>  <br/> |
   

