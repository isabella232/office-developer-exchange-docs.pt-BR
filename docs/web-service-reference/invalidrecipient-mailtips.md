---
title: InvalidRecipient (dicas de dicas)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipient
api_type:
- schema
ms.assetid: 48959a99-bb0d-4004-963e-5a5baaa96476
description: O elemento InvalidRecipient indica se o destinatário é inválido.
ms.openlocfilehash: fddd75beb2228c50084bd38b4f4745064cc281dc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529998"
---
# <a name="invalidrecipient-mailtips"></a><span data-ttu-id="1dba9-103">InvalidRecipient (dicas de dicas)</span><span class="sxs-lookup"><span data-stu-id="1dba9-103">InvalidRecipient (MailTips)</span></span>

<span data-ttu-id="1dba9-104">O elemento **InvalidRecipient** indica se o destinatário é inválido.</span><span class="sxs-lookup"><span data-stu-id="1dba9-104">The **InvalidRecipient** element indicates whether the recipient is invalid.</span></span> 
  
```XML
<InvalidRecipient>true | false</InvalidRecipient>
```

 <span data-ttu-id="1dba9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="1dba9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1dba9-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1dba9-106">Attributes and elements</span></span>

<span data-ttu-id="1dba9-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1dba9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1dba9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1dba9-108">Attributes</span></span>

<span data-ttu-id="1dba9-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1dba9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1dba9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1dba9-110">Child elements</span></span>

<span data-ttu-id="1dba9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1dba9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1dba9-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1dba9-112">Parent elements</span></span>

|<span data-ttu-id="1dba9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1dba9-113">**Element**</span></span>|<span data-ttu-id="1dba9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1dba9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1dba9-115">Dicas de Email</span><span class="sxs-lookup"><span data-stu-id="1dba9-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="1dba9-116">Representa valores de vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="1dba9-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1dba9-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="1dba9-117">Text value</span></span>

<span data-ttu-id="1dba9-118">O valor de texto desse elemento será **true** se o destinatário for inválido.</span><span class="sxs-lookup"><span data-stu-id="1dba9-118">The text value of this element is **true** if the recipient is invalid.</span></span> <span data-ttu-id="1dba9-119">O valor será **false** se o destinatário não for inválido.</span><span class="sxs-lookup"><span data-stu-id="1dba9-119">The value is **false** if the recipient is not invalid.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1dba9-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="1dba9-120">Remarks</span></span>

<span data-ttu-id="1dba9-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1dba9-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1dba9-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1dba9-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1dba9-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="1dba9-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1dba9-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1dba9-124">Schema Name</span></span>  <br/> |<span data-ttu-id="1dba9-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1dba9-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="1dba9-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1dba9-126">Validation File</span></span>  <br/> |<span data-ttu-id="1dba9-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1dba9-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1dba9-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1dba9-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="1dba9-129">False</span><span class="sxs-lookup"><span data-stu-id="1dba9-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1dba9-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="1dba9-130">See also</span></span>



- [<span data-ttu-id="1dba9-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1dba9-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

