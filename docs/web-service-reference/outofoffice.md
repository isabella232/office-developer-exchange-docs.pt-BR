---
title: Fora
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OutOfOffice
api_type:
- schema
ms.assetid: fe1256ab-5c0f-467d-abb3-b38a2dc312ae
description: O elemento fora representa a mensagem de resposta e um tempo de duração para enviar a mensagem de resposta.
ms.openlocfilehash: 082a81b62e2b783b302b3e749e0066131a46d73e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456896"
---
# <a name="outofoffice"></a><span data-ttu-id="7f7f5-103">Fora</span><span class="sxs-lookup"><span data-stu-id="7f7f5-103">OutOfOffice</span></span>

<span data-ttu-id="7f7f5-104">O elemento **fora** representa a mensagem de resposta e um tempo de duração para enviar a mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="7f7f5-104">The **OutOfOffice** element represents the response message and a duration time for sending the response message.</span></span> 
  
```XML
<OutOfOffice>
   <ReplyBody/>
   <Duration/>
</OutOfOffice>
```

```XML
<OutOfOffice>
   <ReplyBody/>
</OutOfOffice>
```

<span data-ttu-id="7f7f5-105">**OutOfOfficeMailTip**</span><span class="sxs-lookup"><span data-stu-id="7f7f5-105">**OutOfOfficeMailTip**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7f7f5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="7f7f5-106">Attributes and elements</span></span>

<span data-ttu-id="7f7f5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7f7f5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f7f5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7f7f5-108">Attributes</span></span>

<span data-ttu-id="7f7f5-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7f7f5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7f7f5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7f7f5-110">Child elements</span></span>

|<span data-ttu-id="7f7f5-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7f7f5-111">**Element**</span></span>|<span data-ttu-id="7f7f5-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7f7f5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7f7f5-113">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="7f7f5-113">ReplyBody</span></span>](replybody.md) <br/> |<span data-ttu-id="7f7f5-114">Contém uma mensagem de ausência temporária (OOF) e o idioma usado para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="7f7f5-114">Contains an Out of Office (OOF) message and the language used for the message.</span></span>  <br/> |
|[<span data-ttu-id="7f7f5-115">Duração (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="7f7f5-115">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="7f7f5-116">Contém a duração em que o status de ausência temporária é habilitado se o elemento [OofState](oofstate.md) estiver definido como agendado.</span><span class="sxs-lookup"><span data-stu-id="7f7f5-116">Contains the duration that the OOF status is enabled if the [OofState](oofstate.md) element is set to Scheduled.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7f7f5-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7f7f5-117">Parent elements</span></span>

|<span data-ttu-id="7f7f5-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7f7f5-118">**Element**</span></span>|<span data-ttu-id="7f7f5-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7f7f5-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7f7f5-120">Dicas de Email</span><span class="sxs-lookup"><span data-stu-id="7f7f5-120">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="7f7f5-121">Representa valores de vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="7f7f5-121">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7f7f5-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="7f7f5-122">Text value</span></span>

<span data-ttu-id="7f7f5-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7f7f5-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7f7f5-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="7f7f5-124">Remarks</span></span>

<span data-ttu-id="7f7f5-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7f7f5-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7f7f5-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="7f7f5-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f7f5-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="7f7f5-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7f7f5-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7f7f5-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7f7f5-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7f7f5-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="7f7f5-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7f7f5-130">Validation File</span></span>  <br/> |<span data-ttu-id="7f7f5-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7f7f5-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7f7f5-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7f7f5-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7f7f5-133">False</span><span class="sxs-lookup"><span data-stu-id="7f7f5-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7f7f5-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="7f7f5-134">See also</span></span>

- [<span data-ttu-id="7f7f5-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7f7f5-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

