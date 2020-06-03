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
description: O elemento ServerReplyWithMessage indica a ID da mensagem de modelo a ser enviada como uma resposta a mensagens de entrada.
ms.openlocfilehash: faaa054018a17be3ff59b9fc385b3d846d39c3f1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461972"
---
# <a name="serverreplywithmessage"></a><span data-ttu-id="fc9a3-103">ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="fc9a3-103">ServerReplyWithMessage</span></span>

<span data-ttu-id="fc9a3-104">O elemento **ServerReplyWithMessage** indica a ID da mensagem de modelo a ser enviada como uma resposta a mensagens de entrada.</span><span class="sxs-lookup"><span data-stu-id="fc9a3-104">The **ServerReplyWithMessage** element indicates the ID of the template message that is to be sent as a reply to incoming messages.</span></span> 
  
```XML
<ServerReplyWithMessage>
    <ItemId>
</ServerReplyWithMessage>
```

 <span data-ttu-id="fc9a3-105">**ItemIdtype**</span><span class="sxs-lookup"><span data-stu-id="fc9a3-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc9a3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fc9a3-106">Attributes and elements</span></span>

<span data-ttu-id="fc9a3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fc9a3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc9a3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fc9a3-108">Attributes</span></span>

<span data-ttu-id="fc9a3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc9a3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc9a3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fc9a3-110">Child elements</span></span>

|<span data-ttu-id="fc9a3-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fc9a3-111">**Element**</span></span>|<span data-ttu-id="fc9a3-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc9a3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc9a3-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="fc9a3-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="fc9a3-114">Representa o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc9a3-114">Represents the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fc9a3-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fc9a3-115">Parent elements</span></span>

|<span data-ttu-id="fc9a3-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fc9a3-116">**Element**</span></span>|<span data-ttu-id="fc9a3-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc9a3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc9a3-118">Actions</span><span class="sxs-lookup"><span data-stu-id="fc9a3-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="fc9a3-119">Representa o conjunto de ações que estão disponíveis para serem realizadas em uma mensagem quando as condições forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="fc9a3-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fc9a3-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="fc9a3-120">Text value</span></span>

<span data-ttu-id="fc9a3-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fc9a3-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fc9a3-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="fc9a3-122">Remarks</span></span>

<span data-ttu-id="fc9a3-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc9a3-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc9a3-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fc9a3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc9a3-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="fc9a3-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fc9a3-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fc9a3-126">Schema Name</span></span>  <br/> |<span data-ttu-id="fc9a3-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="fc9a3-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fc9a3-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fc9a3-128">Validation File</span></span>  <br/> |<span data-ttu-id="fc9a3-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fc9a3-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fc9a3-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fc9a3-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc9a3-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="fc9a3-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc9a3-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="fc9a3-132">See also</span></span>



- [<span data-ttu-id="fc9a3-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fc9a3-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

