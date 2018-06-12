---
title: ServerReplyWithMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServerReplyWithMessage
api_type:
- schema
ms.assetid: 113c6ff2-9592-44f0-b542-54e4d5122ccb
description: O elemento ServerReplyWithMessage indica a identificação da mensagem modelo que deve ser enviado como uma resposta às mensagens de entrada.
ms.openlocfilehash: f2d927ae18ac68523d4cdd173f0474fbbeb36c98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825390"
---
# <a name="serverreplywithmessage"></a><span data-ttu-id="1c08d-103">ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="1c08d-103">ServerReplyWithMessage</span></span>

<span data-ttu-id="1c08d-104">O elemento **ServerReplyWithMessage** indica a identificação da mensagem modelo que deve ser enviado como uma resposta às mensagens de entrada.</span><span class="sxs-lookup"><span data-stu-id="1c08d-104">The **ServerReplyWithMessage** element indicates the ID of the template message that is to be sent as a reply to incoming messages.</span></span> 
  
```XML
<ServerReplyWithMessage>
    <ItemId>
</ServerReplyWithMessage>
```

 <span data-ttu-id="1c08d-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="1c08d-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1c08d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1c08d-106">Attributes and elements</span></span>

<span data-ttu-id="1c08d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1c08d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c08d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1c08d-108">Attributes</span></span>

<span data-ttu-id="1c08d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1c08d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1c08d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1c08d-110">Child elements</span></span>

|<span data-ttu-id="1c08d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1c08d-111">**Element**</span></span>|<span data-ttu-id="1c08d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1c08d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c08d-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="1c08d-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="1c08d-114">Representa o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1c08d-114">Represents the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1c08d-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1c08d-115">Parent elements</span></span>

|<span data-ttu-id="1c08d-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1c08d-116">**Element**</span></span>|<span data-ttu-id="1c08d-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1c08d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c08d-118">Ações</span><span class="sxs-lookup"><span data-stu-id="1c08d-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="1c08d-119">Representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.</span><span class="sxs-lookup"><span data-stu-id="1c08d-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1c08d-120">Text value</span><span class="sxs-lookup"><span data-stu-id="1c08d-120">Text value</span></span>

<span data-ttu-id="1c08d-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1c08d-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1c08d-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="1c08d-122">Remarks</span></span>

<span data-ttu-id="1c08d-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1c08d-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1c08d-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1c08d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1c08d-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="1c08d-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1c08d-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1c08d-126">Schema Name</span></span>  <br/> |<span data-ttu-id="1c08d-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="1c08d-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1c08d-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1c08d-128">Validation File</span></span>  <br/> |<span data-ttu-id="1c08d-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1c08d-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1c08d-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1c08d-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="1c08d-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="1c08d-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1c08d-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="1c08d-132">See also</span></span>



- [<span data-ttu-id="1c08d-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1c08d-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

