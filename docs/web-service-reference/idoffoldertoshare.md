---
title: IdOfFolderToShare
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IdOfFolderToShare
api_type:
- schema
ms.assetid: 199d1839-f061-4070-a977-874b0c08e5be
description: O elemento IdOfFolderToShare representa o identificador da pasta no servidor que será compartilhado.
ms.openlocfilehash: 93a4740d9adefbb35aae071f0a6bfcb4b2021b4d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457624"
---
# <a name="idoffoldertoshare"></a><span data-ttu-id="cba94-103">IdOfFolderToShare</span><span class="sxs-lookup"><span data-stu-id="cba94-103">IdOfFolderToShare</span></span>

<span data-ttu-id="cba94-104">O elemento **IdOfFolderToShare** representa o identificador da pasta no servidor que será compartilhado.</span><span class="sxs-lookup"><span data-stu-id="cba94-104">The **IdOfFolderToShare** element represents the identifier of the folder on the server that will be shared.</span></span> 
  
```
<IdOfFolderToShare Id="" ChangeKey="" />
```

 <span data-ttu-id="cba94-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="cba94-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cba94-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cba94-106">Attributes and elements</span></span>

<span data-ttu-id="cba94-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cba94-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cba94-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cba94-108">Attributes</span></span>

|<span data-ttu-id="cba94-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="cba94-109">**Attribute**</span></span>|<span data-ttu-id="cba94-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cba94-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cba94-111">Id</span><span class="sxs-lookup"><span data-stu-id="cba94-111">Id</span></span>  <br/> |<span data-ttu-id="cba94-112">Contém uma cadeia de caracteres que identifica uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cba94-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="cba94-113">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="cba94-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="cba94-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="cba94-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="cba94-115">Contém uma cadeia de caracteres que identifica uma versão de uma pasta identificada pelo atributo ID.</span><span class="sxs-lookup"><span data-stu-id="cba94-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="cba94-116">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="cba94-116">This attribute is optional.</span></span> <span data-ttu-id="cba94-117">Use este atributo para certificar-se de que a versão correta de uma pasta é usada.</span><span class="sxs-lookup"><span data-stu-id="cba94-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cba94-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cba94-118">Child elements</span></span>

<span data-ttu-id="cba94-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cba94-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cba94-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cba94-120">Parent elements</span></span>

|<span data-ttu-id="cba94-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cba94-121">**Element**</span></span>|<span data-ttu-id="cba94-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cba94-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cba94-123">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="cba94-123">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="cba94-124">Define uma solicitação para obter um token de autenticação opaco que identifica o convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="cba94-124">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cba94-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="cba94-125">Remarks</span></span>

<span data-ttu-id="cba94-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="cba94-126">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cba94-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cba94-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cba94-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="cba94-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cba94-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cba94-129">Schema Name</span></span>  <br/> |<span data-ttu-id="cba94-130">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="cba94-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cba94-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cba94-131">Validation File</span></span>  <br/> |<span data-ttu-id="cba94-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cba94-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cba94-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cba94-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="cba94-134">False</span><span class="sxs-lookup"><span data-stu-id="cba94-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cba94-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="cba94-135">See also</span></span>



[<span data-ttu-id="cba94-136">Operação GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="cba94-136">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="cba94-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cba94-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

