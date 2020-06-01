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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467316"
---
# <a name="settelephoneaccessfolderemail-um-web-service"></a><span data-ttu-id="ea9f4-103">SetTelephoneAccessFolderEmail (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="ea9f4-103">SetTelephoneAccessFolderEmail (UM web service)</span></span>

<span data-ttu-id="ea9f4-104">O elemento **SetTelephoneAccessFolderEmail** define uma solicitação para definir a pasta de email padrão a partir da qual a Unificação de mensagens lerá as mensagens por telefone.</span><span class="sxs-lookup"><span data-stu-id="ea9f4-104">The **SetTelephoneAccessFolderEmail** element defines a request to set the default e-mail folder from which Unified Messaging will read messages over the telephone.</span></span> 
  
[<span data-ttu-id="ea9f4-105">SetTelephoneAccessFolderEmail (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="ea9f4-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
```xml
<SetTelephoneAccessFolderEmail>
  <base64FolderId>   </base64FolderId>
</SetTelephoneAccessFolderEmail>
```

 <span data-ttu-id="ea9f4-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="ea9f4-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea9f4-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ea9f4-107">Attributes and elements</span></span>

<span data-ttu-id="ea9f4-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ea9f4-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea9f4-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="ea9f4-109">Attributes</span></span>

<span data-ttu-id="ea9f4-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea9f4-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea9f4-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ea9f4-111">Child elements</span></span>

|<span data-ttu-id="ea9f4-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ea9f4-112">**Element**</span></span>|<span data-ttu-id="ea9f4-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ea9f4-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea9f4-114">base64FolderId (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="ea9f4-114">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md) <br/> |<span data-ttu-id="ea9f4-115">O identificador da pasta de email.</span><span class="sxs-lookup"><span data-stu-id="ea9f4-115">The identifier of the e-mail folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ea9f4-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ea9f4-116">Parent elements</span></span>

<span data-ttu-id="ea9f4-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea9f4-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ea9f4-118">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ea9f4-118">Text value</span></span>

<span data-ttu-id="ea9f4-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea9f4-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea9f4-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ea9f4-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea9f4-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="ea9f4-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ea9f4-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ea9f4-122">Schema Name</span></span>  <br/> |<span data-ttu-id="ea9f4-123">Mensagens</span><span class="sxs-lookup"><span data-stu-id="ea9f4-123">Messages</span></span>  <br/> |
|<span data-ttu-id="ea9f4-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ea9f4-124">Validation File</span></span>  <br/> |<span data-ttu-id="ea9f4-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ea9f4-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ea9f4-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ea9f4-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="ea9f4-127">False</span><span class="sxs-lookup"><span data-stu-id="ea9f4-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea9f4-128">Confira também</span><span class="sxs-lookup"><span data-stu-id="ea9f4-128">See also</span></span>



[<span data-ttu-id="ea9f4-129">Operação SetTelephoneAccessFolderEmail (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="ea9f4-129">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)

