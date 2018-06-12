---
title: MailboxDataArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxDataArray
api_type:
- schema
ms.assetid: a14af788-beee-452c-b5d0-37bcb4ef02ff
description: O elemento MailboxDataArray contém uma lista de caixas de correio para consultar informações sobre a disponibilidade.
ms.openlocfilehash: b76e71ee9127dc2221e0065a27d3c781f8b5786a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824283"
---
# <a name="mailboxdataarray"></a><span data-ttu-id="57d34-103">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="57d34-103">MailboxDataArray</span></span>

<span data-ttu-id="57d34-104">O elemento **MailboxDataArray** contém uma lista de caixas de correio para consultar informações sobre a disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="57d34-104">The **MailboxDataArray** element contains a list of mailboxes to query for availability information.</span></span> 
  
- [<span data-ttu-id="57d34-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="57d34-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="57d34-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="57d34-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="57d34-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="57d34-107">MailboxData</span></span>](mailboxdata.md)
  
```xml
<MailboxDataArray>
   <MailboxData>...</MailboxData>
</MailboxDataArray>
```

<span data-ttu-id="57d34-108">**ArrayOfMailboxData**</span><span class="sxs-lookup"><span data-stu-id="57d34-108">**ArrayOfMailboxData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="57d34-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="57d34-109">Attributes and elements</span></span>

<span data-ttu-id="57d34-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="57d34-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57d34-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="57d34-111">Attributes</span></span>

<span data-ttu-id="57d34-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="57d34-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57d34-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="57d34-113">Child elements</span></span>

|<span data-ttu-id="57d34-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="57d34-114">**Element**</span></span>|<span data-ttu-id="57d34-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="57d34-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57d34-116">MailboxData</span><span class="sxs-lookup"><span data-stu-id="57d34-116">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="57d34-117">Representa um usuário de caixa de correio individual e opções para o tipo de dados a serem retornadas sobre o usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="57d34-117">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="57d34-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="57d34-118">Parent elements</span></span>

|<span data-ttu-id="57d34-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="57d34-119">**Element**</span></span>|<span data-ttu-id="57d34-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="57d34-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57d34-121">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="57d34-121">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="57d34-122">Contém os argumentos usados para obter informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="57d34-122">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="57d34-123">Este é um elemento raiz.</span><span class="sxs-lookup"><span data-stu-id="57d34-123">This is a root element.</span></span>  <br/> <span data-ttu-id="57d34-124">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="57d34-124">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="57d34-125">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="57d34-125">Remarks</span></span>

<span data-ttu-id="57d34-126">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft® Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="57d34-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57d34-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="57d34-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57d34-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="57d34-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="57d34-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="57d34-129">Schema Name</span></span>  <br/> |<span data-ttu-id="57d34-130">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="57d34-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="57d34-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="57d34-131">Validation File</span></span>  <br/> |<span data-ttu-id="57d34-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="57d34-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="57d34-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="57d34-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="57d34-134">False</span><span class="sxs-lookup"><span data-stu-id="57d34-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57d34-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="57d34-135">See also</span></span>

- [<span data-ttu-id="57d34-136">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="57d34-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="57d34-137">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="57d34-137">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="57d34-138">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="57d34-138">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

