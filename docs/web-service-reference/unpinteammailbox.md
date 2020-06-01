---
title: UnpinTeamMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1034b013-ef34-4e72-99b3-38bff475b3e8
description: O elemento UnpinTeamMailbox contém a solicitação para Desafixar uma caixa de correio de site do cliente, removendo-a da resposta de descoberta automática.
ms.openlocfilehash: a6b01bfa9c5908765ff04ef7f5edbef0b99a9be2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467239"
---
# <a name="unpinteammailbox"></a><span data-ttu-id="20673-103">UnpinTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="20673-103">UnpinTeamMailbox</span></span>

<span data-ttu-id="20673-104">O elemento **UnpinTeamMailbox** contém a solicitação para Desafixar uma caixa de correio de site do cliente, removendo-a da resposta de **descoberta automática** .</span><span class="sxs-lookup"><span data-stu-id="20673-104">The **UnpinTeamMailbox** element contains the request to unpin a site mailbox from the client by removing it from the **Autodiscover** response.</span></span> 
  
```XML
<UnpinTeamMailbox>
   <EmailAddress/>
</UnpinTeamMailbox>
```

 <span data-ttu-id="20673-105">**UnpinTeamMailboxRequestType**</span><span class="sxs-lookup"><span data-stu-id="20673-105">**UnpinTeamMailboxRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20673-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="20673-106">Attributes and elements</span></span>

<span data-ttu-id="20673-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="20673-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20673-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="20673-108">Attributes</span></span>

<span data-ttu-id="20673-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20673-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20673-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="20673-110">Child elements</span></span>

[<span data-ttu-id="20673-111">EmailAddress (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="20673-111">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="20673-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="20673-112">Parent elements</span></span>

<span data-ttu-id="20673-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20673-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="20673-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="20673-114">Remarks</span></span>

<span data-ttu-id="20673-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="20673-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="20673-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="20673-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20673-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="20673-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20673-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="20673-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="20673-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="20673-119">Schema name</span></span>  <br/> |<span data-ttu-id="20673-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="20673-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="20673-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="20673-121">Validation file</span></span>  <br/> |<span data-ttu-id="20673-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="20673-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="20673-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="20673-123">Can be empty</span></span>  <br/> ||
   

