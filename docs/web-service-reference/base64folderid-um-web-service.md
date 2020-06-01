---
title: base64FolderId (serviço Web da UM)
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
description: O elemento base64FolderId contém o identificador da pasta para especificar como a pasta de email padrão da qual a Unificação de mensagens lê mensagens por telefone em uma solicitação de operação do SetTelephoneAccessFolderEmail (serviço da Web da UM).
ms.openlocfilehash: ea31c7a0f93188e563bf95c4a3e6e91f0866746c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458044"
---
# <a name="base64folderid-um-web-service"></a><span data-ttu-id="fb468-103">base64FolderId (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="fb468-103">base64FolderId (UM web service)</span></span>

<span data-ttu-id="fb468-104">O elemento **base64FolderId** contém o identificador da pasta para especificar como a pasta de email padrão da qual a Unificação de mensagens lê mensagens por telefone em uma solicitação de [operação do SetTelephoneAccessFolderEmail (serviço da Web da um)](settelephoneaccessfolderemail-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="fb468-104">The **base64FolderId** element contains the identifier of the folder to specify as the default e-mail folder from which Unified Messaging reads messages over the telephone in a [SetTelephoneAccessFolderEmail operation (UM web service)](settelephoneaccessfolderemail-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="fb468-105">SetTelephoneAccessFolderEmail (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="fb468-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="fb468-106">base64FolderId (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="fb468-106">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 <span data-ttu-id="fb468-107">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="fb468-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb468-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fb468-108">Attributes and elements</span></span>

<span data-ttu-id="fb468-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fb468-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb468-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="fb468-110">Attributes</span></span>

<span data-ttu-id="fb468-111">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="fb468-111">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb468-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fb468-112">Child elements</span></span>

<span data-ttu-id="fb468-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fb468-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fb468-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fb468-114">Parent elements</span></span>

|<span data-ttu-id="fb468-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fb468-115">**Element**</span></span>|<span data-ttu-id="fb468-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fb468-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb468-117">SetTelephoneAccessFolderEmail (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="fb468-117">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="fb468-118">Define a solicitação para definir a pasta de email de acesso telefônico.</span><span class="sxs-lookup"><span data-stu-id="fb468-118">Defines request to set the telephone access e-mail folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fb468-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="fb468-119">Text value</span></span>

<span data-ttu-id="fb468-120">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb468-120">A text value is required.</span></span> <span data-ttu-id="fb468-121">O valor de texto representa a ID de MAPI da pasta.</span><span class="sxs-lookup"><span data-stu-id="fb468-121">The text value represents the MAPI ID of the folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fb468-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="fb468-122">Remarks</span></span>

<span data-ttu-id="fb468-123">Para definir a pasta de email de acesso telefônico, use a [operação SetTelephoneAccessFolderEmail (serviço Web da um)](settelephoneaccessfolderemail-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="fb468-123">To set the telephone access e-mail folder, use the [SetTelephoneAccessFolderEmail operation (UM web service)](settelephoneaccessfolderemail-operation-um-web-service.md).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb468-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fb468-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb468-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="fb468-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fb468-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fb468-126">Schema Name</span></span>  <br/> |<span data-ttu-id="fb468-127">Mensagens</span><span class="sxs-lookup"><span data-stu-id="fb468-127">Messages</span></span>  <br/> |
|<span data-ttu-id="fb468-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fb468-128">Validation File</span></span>  <br/> |<span data-ttu-id="fb468-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fb468-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fb468-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fb468-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="fb468-131">False</span><span class="sxs-lookup"><span data-stu-id="fb468-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb468-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="fb468-132">See also</span></span>



[<span data-ttu-id="fb468-133">SetTelephoneAccessFolderEmail (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="fb468-133">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="fb468-134">Operação SetTelephoneAccessFolderEmail (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="fb468-134">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[<span data-ttu-id="fb468-135">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="fb468-135">FindFolder operation</span></span>](findfolder-operation.md)
  
[<span data-ttu-id="fb468-136">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="fb468-136">FindItem operation</span></span>](finditem-operation.md)

