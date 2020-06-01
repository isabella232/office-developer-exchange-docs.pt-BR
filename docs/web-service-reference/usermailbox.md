---
title: UserMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1d47141c-3c3f-45b8-90c5-33a44adb34b2
description: O elemento UserMailbox identifica uma caixa de correio de usuário.
ms.openlocfilehash: 9bb1b08320f5e6f4843383a8e3aff96fc3dcccad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465314"
---
# <a name="usermailbox"></a><span data-ttu-id="b5906-103">UserMailbox</span><span class="sxs-lookup"><span data-stu-id="b5906-103">UserMailbox</span></span>

<span data-ttu-id="b5906-104">O elemento **UserMailbox** identifica uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="b5906-104">The **UserMailbox** element identifies a user mailbox.</span></span> 
  
```XML
<UserMailbox Id="" IsArchive=""/>
```

 <span data-ttu-id="b5906-105">**Usermailboxtype**</span><span class="sxs-lookup"><span data-stu-id="b5906-105">**UserMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b5906-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b5906-106">Attributes and elements</span></span>

<span data-ttu-id="b5906-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b5906-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5906-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b5906-108">Attributes</span></span>

|<span data-ttu-id="b5906-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="b5906-109">**Attribute**</span></span>|<span data-ttu-id="b5906-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b5906-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b5906-111">Id</span><span class="sxs-lookup"><span data-stu-id="b5906-111">Id</span></span>  <br/> |<span data-ttu-id="b5906-112">O valor de texto do atributo **ID** é o identificador da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b5906-112">The text value of the **Id** attribute is the identifier of the mailbox.</span></span>  <br/> |
|<span data-ttu-id="b5906-113">IsArchive</span><span class="sxs-lookup"><span data-stu-id="b5906-113">IsArchive</span></span>  <br/> |<span data-ttu-id="b5906-114">O valor de texto do atributo **IsArchive** indica se a caixa de correio é uma caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="b5906-114">The text value of the **IsArchive** attribute indicates whether the mailbox is an archive mailbox.</span></span> <span data-ttu-id="b5906-115">Um valor de texto **true** para o atributo **IsArchive** indica que a caixa de correio é uma caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="b5906-115">A text value of **true** for the **IsArchive** attribute indicates that the mailbox is an archive mailbox.</span></span> <span data-ttu-id="b5906-116">Um valor **false** para o atributo **IsArchive** indica que a caixa de correio é uma caixa de correio principal.</span><span class="sxs-lookup"><span data-stu-id="b5906-116">A value of **false** for the **IsArchive** attribute indicates that the mailbox is a primary mailbox.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b5906-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b5906-117">Child elements</span></span>

<span data-ttu-id="b5906-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b5906-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b5906-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b5906-119">Parent elements</span></span>

<span data-ttu-id="b5906-120">[Caixas de correio (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md)  |  [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)</span><span class="sxs-lookup"><span data-stu-id="b5906-120">[Mailboxes (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) | [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b5906-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="b5906-121">Remarks</span></span>

<span data-ttu-id="b5906-122">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b5906-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b5906-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5906-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b5906-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b5906-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b5906-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="b5906-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b5906-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b5906-126">Schema name</span></span>  <br/> |<span data-ttu-id="b5906-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b5906-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="b5906-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b5906-128">Validation file</span></span>  <br/> |<span data-ttu-id="b5906-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b5906-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b5906-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b5906-130">Can be empty</span></span>  <br/> |<span data-ttu-id="b5906-131">verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b5906-131">true</span></span>  <br/> |
   

