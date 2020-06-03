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
description: O elemento GetSharingMetadata define uma solicitação para obter um token de autenticação opaco que identifica o convite de compartilhamento. Este elemento é o elemento base para a operação GetSharingMetadata.
ms.openlocfilehash: 406908e566d6d4249003b1a19a9ce79b8b328c4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530843"
---
# <a name="getsharingmetadata"></a><span data-ttu-id="d6c94-104">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="d6c94-104">GetSharingMetadata</span></span>

<span data-ttu-id="d6c94-105">O elemento **GetSharingMetadata** define uma solicitação para obter um token de autenticação opaco que identifica o convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="d6c94-105">The **GetSharingMetadata** element defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span> <span data-ttu-id="d6c94-106">Este elemento é o elemento base para a [operação GetSharingMetadata](getsharingmetadata-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d6c94-106">This element is the base element for the [GetSharingMetadata operation](getsharingmetadata-operation.md).</span></span>
  
```XML
<GetSharingMetadata>
   <IdOfFolderToShare/>
   <SenderSmtpAddress/>
   <Recipients/>
</GetSharingMetadata>
```

 <span data-ttu-id="d6c94-107">**GetSharingMetadataType**</span><span class="sxs-lookup"><span data-stu-id="d6c94-107">**GetSharingMetadataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6c94-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d6c94-108">Attributes and elements</span></span>

<span data-ttu-id="d6c94-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d6c94-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6c94-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="d6c94-110">Attributes</span></span>

<span data-ttu-id="d6c94-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6c94-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6c94-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d6c94-112">Child elements</span></span>

|<span data-ttu-id="d6c94-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d6c94-113">**Element**</span></span>|<span data-ttu-id="d6c94-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d6c94-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6c94-115">IdOfFolderToShare</span><span class="sxs-lookup"><span data-stu-id="d6c94-115">IdOfFolderToShare</span></span>](idoffoldertoshare.md) <br/> |<span data-ttu-id="d6c94-116">Representa o identificador da pasta no servidor que será compartilhado.</span><span class="sxs-lookup"><span data-stu-id="d6c94-116">Represents the identifier of the folder on the server that will be shared.</span></span> <span data-ttu-id="d6c94-117">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6c94-117">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="d6c94-118">SenderSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="d6c94-118">SenderSmtpAddress</span></span>](sendersmtpaddress.md) <br/> |<span data-ttu-id="d6c94-119">Representa o endereço de email SMTP que corresponde à caixa de correio que contém a pasta identificada pelo elemento [IdOfFolderToShare](idoffoldertoshare.md) .</span><span class="sxs-lookup"><span data-stu-id="d6c94-119">Represents the SMTP email address that corresponds to the mailbox that contains the folder that is identified by the [IdOfFolderToShare](idoffoldertoshare.md) element.</span></span> <span data-ttu-id="d6c94-120">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6c94-120">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="d6c94-121">Destinatários (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="d6c94-121">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="d6c94-122">Representa os endereços de email SMTP de uma ou mais entidades que terão acesso aos dados na pasta identificada pelo elemento [IdOfFolderToShare](idoffoldertoshare.md) .</span><span class="sxs-lookup"><span data-stu-id="d6c94-122">Represents the SMTP email addresses of one or more entities that will be granted access to the data in the folder that is identified by the [IdOfFolderToShare](idoffoldertoshare.md) element.</span></span> <span data-ttu-id="d6c94-123">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6c94-123">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d6c94-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d6c94-124">Parent elements</span></span>

<span data-ttu-id="d6c94-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6c94-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d6c94-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d6c94-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6c94-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="d6c94-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d6c94-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d6c94-128">Schema Name</span></span>  <br/> |<span data-ttu-id="d6c94-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d6c94-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d6c94-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d6c94-130">Validation File</span></span>  <br/> |<span data-ttu-id="d6c94-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d6c94-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d6c94-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d6c94-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="d6c94-133">False</span><span class="sxs-lookup"><span data-stu-id="d6c94-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d6c94-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="d6c94-134">See also</span></span>



[<span data-ttu-id="d6c94-135">Operação GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="d6c94-135">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="d6c94-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d6c94-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

