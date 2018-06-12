---
title: ReminderType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfaf84eb-271a-4728-84fc-a20205a100bd
description: O elemento ReminderType Especifica o tipo de lembretes para retornar.
ms.openlocfilehash: 11739d2068a1009b2840b2169e86b113151cbfa9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825077"
---
# <a name="remindertype"></a><span data-ttu-id="89756-103">ReminderType</span><span class="sxs-lookup"><span data-stu-id="89756-103">ReminderType</span></span>

<span data-ttu-id="89756-104">O elemento **ReminderType** Especifica o tipo de lembretes para retornar.</span><span class="sxs-lookup"><span data-stu-id="89756-104">The **ReminderType** element specifies the type of reminders to return.</span></span> 
  
```XML
<ReminderType> All | Current | Old </ReminderType>
```

 <span data-ttu-id="89756-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="89756-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89756-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="89756-106">Attributes and elements</span></span>

<span data-ttu-id="89756-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="89756-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89756-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="89756-108">Attributes</span></span>

<span data-ttu-id="89756-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="89756-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89756-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="89756-110">Child elements</span></span>

<span data-ttu-id="89756-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="89756-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="89756-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="89756-112">Parent elements</span></span>

[<span data-ttu-id="89756-113">GetReminders</span><span class="sxs-lookup"><span data-stu-id="89756-113">GetReminders</span></span>](getreminders.md)
  
## <a name="text-value"></a><span data-ttu-id="89756-114">Text value</span><span class="sxs-lookup"><span data-stu-id="89756-114">Text value</span></span>

<span data-ttu-id="89756-115">O valor de texto do elemento **ReminderType** é o tipo de lembretes a serem retornadas, **tudo**, **atual**ou **antigo**.</span><span class="sxs-lookup"><span data-stu-id="89756-115">The text value of the **ReminderType** element is the type of reminders to return, either **All**, **Current**, or **Old**.</span></span> <span data-ttu-id="89756-116">**All** é o valor recomendado para esse elemento.</span><span class="sxs-lookup"><span data-stu-id="89756-116">**All** is the recommended value for this element.</span></span> <span data-ttu-id="89756-117">Para obter mais informações sobre a relação entre o elemento **ReminderType** e os elementos [BeginTime](begintime.md) e [EndTime](endtime-remindermessagedatatype.md) , consulte [GetReminders operação](getreminders-operation.md).</span><span class="sxs-lookup"><span data-stu-id="89756-117">For more information about the relationship between the **ReminderType** element and the [BeginTime](begintime.md) and [EndTime](endtime-remindermessagedatatype.md) elements, see [GetReminders operation](getreminders-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="89756-118">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="89756-118">Remarks</span></span>

<span data-ttu-id="89756-119">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="89756-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="89756-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="89756-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89756-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="89756-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89756-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="89756-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="89756-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="89756-123">Schema Name</span></span>  <br/> |<span data-ttu-id="89756-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="89756-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="89756-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="89756-125">Validation File</span></span>  <br/> |<span data-ttu-id="89756-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="89756-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="89756-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="89756-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="89756-128">False</span><span class="sxs-lookup"><span data-stu-id="89756-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89756-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="89756-129">See also</span></span>



[<span data-ttu-id="89756-130">GetReminders</span><span class="sxs-lookup"><span data-stu-id="89756-130">GetReminders</span></span>](getreminders.md)


- [<span data-ttu-id="89756-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="89756-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

