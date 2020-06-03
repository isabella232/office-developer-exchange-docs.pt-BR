---
title: SendNotification
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendNotification
api_type:
- schema
ms.assetid: e45c4451-a286-4aec-a691-119ec41c58e0
description: O elemento SendNotification contém as notificações por push enviadas pelo computador que está executando o Microsoft Exchange Server 2007 para o aplicativo cliente.
ms.openlocfilehash: 49f2f6cb7f5c8e1171b54ff965ee1d22accc9bf2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462112"
---
# <a name="sendnotification"></a><span data-ttu-id="f6080-103">SendNotification</span><span class="sxs-lookup"><span data-stu-id="f6080-103">SendNotification</span></span>

<span data-ttu-id="f6080-104">O elemento **SendNotification** contém as notificações por push enviadas pelo computador que está executando o Microsoft Exchange Server 2007 para o aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="f6080-104">The **SendNotification** element contains the push notifications that are sent by the computer that is running Microsoft Exchange Server 2007 to the client application.</span></span> 
  
```xml
<SendNotification>
   <ResponseMessages/>
</SendNotification>
```

 <span data-ttu-id="f6080-105">**SendNotificationResponseType**</span><span class="sxs-lookup"><span data-stu-id="f6080-105">**SendNotificationResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6080-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f6080-106">Attributes and elements</span></span>

<span data-ttu-id="f6080-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f6080-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6080-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f6080-108">Attributes</span></span>

<span data-ttu-id="f6080-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f6080-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f6080-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f6080-110">Child elements</span></span>

|<span data-ttu-id="f6080-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f6080-111">**Element**</span></span>|<span data-ttu-id="f6080-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f6080-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6080-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f6080-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f6080-114">Contém as notificações por push enviadas pelo servidor de acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="f6080-114">Contains the push notifications that are sent by the Client Access server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f6080-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f6080-115">Parent elements</span></span>

<span data-ttu-id="f6080-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f6080-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f6080-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="f6080-117">Remarks</span></span>

<span data-ttu-id="f6080-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="f6080-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6080-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f6080-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6080-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="f6080-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f6080-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f6080-121">Schema Name</span></span>  <br/> |<span data-ttu-id="f6080-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f6080-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f6080-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f6080-123">Validation File</span></span>  <br/> |<span data-ttu-id="f6080-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f6080-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f6080-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f6080-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6080-126">False</span><span class="sxs-lookup"><span data-stu-id="f6080-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6080-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="f6080-127">See also</span></span>



- [<span data-ttu-id="f6080-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f6080-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f6080-129">Notificações de eventos no EWS</span><span class="sxs-lookup"><span data-stu-id="f6080-129">Event notifications in EWS</span></span>](https://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)
  
[<span data-ttu-id="f6080-130">Aplicativo de amostra de notificação por push</span><span class="sxs-lookup"><span data-stu-id="f6080-130">Push Notification Sample Application</span></span>](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

