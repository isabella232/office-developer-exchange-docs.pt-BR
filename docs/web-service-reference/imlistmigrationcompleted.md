---
title: ImListMigrationCompleted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6eed9502-5d9e-4345-ba23-3582ff487147
description: O elemento ImListMigrationCompleted indica se o armazenamento do Exchange contém os itens de mensagens instantâneos usados por clientes de mensagens instantâneas.
ms.openlocfilehash: 25f1b583b354a71958fbc8052c492726dc0eb7db
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823893"
---
# <a name="imlistmigrationcompleted"></a><span data-ttu-id="83ef7-103">ImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="83ef7-103">ImListMigrationCompleted</span></span>

<span data-ttu-id="83ef7-104">O elemento **ImListMigrationCompleted** indica se o armazenamento do Exchange contém a itens usados por clientes de mensagens instantâneas de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="83ef7-104">The **ImListMigrationCompleted** element indicates whether the Exchange store contains the instant messaging items used by instant messaging clients.</span></span> 
  
```XML
<ImListMigrationCompleted>true | false</ImListMigrationCompleted>
```

 <span data-ttu-id="83ef7-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="83ef7-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="83ef7-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="83ef7-106">Attributes and elements</span></span>

<span data-ttu-id="83ef7-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="83ef7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83ef7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="83ef7-108">Attributes</span></span>

<span data-ttu-id="83ef7-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="83ef7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83ef7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="83ef7-110">Child elements</span></span>

<span data-ttu-id="83ef7-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="83ef7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="83ef7-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="83ef7-112">Parent elements</span></span>

[<span data-ttu-id="83ef7-113">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="83ef7-113">SetImListMigrationCompleted</span></span>](setimlistmigrationcompleted.md)
  
## <a name="text-value"></a><span data-ttu-id="83ef7-114">Text value</span><span class="sxs-lookup"><span data-stu-id="83ef7-114">Text value</span></span>

<span data-ttu-id="83ef7-115">Um valor de texto de **true** para o elemento **ImListMigrationCompleted** indica que os contatos de mensagens instantâneas repositório ter sido migrado para o Exchange armazenam.</span><span class="sxs-lookup"><span data-stu-id="83ef7-115">A text value of **true** for the **ImListMigrationCompleted** element indicates that the instant messaging contacts store has been migrated to the Exchange store.</span></span> <span data-ttu-id="83ef7-116">Um valor **false** indica que o repositório de contatos de mensagem instantânea não tenha sido migrado.</span><span class="sxs-lookup"><span data-stu-id="83ef7-116">A value of **false** indicates that the instant message contacts store has not been migrated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="83ef7-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="83ef7-117">Remarks</span></span>

<span data-ttu-id="83ef7-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="83ef7-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="83ef7-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="83ef7-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83ef7-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="83ef7-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83ef7-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="83ef7-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="83ef7-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="83ef7-122">Schema name</span></span>  <br/> |<span data-ttu-id="83ef7-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="83ef7-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="83ef7-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="83ef7-124">Validation file</span></span>  <br/> |<span data-ttu-id="83ef7-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="83ef7-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="83ef7-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="83ef7-126">Can be empty</span></span>  <br/> ||
   

