---
title: GetSharingMetadata
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadata
api_type:
- schema
ms.assetid: b609ee26-6d28-4559-81b6-b8e8d4759a23
description: O elemento de GetSharingMetadata define uma solicitação para obter um token de autenticação opaco que identifica o convite de compartilhamento. Este elemento é a base para a operação GetSharingMetadata.
ms.openlocfilehash: 5283d35e11350ef10ed8cc01527e787ef54be927
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823677"
---
# <a name="getsharingmetadata"></a><span data-ttu-id="c1e10-104">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="c1e10-104">GetSharingMetadata</span></span>

<span data-ttu-id="c1e10-105">O elemento de **GetSharingMetadata** define uma solicitação para obter um token de autenticação opaco que identifica o convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="c1e10-105">The **GetSharingMetadata** element defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span> <span data-ttu-id="c1e10-106">Este elemento é a base para a [operação GetSharingMetadata](getsharingmetadata-operation.md).</span><span class="sxs-lookup"><span data-stu-id="c1e10-106">This element is the base element for the [GetSharingMetadata operation](getsharingmetadata-operation.md).</span></span>
  
```XML
<GetSharingMetadata>
   <IdOfFolderToShare/>
   <SenderSmtpAddress/>
   <Recipients/>
</GetSharingMetadata>
```

 <span data-ttu-id="c1e10-107">**GetSharingMetadataType**</span><span class="sxs-lookup"><span data-stu-id="c1e10-107">**GetSharingMetadataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c1e10-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c1e10-108">Attributes and elements</span></span>

<span data-ttu-id="c1e10-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c1e10-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c1e10-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="c1e10-110">Attributes</span></span>

<span data-ttu-id="c1e10-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c1e10-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c1e10-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c1e10-112">Child elements</span></span>

|<span data-ttu-id="c1e10-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c1e10-113">**Element**</span></span>|<span data-ttu-id="c1e10-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c1e10-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1e10-115">IdOfFolderToShare</span><span class="sxs-lookup"><span data-stu-id="c1e10-115">IdOfFolderToShare</span></span>](idoffoldertoshare.md) <br/> |<span data-ttu-id="c1e10-116">Representa o identificador da pasta no servidor que será compartilhado.</span><span class="sxs-lookup"><span data-stu-id="c1e10-116">Represents the identifier of the folder on the server that will be shared.</span></span> <span data-ttu-id="c1e10-117">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1e10-117">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c1e10-118">SenderSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="c1e10-118">SenderSmtpAddress</span></span>](sendersmtpaddress.md) <br/> |<span data-ttu-id="c1e10-119">Representa o endereço de email SMTP que corresponde à caixa de correio que contém a pasta que é identificada pelo elemento [IdOfFolderToShare](idoffoldertoshare.md) .</span><span class="sxs-lookup"><span data-stu-id="c1e10-119">Represents the SMTP email address that corresponds to the mailbox that contains the folder that is identified by the [IdOfFolderToShare](idoffoldertoshare.md) element.</span></span> <span data-ttu-id="c1e10-120">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1e10-120">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c1e10-121">Destinatários (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="c1e10-121">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="c1e10-122">Representa os endereços de email SMTP de uma ou mais entidades que receberão acesso aos dados na pasta que é identificado pelo elemento [IdOfFolderToShare](idoffoldertoshare.md) .</span><span class="sxs-lookup"><span data-stu-id="c1e10-122">Represents the SMTP email addresses of one or more entities that will be granted access to the data in the folder that is identified by the [IdOfFolderToShare](idoffoldertoshare.md) element.</span></span> <span data-ttu-id="c1e10-123">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1e10-123">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c1e10-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c1e10-124">Parent elements</span></span>

<span data-ttu-id="c1e10-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c1e10-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c1e10-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c1e10-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c1e10-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="c1e10-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c1e10-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c1e10-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c1e10-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c1e10-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c1e10-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c1e10-130">Validation File</span></span>  <br/> |<span data-ttu-id="c1e10-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c1e10-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c1e10-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c1e10-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c1e10-133">False</span><span class="sxs-lookup"><span data-stu-id="c1e10-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c1e10-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="c1e10-134">See also</span></span>



[<span data-ttu-id="c1e10-135">Operação GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="c1e10-135">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="c1e10-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c1e10-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

