---
title: ServerHint
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServerHint
api_type:
- schema
ms.assetid: 5ac60472-a565-43d1-a5fb-8be0c9511f82
description: O elemento ServerHint representa o ponto de partida para rastrear uma mensagem em um site ou floresta remoto.
ms.openlocfilehash: 76a719901f4e4d1da67ce377ab8b73e4a4592dc4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461986"
---
# <a name="serverhint"></a><span data-ttu-id="c02bc-103">ServerHint</span><span class="sxs-lookup"><span data-stu-id="c02bc-103">ServerHint</span></span>

<span data-ttu-id="c02bc-104">O elemento **ServerHint** representa o ponto de partida para rastrear uma mensagem em um site ou floresta remoto.</span><span class="sxs-lookup"><span data-stu-id="c02bc-104">The **ServerHint** element represents the starting point for tracking a message in a remote site or forest.</span></span> 
  
```xml
<ServerHint/>
```

 <span data-ttu-id="c02bc-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="c02bc-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c02bc-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c02bc-106">Attributes and elements</span></span>

<span data-ttu-id="c02bc-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c02bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c02bc-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c02bc-108">Attributes</span></span>

<span data-ttu-id="c02bc-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c02bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c02bc-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c02bc-110">Child elements</span></span>

<span data-ttu-id="c02bc-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c02bc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c02bc-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c02bc-112">Parent elements</span></span>

|<span data-ttu-id="c02bc-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c02bc-113">**Element**</span></span>|<span data-ttu-id="c02bc-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c02bc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c02bc-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="c02bc-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="c02bc-116">Especifica critérios para os tipos de mensagens a serem encontradas.</span><span class="sxs-lookup"><span data-stu-id="c02bc-116">Specifies criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c02bc-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c02bc-117">Text value</span></span>

<span data-ttu-id="c02bc-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c02bc-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c02bc-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="c02bc-119">Remarks</span></span>

<span data-ttu-id="c02bc-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c02bc-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c02bc-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c02bc-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c02bc-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="c02bc-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c02bc-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c02bc-123">Schema Name</span></span>  <br/> |<span data-ttu-id="c02bc-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c02bc-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c02bc-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c02bc-125">Validation File</span></span>  <br/> |<span data-ttu-id="c02bc-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c02bc-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c02bc-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c02bc-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="c02bc-128">False</span><span class="sxs-lookup"><span data-stu-id="c02bc-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c02bc-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="c02bc-129">See also</span></span>



[<span data-ttu-id="c02bc-130">Operação FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="c02bc-130">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="c02bc-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c02bc-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

