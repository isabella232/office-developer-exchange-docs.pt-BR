---
title: SetTelephoneAccessFolderEmail (serviço Web da UM)
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
description: O elemento SetTelephoneAccessFolderEmail define uma solicitação para definir a pasta de email padrão a partir da qual a Unificação de mensagens lerá as mensagens por telefone.
ms.openlocfilehash: 806bdb1f0c7930a9e89555192aa32ad997716e7e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467316"
---
# <a name="settelephoneaccessfolderemail-um-web-service"></a><span data-ttu-id="458e7-103">SetTelephoneAccessFolderEmail (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="458e7-103">SetTelephoneAccessFolderEmail (UM web service)</span></span>

<span data-ttu-id="458e7-104">O elemento **SetTelephoneAccessFolderEmail** define uma solicitação para definir a pasta de email padrão a partir da qual a Unificação de mensagens lerá as mensagens por telefone.</span><span class="sxs-lookup"><span data-stu-id="458e7-104">The **SetTelephoneAccessFolderEmail** element defines a request to set the default e-mail folder from which Unified Messaging will read messages over the telephone.</span></span> 
  
[<span data-ttu-id="458e7-105">SetTelephoneAccessFolderEmail (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="458e7-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
```xml
<SetTelephoneAccessFolderEmail>
  <base64FolderId>   </base64FolderId>
</SetTelephoneAccessFolderEmail>
```

 <span data-ttu-id="458e7-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="458e7-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="458e7-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="458e7-107">Attributes and elements</span></span>

<span data-ttu-id="458e7-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="458e7-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="458e7-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="458e7-109">Attributes</span></span>

<span data-ttu-id="458e7-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="458e7-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="458e7-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="458e7-111">Child elements</span></span>

|<span data-ttu-id="458e7-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="458e7-112">**Element**</span></span>|<span data-ttu-id="458e7-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="458e7-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="458e7-114">base64FolderId (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="458e7-114">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md) <br/> |<span data-ttu-id="458e7-115">O identificador da pasta de email.</span><span class="sxs-lookup"><span data-stu-id="458e7-115">The identifier of the e-mail folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="458e7-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="458e7-116">Parent elements</span></span>

<span data-ttu-id="458e7-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="458e7-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="458e7-118">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="458e7-118">Text value</span></span>

<span data-ttu-id="458e7-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="458e7-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="458e7-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="458e7-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="458e7-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="458e7-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="458e7-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="458e7-122">Schema Name</span></span>  <br/> |<span data-ttu-id="458e7-123">Mensagens</span><span class="sxs-lookup"><span data-stu-id="458e7-123">Messages</span></span>  <br/> |
|<span data-ttu-id="458e7-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="458e7-124">Validation File</span></span>  <br/> |<span data-ttu-id="458e7-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="458e7-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="458e7-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="458e7-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="458e7-127">False</span><span class="sxs-lookup"><span data-stu-id="458e7-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="458e7-128">Confira também</span><span class="sxs-lookup"><span data-stu-id="458e7-128">See also</span></span>



[<span data-ttu-id="458e7-129">Operação SetTelephoneAccessFolderEmail (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="458e7-129">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)

