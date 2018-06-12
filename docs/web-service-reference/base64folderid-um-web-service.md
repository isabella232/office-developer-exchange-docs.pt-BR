---
title: base64FolderId (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- base64FolderId
api_type:
- schema
ms.assetid: 662f8f2f-49a7-4c7a-9065-98a02a49cfcd
description: O elemento base64FolderId contém o identificador da pasta para especificar como a pasta de email padrão do qual Unificação de mensagens lê as mensagens por telefone em uma solicitação do SetTelephoneAccessFolderEmail operação (serviço web de Unificação de mensagens).
ms.openlocfilehash: 7d710542418a717c6fcad243a22682e5840ebbd2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751256"
---
# <a name="base64folderid-um-web-service"></a><span data-ttu-id="7a4c4-103">base64FolderId (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="7a4c4-103">base64FolderId (UM web service)</span></span>

<span data-ttu-id="7a4c4-104">O elemento **base64FolderId** contém o identificador da pasta para especificar como a pasta de email padrão do qual Unificação de mensagens lê as mensagens por telefone em uma solicitação de [operação SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)](settelephoneaccessfolderemail-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="7a4c4-104">The **base64FolderId** element contains the identifier of the folder to specify as the default e-mail folder from which Unified Messaging reads messages over the telephone in a [SetTelephoneAccessFolderEmail operation (UM web service)](settelephoneaccessfolderemail-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="7a4c4-105">SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="7a4c4-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="7a4c4-106">base64FolderId (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="7a4c4-106">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 <span data-ttu-id="7a4c4-107">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="7a4c4-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a4c4-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7a4c4-108">Attributes and elements</span></span>

<span data-ttu-id="7a4c4-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7a4c4-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a4c4-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="7a4c4-110">Attributes</span></span>

<span data-ttu-id="7a4c4-111">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7a4c4-111">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a4c4-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7a4c4-112">Child elements</span></span>

<span data-ttu-id="7a4c4-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7a4c4-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7a4c4-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7a4c4-114">Parent elements</span></span>

|<span data-ttu-id="7a4c4-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7a4c4-115">**Element**</span></span>|<span data-ttu-id="7a4c4-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7a4c4-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a4c4-117">SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="7a4c4-117">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="7a4c4-118">Define a solicitação para definir a pasta de email de acesso de telefone.</span><span class="sxs-lookup"><span data-stu-id="7a4c4-118">Defines request to set the telephone access e-mail folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7a4c4-119">Text value</span><span class="sxs-lookup"><span data-stu-id="7a4c4-119">Text value</span></span>

<span data-ttu-id="7a4c4-120">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="7a4c4-120">A text value is required.</span></span> <span data-ttu-id="7a4c4-121">O valor de texto representa a identificação de MAPI da pasta.</span><span class="sxs-lookup"><span data-stu-id="7a4c4-121">The text value represents the MAPI ID of the folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7a4c4-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="7a4c4-122">Remarks</span></span>

<span data-ttu-id="7a4c4-123">Para definir a pasta de email de acesso de telefone, use a [operação SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)](settelephoneaccessfolderemail-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="7a4c4-123">To set the telephone access e-mail folder, use the [SetTelephoneAccessFolderEmail operation (UM web service)](settelephoneaccessfolderemail-operation-um-web-service.md).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a4c4-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7a4c4-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a4c4-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="7a4c4-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7a4c4-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7a4c4-126">Schema Name</span></span>  <br/> |<span data-ttu-id="7a4c4-127">Mensagens</span><span class="sxs-lookup"><span data-stu-id="7a4c4-127">Messages</span></span>  <br/> |
|<span data-ttu-id="7a4c4-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7a4c4-128">Validation File</span></span>  <br/> |<span data-ttu-id="7a4c4-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7a4c4-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7a4c4-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7a4c4-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="7a4c4-131">False</span><span class="sxs-lookup"><span data-stu-id="7a4c4-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a4c4-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="7a4c4-132">See also</span></span>



[<span data-ttu-id="7a4c4-133">SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="7a4c4-133">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="7a4c4-134">Operação de SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="7a4c4-134">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[<span data-ttu-id="7a4c4-135">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="7a4c4-135">FindFolder operation</span></span>](findfolder-operation.md)
  
[<span data-ttu-id="7a4c4-136">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="7a4c4-136">FindItem operation</span></span>](finditem-operation.md)

