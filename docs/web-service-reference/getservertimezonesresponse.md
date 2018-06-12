---
title: GetServerTimeZonesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZonesResponse
api_type:
- schema
ms.assetid: 97c94d32-10f1-4c3e-ab20-9fd7e8257e50
description: O elemento de GetServerTimeZonesResponse define uma resposta a uma solicitação de operação GetServerTimeZones.
ms.openlocfilehash: 119809076c82ff75a6dd061fc976f861e13f4e57
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823664"
---
# <a name="getservertimezonesresponse"></a><span data-ttu-id="1cda3-103">GetServerTimeZonesResponse</span><span class="sxs-lookup"><span data-stu-id="1cda3-103">GetServerTimeZonesResponse</span></span>

<span data-ttu-id="1cda3-104">O elemento de **GetServerTimeZonesResponse** define uma resposta a uma solicitação de [operação GetServerTimeZones](getservertimezones-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1cda3-104">The **GetServerTimeZonesResponse** element defines a response to a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span> 
  
```XML
<GetServerTimeZonesResponse>
   <ResponseMessages/>
</GetServerTimeZonesResponse>
```

 <span data-ttu-id="1cda3-105">**GetServerTimeZonesResponseType**</span><span class="sxs-lookup"><span data-stu-id="1cda3-105">**GetServerTimeZonesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1cda3-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1cda3-106">Attributes and elements</span></span>

<span data-ttu-id="1cda3-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1cda3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1cda3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1cda3-108">Attributes</span></span>

<span data-ttu-id="1cda3-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1cda3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1cda3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1cda3-110">Child elements</span></span>

|<span data-ttu-id="1cda3-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1cda3-111">**Element**</span></span>|<span data-ttu-id="1cda3-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1cda3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cda3-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1cda3-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="1cda3-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1cda3-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1cda3-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1cda3-115">Parent elements</span></span>

<span data-ttu-id="1cda3-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1cda3-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1cda3-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="1cda3-117">Remarks</span></span>

<span data-ttu-id="1cda3-118">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1cda3-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1cda3-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1cda3-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1cda3-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="1cda3-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1cda3-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1cda3-121">Schema Name</span></span>  <br/> |<span data-ttu-id="1cda3-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="1cda3-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1cda3-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1cda3-123">Validation File</span></span>  <br/> |<span data-ttu-id="1cda3-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1cda3-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1cda3-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1cda3-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="1cda3-126">False</span><span class="sxs-lookup"><span data-stu-id="1cda3-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1cda3-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="1cda3-127">See also</span></span>



- [<span data-ttu-id="1cda3-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1cda3-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

