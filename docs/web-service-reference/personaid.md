---
title: PersonaId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: eec3a468-afd5-4d72-a61e-cd1964fb686c
description: O elemento PersonaId Especifica o identificador de pessoa para a pessoa associada.
ms.openlocfilehash: 77668a1b32a97eef08b3316c7d4d7c8e6494c7bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824738"
---
# <a name="personaid"></a><span data-ttu-id="a3f90-103">PersonaId</span><span class="sxs-lookup"><span data-stu-id="a3f90-103">PersonaId</span></span>

<span data-ttu-id="a3f90-104">O elemento **PersonaId** Especifica o identificador de pessoa para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="a3f90-104">The **PersonaId** element specifies the persona identifier for the associated persona.</span></span> 
  
```XML
<PersonaId Id="" ChangeKey=""/>
```

 <span data-ttu-id="a3f90-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="a3f90-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a3f90-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a3f90-106">Attributes and elements</span></span>

<span data-ttu-id="a3f90-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a3f90-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3f90-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a3f90-108">Attributes</span></span>

|<span data-ttu-id="a3f90-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="a3f90-109">**Attribute**</span></span>|<span data-ttu-id="a3f90-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a3f90-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a3f90-111">Id</span><span class="sxs-lookup"><span data-stu-id="a3f90-111">Id</span></span>  <br/> |<span data-ttu-id="a3f90-112">O valor de texto do atributo **Id** é o identificador da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a3f90-112">The text value of the **Id** attribute is the identifier of the persona.</span></span>  <br/> |
|<span data-ttu-id="a3f90-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="a3f90-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="a3f90-114">O valor de texto do atributo **ChangeKey** é a chave de alteração da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a3f90-114">The text value of the **ChangeKey** attribute is the change key of the persona.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a3f90-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a3f90-115">Child elements</span></span>

<span data-ttu-id="a3f90-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a3f90-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a3f90-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a3f90-117">Parent elements</span></span>

<span data-ttu-id="a3f90-118">[GetPersona](getpersona.md) | [pessoa](persona.md)</span><span class="sxs-lookup"><span data-stu-id="a3f90-118">[GetPersona](getpersona.md) | [Persona](persona.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a3f90-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="a3f90-119">Remarks</span></span>

<span data-ttu-id="a3f90-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a3f90-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a3f90-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3f90-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3f90-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a3f90-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3f90-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="a3f90-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a3f90-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a3f90-124">Schema name</span></span>  <br/> |<span data-ttu-id="a3f90-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a3f90-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a3f90-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a3f90-126">Validation file</span></span>  <br/> |<span data-ttu-id="a3f90-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a3f90-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a3f90-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a3f90-128">Can be empty</span></span>  <br/> ||
   

