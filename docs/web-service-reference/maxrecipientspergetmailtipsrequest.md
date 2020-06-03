---
title: MaxRecipientsPerGetMailTipsRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxRecipientsPerGetMailTipsRequest
api_type:
- schema
ms.assetid: 8ff5df18-1989-4217-b4c0-599232911d0c
description: O elemento MaxRecipientsPerGetMailTipsRequest indica o número máximo de destinatários que podem ser passados para a operação GetQuery.
ms.openlocfilehash: cec343182b364fce040d5e32928cbeb569a22124
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468401"
---
# <a name="maxrecipientspergetmailtipsrequest"></a><span data-ttu-id="5f87b-103">MaxRecipientsPerGetMailTipsRequest</span><span class="sxs-lookup"><span data-stu-id="5f87b-103">MaxRecipientsPerGetMailTipsRequest</span></span>

<span data-ttu-id="5f87b-104">O elemento **MaxRecipientsPerGetMailTipsRequest** indica o número máximo de destinatários que podem ser passados para a [operação](getmailtips-operation.md)GetQuery.</span><span class="sxs-lookup"><span data-stu-id="5f87b-104">The **MaxRecipientsPerGetMailTipsRequest** element indicates the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span>
  
```XML
<MaxRecipientsPerGetMailTipsRequest/>
```

 <span data-ttu-id="5f87b-105">**int**</span><span class="sxs-lookup"><span data-stu-id="5f87b-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5f87b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5f87b-106">Attributes and elements</span></span>

<span data-ttu-id="5f87b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5f87b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5f87b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5f87b-108">Attributes</span></span>

<span data-ttu-id="5f87b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f87b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5f87b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5f87b-110">Child elements</span></span>

<span data-ttu-id="5f87b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5f87b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5f87b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5f87b-112">Parent elements</span></span>

|<span data-ttu-id="5f87b-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5f87b-113">**Element**</span></span>|<span data-ttu-id="5f87b-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5f87b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f87b-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="5f87b-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="5f87b-116">Contém informações de configuração de serviço para o serviço de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="5f87b-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5f87b-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5f87b-117">Text value</span></span>

<span data-ttu-id="5f87b-118">O valor de texto é um inteiro que representa o número máximo de destinatários que podem ser passados para a [operação](getmailtips-operation.md)getquers.</span><span class="sxs-lookup"><span data-stu-id="5f87b-118">The text value is an integer that represents the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5f87b-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="5f87b-119">Remarks</span></span>

<span data-ttu-id="5f87b-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f87b-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5f87b-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5f87b-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5f87b-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="5f87b-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5f87b-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5f87b-123">Schema Name</span></span>  <br/> |<span data-ttu-id="5f87b-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5f87b-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="5f87b-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5f87b-125">Validation File</span></span>  <br/> |<span data-ttu-id="5f87b-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5f87b-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5f87b-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5f87b-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="5f87b-128">False</span><span class="sxs-lookup"><span data-stu-id="5f87b-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5f87b-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="5f87b-129">See also</span></span>



[<span data-ttu-id="5f87b-130">Operação</span><span class="sxs-lookup"><span data-stu-id="5f87b-130">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="5f87b-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5f87b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

