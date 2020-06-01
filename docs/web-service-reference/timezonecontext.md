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
description: O elemento TimeZoneContext é usado no cabeçalho SOAP (Simple Object Access Protocol) para especificar a definição de fuso horário que deve ser usada como padrão ao atribuir o fuso horário das propriedades DateTime dos objetos criados, atualizados e recuperados usando o EWS (serviços Web do Exchange).
ms.openlocfilehash: 26727317ccf34338e8d62ec92bd7a44d43a6cfdb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460250"
---
# <a name="timezonecontext"></a><span data-ttu-id="f1509-103">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="f1509-103">TimeZoneContext</span></span>

<span data-ttu-id="f1509-104">O elemento **TimeZoneContext** é usado no cabeçalho SOAP (Simple Object Access Protocol) para especificar a definição de fuso horário que deve ser usada como padrão ao atribuir o fuso horário das propriedades DateTime dos objetos criados, atualizados e recuperados usando o EWS (serviços Web do Exchange).</span><span class="sxs-lookup"><span data-stu-id="f1509-104">The **TimeZoneContext** element is used in the Simple Object Access Protocol (SOAP) header to specify the time zone definition that is to be used as the default when assigning the time zone for the DateTime properties of objects that are created, updated, and retrieved by using Exchange Web Services (EWS).</span></span> 
  
```xml
<TimeZoneContext>
   <TimeZoneDefinition/>
</TimeZoneContext>
```

 <span data-ttu-id="f1509-105">**TimeZoneContextType**</span><span class="sxs-lookup"><span data-stu-id="f1509-105">**TimeZoneContextType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1509-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f1509-106">Attributes and elements</span></span>

<span data-ttu-id="f1509-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f1509-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1509-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f1509-108">Attributes</span></span>

<span data-ttu-id="f1509-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f1509-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1509-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f1509-110">Child elements</span></span>

|<span data-ttu-id="f1509-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f1509-111">**Element**</span></span>|<span data-ttu-id="f1509-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f1509-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1509-113">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="f1509-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="f1509-114">Especifica os períodos e as transições que definem um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="f1509-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f1509-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f1509-115">Parent elements</span></span>

<span data-ttu-id="f1509-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f1509-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f1509-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="f1509-117">Remarks</span></span>

<span data-ttu-id="f1509-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f1509-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1509-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f1509-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1509-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="f1509-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f1509-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f1509-121">Schema Name</span></span>  <br/> |<span data-ttu-id="f1509-122">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f1509-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="f1509-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f1509-123">Validation File</span></span>  <br/> |<span data-ttu-id="f1509-124">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f1509-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f1509-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f1509-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1509-126">False</span><span class="sxs-lookup"><span data-stu-id="f1509-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1509-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="f1509-127">See also</span></span>



- [<span data-ttu-id="f1509-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f1509-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

