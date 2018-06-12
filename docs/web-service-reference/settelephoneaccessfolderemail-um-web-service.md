---
title: SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetTelephoneAccessFolderEmail
api_type:
- schema
ms.assetid: 90759da7-6dba-499e-b8c8-e44a016b3198
description: O elemento de SetTelephoneAccessFolderEmail define uma solicitação para definir a pasta de email padrão do qual Unificação de mensagens lê as mensagens por telefone.
ms.openlocfilehash: e19f151e364411717d5129cbef8c5cc097689f89
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825461"
---
# <a name="settelephoneaccessfolderemail-um-web-service"></a><span data-ttu-id="6d8c4-103">SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="6d8c4-103">SetTelephoneAccessFolderEmail (UM web service)</span></span>

<span data-ttu-id="6d8c4-104">O elemento de **SetTelephoneAccessFolderEmail** define uma solicitação para definir a pasta de email padrão do qual Unificação de mensagens lê as mensagens por telefone.</span><span class="sxs-lookup"><span data-stu-id="6d8c4-104">The **SetTelephoneAccessFolderEmail** element defines a request to set the default e-mail folder from which Unified Messaging will read messages over the telephone.</span></span> 
  
[<span data-ttu-id="6d8c4-105">SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="6d8c4-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
```xml
<SetTelephoneAccessFolderEmail>
  <base64FolderId>   </base64FolderId>
</SetTelephoneAccessFolderEmail>
```

 <span data-ttu-id="6d8c4-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="6d8c4-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d8c4-107">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6d8c4-107">Attributes and elements</span></span>

<span data-ttu-id="6d8c4-108">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6d8c4-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d8c4-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="6d8c4-109">Attributes</span></span>

<span data-ttu-id="6d8c4-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6d8c4-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d8c4-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6d8c4-111">Child elements</span></span>

|<span data-ttu-id="6d8c4-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6d8c4-112">**Element**</span></span>|<span data-ttu-id="6d8c4-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6d8c4-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d8c4-114">base64FolderId (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="6d8c4-114">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md) <br/> |<span data-ttu-id="6d8c4-115">O identificador da pasta de email.</span><span class="sxs-lookup"><span data-stu-id="6d8c4-115">The identifier of the e-mail folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6d8c4-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6d8c4-116">Parent elements</span></span>

<span data-ttu-id="6d8c4-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6d8c4-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="6d8c4-118">Text value</span><span class="sxs-lookup"><span data-stu-id="6d8c4-118">Text value</span></span>

<span data-ttu-id="6d8c4-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6d8c4-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d8c4-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6d8c4-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d8c4-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="6d8c4-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6d8c4-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6d8c4-122">Schema Name</span></span>  <br/> |<span data-ttu-id="6d8c4-123">Mensagens</span><span class="sxs-lookup"><span data-stu-id="6d8c4-123">Messages</span></span>  <br/> |
|<span data-ttu-id="6d8c4-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6d8c4-124">Validation File</span></span>  <br/> |<span data-ttu-id="6d8c4-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6d8c4-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6d8c4-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6d8c4-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="6d8c4-127">False</span><span class="sxs-lookup"><span data-stu-id="6d8c4-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6d8c4-128">Ver também</span><span class="sxs-lookup"><span data-stu-id="6d8c4-128">See also</span></span>



[<span data-ttu-id="6d8c4-129">Operação de SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="6d8c4-129">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)

