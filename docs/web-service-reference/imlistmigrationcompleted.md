---
title: ImListMigrationCompleted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6eed9502-5d9e-4345-ba23-3582ff487147
description: O elemento ImListMigrationCompleted indica se o repositório do Exchange contém os itens de mensagens instantâneas usados por clientes de mensagens instantâneas.
ms.openlocfilehash: 09f37d6e3663aab7cb98fc922f727ddd604f2acd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456021"
---
# <a name="imlistmigrationcompleted"></a><span data-ttu-id="013aa-103">ImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="013aa-103">ImListMigrationCompleted</span></span>

<span data-ttu-id="013aa-104">O elemento **ImListMigrationCompleted** indica se o repositório do Exchange contém os itens de mensagens instantâneas usados por clientes de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="013aa-104">The **ImListMigrationCompleted** element indicates whether the Exchange store contains the instant messaging items used by instant messaging clients.</span></span> 
  
```XML
<ImListMigrationCompleted>true | false</ImListMigrationCompleted>
```

 <span data-ttu-id="013aa-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="013aa-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="013aa-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="013aa-106">Attributes and elements</span></span>

<span data-ttu-id="013aa-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="013aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="013aa-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="013aa-108">Attributes</span></span>

<span data-ttu-id="013aa-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="013aa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="013aa-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="013aa-110">Child elements</span></span>

<span data-ttu-id="013aa-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="013aa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="013aa-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="013aa-112">Parent elements</span></span>

[<span data-ttu-id="013aa-113">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="013aa-113">SetImListMigrationCompleted</span></span>](setimlistmigrationcompleted.md)
  
## <a name="text-value"></a><span data-ttu-id="013aa-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="013aa-114">Text value</span></span>

<span data-ttu-id="013aa-115">Um valor de texto **true** para o elemento **ImListMigrationCompleted** indica que o repositório de contatos de mensagens instantâneas foi migrado para o repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="013aa-115">A text value of **true** for the **ImListMigrationCompleted** element indicates that the instant messaging contacts store has been migrated to the Exchange store.</span></span> <span data-ttu-id="013aa-116">Um valor **false** indica que o repositório de contatos de mensagens instantâneas não foi migrado.</span><span class="sxs-lookup"><span data-stu-id="013aa-116">A value of **false** indicates that the instant message contacts store has not been migrated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="013aa-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="013aa-117">Remarks</span></span>

<span data-ttu-id="013aa-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="013aa-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="013aa-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="013aa-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="013aa-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="013aa-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="013aa-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="013aa-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="013aa-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="013aa-122">Schema name</span></span>  <br/> |<span data-ttu-id="013aa-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="013aa-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="013aa-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="013aa-124">Validation file</span></span>  <br/> |<span data-ttu-id="013aa-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="013aa-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="013aa-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="013aa-126">Can be empty</span></span>  <br/> ||
   

