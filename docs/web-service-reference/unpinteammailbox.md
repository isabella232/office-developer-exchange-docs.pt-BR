---
title: UnpinTeamMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1034b013-ef34-4e72-99b3-38bff475b3e8
description: O elemento UnpinTeamMailbox contém a solicitação para Desafixar uma caixa de correio do site do cliente por removê-lo da resposta da descoberta automática.
ms.openlocfilehash: d303b47f0796f9bec7e9f198afa81d2ecd9fd5cd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837855"
---
# <a name="unpinteammailbox"></a><span data-ttu-id="74363-103">UnpinTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="74363-103">UnpinTeamMailbox</span></span>

<span data-ttu-id="74363-104">O elemento **UnpinTeamMailbox** contém a solicitação para Desafixar uma caixa de correio do site do cliente por removê-lo da resposta da **descoberta automática** .</span><span class="sxs-lookup"><span data-stu-id="74363-104">The **UnpinTeamMailbox** element contains the request to unpin a site mailbox from the client by removing it from the **Autodiscover** response.</span></span> 
  
```XML
<UnpinTeamMailbox>
   <EmailAddress/>
</UnpinTeamMailbox>
```

 <span data-ttu-id="74363-105">**UnpinTeamMailboxRequestType**</span><span class="sxs-lookup"><span data-stu-id="74363-105">**UnpinTeamMailboxRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74363-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="74363-106">Attributes and elements</span></span>

<span data-ttu-id="74363-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="74363-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74363-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="74363-108">Attributes</span></span>

<span data-ttu-id="74363-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="74363-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74363-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="74363-110">Child elements</span></span>

[<span data-ttu-id="74363-111">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="74363-111">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="74363-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="74363-112">Parent elements</span></span>

<span data-ttu-id="74363-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="74363-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="74363-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="74363-114">Remarks</span></span>

<span data-ttu-id="74363-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="74363-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="74363-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="74363-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74363-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="74363-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74363-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="74363-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="74363-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="74363-119">Schema name</span></span>  <br/> |<span data-ttu-id="74363-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="74363-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="74363-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="74363-121">Validation file</span></span>  <br/> |<span data-ttu-id="74363-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="74363-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74363-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="74363-123">Can be empty</span></span>  <br/> ||
   

