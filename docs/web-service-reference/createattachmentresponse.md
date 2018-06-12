---
title: CreateAttachmentResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachmentResponse
api_type:
- schema
ms.assetid: cf6bd8bb-5317-4a03-bd75-297dd359b5da
description: O elemento de CreateAttachmentResponse define uma resposta a uma solicitação de CreateAttachment.
ms.openlocfilehash: dfc86516c5737296bc32330583fa63c36e9e63a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751566"
---
# <a name="createattachmentresponse"></a><span data-ttu-id="ee44e-103">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="ee44e-103">CreateAttachmentResponse</span></span>

<span data-ttu-id="ee44e-104">O elemento de **CreateAttachmentResponse** define uma resposta a uma solicitação de CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="ee44e-104">The **CreateAttachmentResponse** element defines a response to a CreateAttachment request.</span></span> 
  
```xml
<CreateAttachmentResponse>
   <ResponseMessages/>
</CreateAttachmentResponse>
```

 <span data-ttu-id="ee44e-105">**CreateAttachmentResponseType**</span><span class="sxs-lookup"><span data-stu-id="ee44e-105">**CreateAttachmentResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ee44e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ee44e-106">Attributes and elements</span></span>

<span data-ttu-id="ee44e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ee44e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ee44e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ee44e-108">Attributes</span></span>

<span data-ttu-id="ee44e-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ee44e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ee44e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ee44e-110">Child elements</span></span>

|<span data-ttu-id="ee44e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ee44e-111">**Element**</span></span>|<span data-ttu-id="ee44e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ee44e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee44e-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ee44e-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ee44e-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee44e-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ee44e-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ee44e-115">Parent elements</span></span>

<span data-ttu-id="ee44e-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ee44e-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ee44e-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="ee44e-117">Remarks</span></span>

<span data-ttu-id="ee44e-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="ee44e-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ee44e-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ee44e-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ee44e-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="ee44e-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ee44e-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ee44e-121">Schema name</span></span>  <br/> |<span data-ttu-id="ee44e-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ee44e-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ee44e-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ee44e-123">Validation file</span></span>  <br/> |<span data-ttu-id="ee44e-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ee44e-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ee44e-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ee44e-125">Can be empty</span></span>  <br/> |<span data-ttu-id="ee44e-126">False</span><span class="sxs-lookup"><span data-stu-id="ee44e-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ee44e-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="ee44e-127">See also</span></span>



[<span data-ttu-id="ee44e-128">Operação CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="ee44e-128">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="ee44e-129">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="ee44e-129">CreateAttachment</span></span>](createattachment.md)


- [<span data-ttu-id="ee44e-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ee44e-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

