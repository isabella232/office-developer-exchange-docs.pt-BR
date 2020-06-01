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
description: O elemento MaxMessageSize representa o tamanho máximo de mensagem que um destinatário pode aceitar.
ms.openlocfilehash: 727eed38a129800b7d38aa49c41cdacfa13e7a36
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468408"
---
# <a name="maxmessagesize"></a><span data-ttu-id="03b04-103">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="03b04-103">MaxMessageSize</span></span>

<span data-ttu-id="03b04-104">O elemento **MaxMessageSize** representa o tamanho máximo de mensagem que um destinatário pode aceitar.</span><span class="sxs-lookup"><span data-stu-id="03b04-104">The **MaxMessageSize** element represents the maximum message size a recipient can accept.</span></span> 
  
```XML
<MaxMessageSize/>
```

 <span data-ttu-id="03b04-105">**int**</span><span class="sxs-lookup"><span data-stu-id="03b04-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="03b04-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="03b04-106">Attributes and elements</span></span>

<span data-ttu-id="03b04-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="03b04-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03b04-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="03b04-108">Attributes</span></span>

<span data-ttu-id="03b04-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03b04-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03b04-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="03b04-110">Child elements</span></span>

<span data-ttu-id="03b04-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="03b04-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="03b04-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="03b04-112">Parent elements</span></span>

|<span data-ttu-id="03b04-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="03b04-113">**Element**</span></span>|<span data-ttu-id="03b04-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="03b04-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03b04-115">Dicas de Email</span><span class="sxs-lookup"><span data-stu-id="03b04-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="03b04-116">Representa valores de vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="03b04-116">Represents values for various types of mail tips.</span></span>  <br/> |
|[<span data-ttu-id="03b04-117">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="03b04-117">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="03b04-118">Contém informações de configuração de serviço para o serviço de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="03b04-118">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="03b04-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="03b04-119">Text value</span></span>

<span data-ttu-id="03b04-120">O valor de texto é um inteiro que representa o tamanho máximo de mensagem que um destinatário pode aceitar.</span><span class="sxs-lookup"><span data-stu-id="03b04-120">The text value is an integer that represents the maximum message size a recipient can accept.</span></span> <span data-ttu-id="03b04-121">Esse valor pode ser medido em kilobytes ou megabytes.</span><span class="sxs-lookup"><span data-stu-id="03b04-121">This value can be measured in kilobytes or megabytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="03b04-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="03b04-122">Remarks</span></span>

<span data-ttu-id="03b04-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="03b04-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03b04-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="03b04-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03b04-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="03b04-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="03b04-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="03b04-126">Schema Name</span></span>  <br/> |<span data-ttu-id="03b04-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="03b04-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="03b04-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="03b04-128">Validation File</span></span>  <br/> |<span data-ttu-id="03b04-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="03b04-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="03b04-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="03b04-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="03b04-131">False</span><span class="sxs-lookup"><span data-stu-id="03b04-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03b04-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="03b04-132">See also</span></span>



- [<span data-ttu-id="03b04-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="03b04-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

