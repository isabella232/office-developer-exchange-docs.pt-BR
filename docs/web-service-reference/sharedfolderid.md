---
title: SharedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharedFolderId
api_type:
- schema
ms.assetid: 21181ba3-9626-4284-9717-0b1c16948e8f
description: O elemento SharedFolderId representa o identificador da pasta compartilhada o identificador de pasta local para o qual deve ser retornado por uma solicitação de operação GetSharingFolder.
ms.openlocfilehash: 6d4e541ef3cae89e413efa8cc5f1beaf651dc4dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825477"
---
# <a name="sharedfolderid"></a><span data-ttu-id="0d845-103">SharedFolderId</span><span class="sxs-lookup"><span data-stu-id="0d845-103">SharedFolderId</span></span>

<span data-ttu-id="0d845-104">O elemento **SharedFolderId** representa o identificador da pasta compartilhada o identificador de pasta local para o qual deve ser retornado por uma solicitação de [operação GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0d845-104">The **SharedFolderId** element represents the identifier of the shared folder the local folder identifier for which should be returned by a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
```xml
<SharedFolderId/>
```

 <span data-ttu-id="0d845-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="0d845-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d845-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0d845-106">Attributes and elements</span></span>

<span data-ttu-id="0d845-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0d845-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d845-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0d845-108">Attributes</span></span>

<span data-ttu-id="0d845-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0d845-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0d845-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0d845-110">Child elements</span></span>

<span data-ttu-id="0d845-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0d845-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0d845-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0d845-112">Parent elements</span></span>

|<span data-ttu-id="0d845-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0d845-113">**Element**</span></span>|<span data-ttu-id="0d845-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0d845-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d845-115">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="0d845-115">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="0d845-116">Define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada.</span><span class="sxs-lookup"><span data-stu-id="0d845-116">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0d845-117">Text value</span><span class="sxs-lookup"><span data-stu-id="0d845-117">Text value</span></span>

<span data-ttu-id="0d845-118">O valor de texto é uma cadeia de caracteres que representa o identificador da pasta compartilhada o identificador de pasta local para o qual deve ser retornado por uma solicitação de [operação GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0d845-118">The text value is a string that represents the identifier of the shared folder the local folder identifier for which should be returned by a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0d845-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="0d845-119">Remarks</span></span>

<span data-ttu-id="0d845-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d845-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d845-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0d845-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d845-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="0d845-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0d845-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0d845-123">Schema Name</span></span>  <br/> |<span data-ttu-id="0d845-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0d845-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0d845-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0d845-125">Validation File</span></span>  <br/> |<span data-ttu-id="0d845-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0d845-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0d845-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0d845-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="0d845-128">False</span><span class="sxs-lookup"><span data-stu-id="0d845-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0d845-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="0d845-129">See also</span></span>



[<span data-ttu-id="0d845-130">Operação GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="0d845-130">GetSharingFolder operation</span></span>](getsharingfolder-operation.md)


- [<span data-ttu-id="0d845-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0d845-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

