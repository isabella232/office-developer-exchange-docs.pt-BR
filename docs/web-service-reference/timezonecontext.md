---
title: TimeZoneContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneContext
api_type:
- schema
ms.assetid: 573c462b-aa1d-4ba0-8852-e3f48b26873b
description: O elemento TimeZoneContext é usado no cabeçalho simples (SOAP Object Access Protocol) para especificar a que deve ser usado como padrão ao atribuir o fuso horário para as propriedades de data/hora dos objetos que são criados, atualizados e recuperados pela definição de fuso horário usando serviços Web do Exchange (EWS).
ms.openlocfilehash: 38b7ab4c587adac45fc3bcf351f417ea72313a97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837751"
---
# <a name="timezonecontext"></a><span data-ttu-id="a8b04-103">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="a8b04-103">TimeZoneContext</span></span>

<span data-ttu-id="a8b04-104">O elemento **TimeZoneContext** é usado no cabeçalho simples (SOAP Object Access Protocol) para especificar a definição de fuso horário que será usado como padrão ao atribuir o fuso horário para as propriedades de data/hora dos objetos criados, atualizado, e recuperada usando serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="a8b04-104">The **TimeZoneContext** element is used in the Simple Object Access Protocol (SOAP) header to specify the time zone definition that is to be used as the default when assigning the time zone for the DateTime properties of objects that are created, updated, and retrieved by using Exchange Web Services (EWS).</span></span> 
  
```xml
<TimeZoneContext>
   <TimeZoneDefinition/>
</TimeZoneContext>
```

 <span data-ttu-id="a8b04-105">**TimeZoneContextType**</span><span class="sxs-lookup"><span data-stu-id="a8b04-105">**TimeZoneContextType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8b04-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a8b04-106">Attributes and elements</span></span>

<span data-ttu-id="a8b04-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a8b04-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8b04-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a8b04-108">Attributes</span></span>

<span data-ttu-id="a8b04-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a8b04-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8b04-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a8b04-110">Child elements</span></span>

|<span data-ttu-id="a8b04-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a8b04-111">**Element**</span></span>|<span data-ttu-id="a8b04-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a8b04-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8b04-113">Timezonedefinition pela última vez</span><span class="sxs-lookup"><span data-stu-id="a8b04-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="a8b04-114">Especifica os períodos e transições que definem um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="a8b04-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a8b04-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a8b04-115">Parent elements</span></span>

<span data-ttu-id="a8b04-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a8b04-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a8b04-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="a8b04-117">Remarks</span></span>

<span data-ttu-id="a8b04-118">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="a8b04-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8b04-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a8b04-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8b04-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="a8b04-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8b04-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a8b04-121">Schema Name</span></span>  <br/> |<span data-ttu-id="a8b04-122">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a8b04-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="a8b04-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a8b04-123">Validation File</span></span>  <br/> |<span data-ttu-id="a8b04-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a8b04-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8b04-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a8b04-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8b04-126">False</span><span class="sxs-lookup"><span data-stu-id="a8b04-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8b04-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="a8b04-127">See also</span></span>



- [<span data-ttu-id="a8b04-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a8b04-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

