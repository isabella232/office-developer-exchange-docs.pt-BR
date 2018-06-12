---
title: GetSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: ed5bb61f-89c7-4baa-83ee-30f06a49ff9b
description: O elemento de GetSharingFolder define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada. É o elemento de base para a operação GetSharingFolder.
ms.openlocfilehash: 7c2f31aa27c1cbde6cdad2b41a341916b4bed2ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823669"
---
# <a name="getsharingfolder"></a><span data-ttu-id="27e9d-104">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="27e9d-104">GetSharingFolder</span></span>

<span data-ttu-id="27e9d-105">O elemento de **GetSharingFolder** define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada.</span><span class="sxs-lookup"><span data-stu-id="27e9d-105">The **GetSharingFolder** element defines a request to get the local folder identifier of a specified shared folder.</span></span> <span data-ttu-id="27e9d-106">É o elemento de base para a [operação GetSharingFolder](getsharingfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="27e9d-106">It is the base element for the [GetSharingFolder operation](getsharingfolder-operation.md).</span></span>
  
```xml
<GetSharingFolder>   <SmtpAddress/>   <DataType/>   <SharedFolderId/></GetSharingFolder>
```

 <span data-ttu-id="27e9d-107">**GetSharingFolderType**</span><span class="sxs-lookup"><span data-stu-id="27e9d-107">**GetSharingFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27e9d-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="27e9d-108">Attributes and elements</span></span>

<span data-ttu-id="27e9d-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="27e9d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27e9d-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="27e9d-110">Attributes</span></span>

<span data-ttu-id="27e9d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="27e9d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27e9d-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="27e9d-112">Child elements</span></span>

|<span data-ttu-id="27e9d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="27e9d-113">**Element**</span></span>|<span data-ttu-id="27e9d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="27e9d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27e9d-115">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="27e9d-115">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="27e9d-116">Representa o endereço de email SMTP da outra na relação de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="27e9d-116">Represents the SMTP e-mail address of the other party in the sharing relationship.</span></span> <span data-ttu-id="27e9d-117">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27e9d-117">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="27e9d-118">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="27e9d-118">DataType</span></span>](datatype.md) <br/> |<span data-ttu-id="27e9d-119">Descreve o tipo de dados que são compartilhados por uma pasta compartilhada.</span><span class="sxs-lookup"><span data-stu-id="27e9d-119">Describes the type of data that is shared by a shared folder.</span></span> <span data-ttu-id="27e9d-120">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="27e9d-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="27e9d-121">SharedFolderId</span><span class="sxs-lookup"><span data-stu-id="27e9d-121">SharedFolderId</span></span>](sharedfolderid.md) <br/> |<span data-ttu-id="27e9d-122">Representa o identificador da pasta compartilhada cujo identificador de pasta local deve ser retornado.</span><span class="sxs-lookup"><span data-stu-id="27e9d-122">Represents the identifier of the shared folder whose local folder identifier should be returned.</span></span> <span data-ttu-id="27e9d-123">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="27e9d-123">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="27e9d-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="27e9d-124">Parent elements</span></span>

<span data-ttu-id="27e9d-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="27e9d-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="27e9d-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="27e9d-126">Remarks</span></span>

<span data-ttu-id="27e9d-127">Um elemento GetSharingFolder deve conter um elemento [SmtpAddress](smtpaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="27e9d-127">A GetSharingFolder element must contain an [SmtpAddress](smtpaddress.md) element.</span></span> <span data-ttu-id="27e9d-128">Um elemento GetSharingFolder também deve conter um elemento [DataType](datatype.md) ou um elemento [SharedFolderId](sharedfolderid.md) , mas não pode conter ambos.</span><span class="sxs-lookup"><span data-stu-id="27e9d-128">A GetSharingFolder element must also contain either a [DataType](datatype.md) element or a [SharedFolderId](sharedfolderid.md) element, but cannot contain both.</span></span> 
  
<span data-ttu-id="27e9d-129">O esquema que descreve este elemento está localizado no diretório Virtual do IIS que hospeda o Exchange Web Services do computador que está executando o Microsoft Exchange Server que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="27e9d-129">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27e9d-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="27e9d-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27e9d-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="27e9d-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="27e9d-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="27e9d-132">Schema Name</span></span>  <br/> |<span data-ttu-id="27e9d-133">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="27e9d-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="27e9d-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="27e9d-134">Validation File</span></span>  <br/> |<span data-ttu-id="27e9d-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="27e9d-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="27e9d-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="27e9d-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="27e9d-137">False</span><span class="sxs-lookup"><span data-stu-id="27e9d-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27e9d-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="27e9d-138">See also</span></span>



[<span data-ttu-id="27e9d-139">Operação GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="27e9d-139">GetSharingFolder operation</span></span>](getsharingfolder-operation.md)


- [<span data-ttu-id="27e9d-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="27e9d-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

