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
description: O elemento ShowExternalRecipientCount indica se os consumidores da operação GetQuery devem mostrar dicas de email que indicam o número de destinatários externos para os quais uma mensagem é endereçada.
ms.openlocfilehash: fc32e5c4a95f0e33b5532af9c77d31bd6446e641
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460467"
---
# <a name="showexternalrecipientcount"></a><span data-ttu-id="5a3b9-103">ShowExternalRecipientCount</span><span class="sxs-lookup"><span data-stu-id="5a3b9-103">ShowExternalRecipientCount</span></span>

<span data-ttu-id="5a3b9-104">O elemento **ShowExternalRecipientCount** indica se os consumidores da [operação](getmailtips-operation.md) GetQuery devem mostrar dicas de email que indicam o número de destinatários externos para os quais uma mensagem é endereçada.</span><span class="sxs-lookup"><span data-stu-id="5a3b9-104">The **ShowExternalRecipientCount** element indicates whether consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> 
  
```XML
<ShowExternalRecipientCount>true | false</ShowExternalRecipientCount>
```

 <span data-ttu-id="5a3b9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5a3b9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a3b9-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5a3b9-106">Attributes and elements</span></span>

<span data-ttu-id="5a3b9-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5a3b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a3b9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5a3b9-108">Attributes</span></span>

<span data-ttu-id="5a3b9-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5a3b9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a3b9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5a3b9-110">Child elements</span></span>

<span data-ttu-id="5a3b9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5a3b9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5a3b9-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5a3b9-112">Parent elements</span></span>

|<span data-ttu-id="5a3b9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5a3b9-113">**Element**</span></span>|<span data-ttu-id="5a3b9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5a3b9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a3b9-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="5a3b9-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="5a3b9-116">Contém informações de configuração de serviço para o serviço de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="5a3b9-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5a3b9-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5a3b9-117">Text value</span></span>

<span data-ttu-id="5a3b9-118">O valor de texto desse elemento será **true** se os consumidores da [operação](getmailtips-operation.md) GetQuery precisarem Mostrar dicas de email que indicam o número de destinatários externos para os quais uma mensagem é endereçada.</span><span class="sxs-lookup"><span data-stu-id="5a3b9-118">The text value of this element is **true** if consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> <span data-ttu-id="5a3b9-119">O valor é **false** se os consumidores da [operação](getmailtips-operation.md) GetQuery não precisam mostrar dicas de email que indicam o número de destinatários externos para os quais uma mensagem é endereçada.</span><span class="sxs-lookup"><span data-stu-id="5a3b9-119">The value is **false** if consumers of the [GetMailTips operation](getmailtips-operation.md) do not have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5a3b9-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="5a3b9-120">Remarks</span></span>

<span data-ttu-id="5a3b9-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5a3b9-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a3b9-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5a3b9-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a3b9-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="5a3b9-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5a3b9-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5a3b9-124">Schema Name</span></span>  <br/> |<span data-ttu-id="5a3b9-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5a3b9-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="5a3b9-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5a3b9-126">Validation File</span></span>  <br/> |<span data-ttu-id="5a3b9-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5a3b9-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5a3b9-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5a3b9-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="5a3b9-129">False</span><span class="sxs-lookup"><span data-stu-id="5a3b9-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a3b9-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="5a3b9-130">See also</span></span>



[<span data-ttu-id="5a3b9-131">Operação</span><span class="sxs-lookup"><span data-stu-id="5a3b9-131">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="5a3b9-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5a3b9-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

