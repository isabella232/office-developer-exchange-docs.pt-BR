---
title: UnsubscribeResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnsubscribeResponse
api_type:
- schema
ms.assetid: 125e0326-6522-42cd-b20e-6977e6fde249
description: O elemento de UnsubscribeResponse define uma resposta a uma solicitação de cancelamento da assinatura.
ms.openlocfilehash: a5d90a6631cba7f18da0261be52488c7f6793dcd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837866"
---
# <a name="unsubscriberesponse"></a><span data-ttu-id="f5621-103">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="f5621-103">UnsubscribeResponse</span></span>

<span data-ttu-id="f5621-104">O elemento de **UnsubscribeResponse** define uma resposta a uma solicitação de cancelamento da assinatura.</span><span class="sxs-lookup"><span data-stu-id="f5621-104">The **UnsubscribeResponse** element defines a response to an Unsubscribe request.</span></span> 
  
```xml
<UnsubscribeResponse>
   <ResponseMessages/>
</UnsubscribeResponse>
```

 <span data-ttu-id="f5621-105">**UnsubscribeResponseType**</span><span class="sxs-lookup"><span data-stu-id="f5621-105">**UnsubscribeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f5621-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f5621-106">Attributes and elements</span></span>

<span data-ttu-id="f5621-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f5621-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5621-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f5621-108">Attributes</span></span>

<span data-ttu-id="f5621-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f5621-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f5621-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f5621-110">Child elements</span></span>

|<span data-ttu-id="f5621-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f5621-111">**Element**</span></span>|<span data-ttu-id="f5621-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f5621-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5621-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f5621-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f5621-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5621-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f5621-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f5621-115">Parent elements</span></span>

<span data-ttu-id="f5621-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f5621-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f5621-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="f5621-117">Remarks</span></span>

<span data-ttu-id="f5621-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="f5621-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f5621-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f5621-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f5621-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="f5621-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f5621-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f5621-121">Schema name</span></span>  <br/> |<span data-ttu-id="f5621-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f5621-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f5621-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f5621-123">Validation file</span></span>  <br/> |<span data-ttu-id="f5621-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f5621-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f5621-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f5621-125">Can be empty</span></span>  <br/> |<span data-ttu-id="f5621-126">False</span><span class="sxs-lookup"><span data-stu-id="f5621-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f5621-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="f5621-127">See also</span></span>



- [<span data-ttu-id="f5621-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f5621-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

