---
title: GetPhoneCallInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetPhoneCallInformation
api_type:
- schema
ms.assetid: 5f4ee71c-bde0-4b0d-b426-0c24dfe67585
description: O elemento GetPhoneCallInformation especifica uma solicitação para obter informações de chamadas telefônicas.
ms.openlocfilehash: b835cd301b1c243e88034d1057026ef1305b9038
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530194"
---
# <a name="getphonecallinformation"></a><span data-ttu-id="9e408-103">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="9e408-103">GetPhoneCallInformation</span></span>

<span data-ttu-id="9e408-104">O elemento **GetPhoneCallInformation** especifica uma solicitação para obter informações de chamadas telefônicas.</span><span class="sxs-lookup"><span data-stu-id="9e408-104">The **GetPhoneCallInformation** element specifies a request to get telephone call information.</span></span> 
  
```xml
<GetPhoneCallInformation>
   <PhoneCallId/>
</GetPhoneCallInformation>
```

 <span data-ttu-id="9e408-105">**GetPhoneCallInformationType**</span><span class="sxs-lookup"><span data-stu-id="9e408-105">**GetPhoneCallInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e408-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9e408-106">Attributes and elements</span></span>

<span data-ttu-id="9e408-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9e408-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e408-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9e408-108">Attributes</span></span>

<span data-ttu-id="9e408-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e408-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e408-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9e408-110">Child elements</span></span>

|<span data-ttu-id="9e408-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9e408-111">**Element**</span></span>|<span data-ttu-id="9e408-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9e408-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e408-113">Chamada de chamada</span><span class="sxs-lookup"><span data-stu-id="9e408-113">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="9e408-114">Especifica o identificador de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="9e408-114">Specifies the identifier of a phone call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9e408-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9e408-115">Parent elements</span></span>

<span data-ttu-id="9e408-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e408-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="9e408-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="9e408-117">Text value</span></span>

<span data-ttu-id="9e408-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9e408-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9e408-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="9e408-119">Remarks</span></span>

<span data-ttu-id="9e408-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e408-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e408-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9e408-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e408-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="9e408-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9e408-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9e408-123">Schema Name</span></span>  <br/> |<span data-ttu-id="9e408-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9e408-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9e408-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9e408-125">Validation File</span></span>  <br/> |<span data-ttu-id="9e408-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9e408-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9e408-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9e408-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="9e408-128">False</span><span class="sxs-lookup"><span data-stu-id="9e408-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e408-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="9e408-129">See also</span></span>



- [<span data-ttu-id="9e408-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9e408-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

