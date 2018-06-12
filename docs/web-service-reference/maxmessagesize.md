---
title: MaxMessageSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxMessageSize
api_type:
- schema
ms.assetid: bb98ac72-9409-4332-81bb-ee3bebb9a00e
description: O elemento MaxMessageSize representa o tamanho de mensagem máximo que um destinatário pode aceitar.
ms.openlocfilehash: 13a5679a03420655356269a7e8b5e22950724164
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824383"
---
# <a name="maxmessagesize"></a><span data-ttu-id="9c6c2-103">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="9c6c2-103">MaxMessageSize</span></span>

<span data-ttu-id="9c6c2-104">O elemento **MaxMessageSize** representa o tamanho de mensagem máximo que um destinatário pode aceitar.</span><span class="sxs-lookup"><span data-stu-id="9c6c2-104">The **MaxMessageSize** element represents the maximum message size a recipient can accept.</span></span> 
  
```XML
<MaxMessageSize/>
```

 <span data-ttu-id="9c6c2-105">**int**</span><span class="sxs-lookup"><span data-stu-id="9c6c2-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c6c2-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9c6c2-106">Attributes and elements</span></span>

<span data-ttu-id="9c6c2-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9c6c2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c6c2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9c6c2-108">Attributes</span></span>

<span data-ttu-id="9c6c2-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9c6c2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c6c2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9c6c2-110">Child elements</span></span>

<span data-ttu-id="9c6c2-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9c6c2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9c6c2-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9c6c2-112">Parent elements</span></span>

|<span data-ttu-id="9c6c2-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9c6c2-113">**Element**</span></span>|<span data-ttu-id="9c6c2-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9c6c2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c6c2-115">Dicas de email</span><span class="sxs-lookup"><span data-stu-id="9c6c2-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="9c6c2-116">Representa os valores para os vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="9c6c2-116">Represents values for various types of mail tips.</span></span>  <br/> |
|[<span data-ttu-id="9c6c2-117">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="9c6c2-117">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="9c6c2-118">Contém informações de configuração de serviço para o serviço de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="9c6c2-118">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9c6c2-119">Text value</span><span class="sxs-lookup"><span data-stu-id="9c6c2-119">Text value</span></span>

<span data-ttu-id="9c6c2-120">O valor de texto é um inteiro que representa o tamanho máximo da mensagem um destinatário pode aceitar.</span><span class="sxs-lookup"><span data-stu-id="9c6c2-120">The text value is an integer that represents the maximum message size a recipient can accept.</span></span> <span data-ttu-id="9c6c2-121">Esse valor pode ser medido em quilobytes ou em megabytes.</span><span class="sxs-lookup"><span data-stu-id="9c6c2-121">This value can be measured in kilobytes or megabytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9c6c2-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="9c6c2-122">Remarks</span></span>

<span data-ttu-id="9c6c2-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c6c2-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c6c2-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9c6c2-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c6c2-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="9c6c2-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9c6c2-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9c6c2-126">Schema Name</span></span>  <br/> |<span data-ttu-id="9c6c2-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9c6c2-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="9c6c2-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9c6c2-128">Validation File</span></span>  <br/> |<span data-ttu-id="9c6c2-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9c6c2-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9c6c2-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9c6c2-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="9c6c2-131">False</span><span class="sxs-lookup"><span data-stu-id="9c6c2-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9c6c2-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="9c6c2-132">See also</span></span>



- [<span data-ttu-id="9c6c2-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9c6c2-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

