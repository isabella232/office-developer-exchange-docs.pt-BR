---
title: ShowExternalRecipientCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ShowExternalRecipientCount
api_type:
- schema
ms.assetid: db28dbcb-d051-4e5c-a9c2-4b8d5149b4e1
description: O elemento de ShowExternalRecipientCount indica se os consumidores da operação GetMailTips têm que mostrar as dicas de email que indicam o número de destinatários externos ao qual uma mensagem é endereçada.
ms.openlocfilehash: 1fd3ceb629689c560dc60afe01f0413602f79a0d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825491"
---
# <a name="showexternalrecipientcount"></a><span data-ttu-id="15391-103">ShowExternalRecipientCount</span><span class="sxs-lookup"><span data-stu-id="15391-103">ShowExternalRecipientCount</span></span>

<span data-ttu-id="15391-104">O elemento de **ShowExternalRecipientCount** indica se os consumidores da [operação GetMailTips](getmailtips-operation.md) têm que mostrar as dicas de email que indicam o número de destinatários externos ao qual uma mensagem é endereçada.</span><span class="sxs-lookup"><span data-stu-id="15391-104">The **ShowExternalRecipientCount** element indicates whether consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> 
  
```XML
<ShowExternalRecipientCount>true | false</ShowExternalRecipientCount>
```

 <span data-ttu-id="15391-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="15391-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="15391-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="15391-106">Attributes and elements</span></span>

<span data-ttu-id="15391-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="15391-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15391-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="15391-108">Attributes</span></span>

<span data-ttu-id="15391-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="15391-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15391-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="15391-110">Child elements</span></span>

<span data-ttu-id="15391-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="15391-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="15391-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="15391-112">Parent elements</span></span>

|<span data-ttu-id="15391-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="15391-113">**Element**</span></span>|<span data-ttu-id="15391-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="15391-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15391-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="15391-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="15391-116">Contém informações de configuração de serviço para o serviço de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="15391-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="15391-117">Text value</span><span class="sxs-lookup"><span data-stu-id="15391-117">Text value</span></span>

<span data-ttu-id="15391-118">O valor de texto deste elemento é **true** se os consumidores da [operação GetMailTips](getmailtips-operation.md) tem que mostrar as dicas de email que indicam o número de destinatários externos ao qual uma mensagem é endereçada.</span><span class="sxs-lookup"><span data-stu-id="15391-118">The text value of this element is **true** if consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> <span data-ttu-id="15391-119">O valor é **false** se não tiver os consumidores da [operação GetMailTips](getmailtips-operation.md) mostrar as dicas de email que indicam o número de destinatários externos ao qual uma mensagem é endereçada.</span><span class="sxs-lookup"><span data-stu-id="15391-119">The value is **false** if consumers of the [GetMailTips operation](getmailtips-operation.md) do not have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="15391-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="15391-120">Remarks</span></span>

<span data-ttu-id="15391-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="15391-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15391-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="15391-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15391-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="15391-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="15391-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="15391-124">Schema Name</span></span>  <br/> |<span data-ttu-id="15391-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="15391-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="15391-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="15391-126">Validation File</span></span>  <br/> |<span data-ttu-id="15391-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="15391-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="15391-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="15391-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="15391-129">False</span><span class="sxs-lookup"><span data-stu-id="15391-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="15391-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="15391-130">See also</span></span>



[<span data-ttu-id="15391-131">Operação GetMailTips</span><span class="sxs-lookup"><span data-stu-id="15391-131">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="15391-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="15391-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

