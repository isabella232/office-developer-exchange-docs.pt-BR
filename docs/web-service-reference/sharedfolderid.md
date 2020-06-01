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
description: O elemento SharedFolderId representa o identificador da pasta compartilhada para a qual o identificador de pasta local deve ser retornado por uma solicitação de operação GetSharingFolder.
ms.openlocfilehash: 546e148540708725bcf335f39bf69d193124d210
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466119"
---
# <a name="sharedfolderid"></a><span data-ttu-id="a0ee7-103">SharedFolderId</span><span class="sxs-lookup"><span data-stu-id="a0ee7-103">SharedFolderId</span></span>

<span data-ttu-id="a0ee7-104">O elemento **SharedFolderId** representa o identificador da pasta compartilhada para a qual o identificador de pasta local deve ser retornado por uma solicitação de [operação GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a0ee7-104">The **SharedFolderId** element represents the identifier of the shared folder the local folder identifier for which should be returned by a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
```xml
<SharedFolderId/>
```

 <span data-ttu-id="a0ee7-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="a0ee7-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0ee7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a0ee7-106">Attributes and elements</span></span>

<span data-ttu-id="a0ee7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a0ee7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0ee7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a0ee7-108">Attributes</span></span>

<span data-ttu-id="a0ee7-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0ee7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0ee7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a0ee7-110">Child elements</span></span>

<span data-ttu-id="a0ee7-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a0ee7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a0ee7-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a0ee7-112">Parent elements</span></span>

|<span data-ttu-id="a0ee7-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a0ee7-113">**Element**</span></span>|<span data-ttu-id="a0ee7-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a0ee7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0ee7-115">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="a0ee7-115">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="a0ee7-116">Define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada.</span><span class="sxs-lookup"><span data-stu-id="a0ee7-116">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a0ee7-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a0ee7-117">Text value</span></span>

<span data-ttu-id="a0ee7-118">O valor de texto é uma cadeia de caracteres que representa o identificador da pasta compartilhada para a qual o identificador de pasta local deve ser retornado por uma solicitação de [operação GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a0ee7-118">The text value is a string that represents the identifier of the shared folder the local folder identifier for which should be returned by a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a0ee7-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="a0ee7-119">Remarks</span></span>

<span data-ttu-id="a0ee7-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0ee7-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0ee7-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a0ee7-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0ee7-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="a0ee7-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a0ee7-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a0ee7-123">Schema Name</span></span>  <br/> |<span data-ttu-id="a0ee7-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a0ee7-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a0ee7-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a0ee7-125">Validation File</span></span>  <br/> |<span data-ttu-id="a0ee7-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a0ee7-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a0ee7-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a0ee7-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="a0ee7-128">False</span><span class="sxs-lookup"><span data-stu-id="a0ee7-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0ee7-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="a0ee7-129">See also</span></span>



[<span data-ttu-id="a0ee7-130">Operação GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="a0ee7-130">GetSharingFolder operation</span></span>](getsharingfolder-operation.md)


- [<span data-ttu-id="a0ee7-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a0ee7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

