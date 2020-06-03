---
title: EmptyFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c900be49-3c90-41aa-aba5-bcf1116ec2aa
description: O elemento EmptyFolderResponse define uma resposta a uma solicitação de operação EmptyFolder.
ms.openlocfilehash: 9b20df8c0b095870185aab14dbd1f7ff4fc47def
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530674"
---
# <a name="emptyfolderresponse"></a><span data-ttu-id="7150b-103">EmptyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="7150b-103">EmptyFolderResponse</span></span>

<span data-ttu-id="7150b-104">O elemento **EmptyFolderResponse** define uma resposta a uma solicitação de [operação EmptyFolder](emptyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7150b-104">The **EmptyFolderResponse** element defines a response to an [EmptyFolder operation](emptyfolder-operation.md) request.</span></span> 
  
```XML
<EmptyFolderResponse>
   <ResponseMessages/>
</EmptyFolderResponse>
```

 <span data-ttu-id="7150b-105">**EmptyFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="7150b-105">**EmptyFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7150b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="7150b-106">Attributes and elements</span></span>

<span data-ttu-id="7150b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7150b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7150b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7150b-108">Attributes</span></span>

<span data-ttu-id="7150b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7150b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7150b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7150b-110">Child elements</span></span>

|<span data-ttu-id="7150b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7150b-111">**Element**</span></span>|<span data-ttu-id="7150b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7150b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7150b-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7150b-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="7150b-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7150b-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7150b-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7150b-115">Parent elements</span></span>

<span data-ttu-id="7150b-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7150b-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7150b-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="7150b-117">Remarks</span></span>

<span data-ttu-id="7150b-118">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7150b-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7150b-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="7150b-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7150b-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="7150b-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7150b-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7150b-121">Schema name</span></span>  <br/> |<span data-ttu-id="7150b-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="7150b-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7150b-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7150b-123">Validation file</span></span>  <br/> |<span data-ttu-id="7150b-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7150b-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7150b-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="7150b-125">Can be empty</span></span>  <br/> |<span data-ttu-id="7150b-126">False</span><span class="sxs-lookup"><span data-stu-id="7150b-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7150b-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="7150b-127">See also</span></span>



[<span data-ttu-id="7150b-128">Operação EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="7150b-128">EmptyFolder operation</span></span>](emptyfolder-operation.md)
  
[<span data-ttu-id="7150b-129">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="7150b-129">EmptyFolder</span></span>](emptyfolder.md)


- [<span data-ttu-id="7150b-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7150b-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

