---
title: Caixa de correio (disponibilidade)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Mailbox
api_type:
- schema
ms.assetid: affd192e-8914-473f-9098-d9bdf898de2c
description: O elemento de caixa de correio representa o usuário de caixa de correio para um SetUserOofSettings ou GetUserOofSettings solicitação.
ms.openlocfilehash: 2e901ae0df56542f56f247184254294735018468
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824254"
---
# <a name="mailbox-availability"></a><span data-ttu-id="ef61a-103">Caixa de correio (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="ef61a-103">Mailbox (Availability)</span></span>

<span data-ttu-id="ef61a-104">O elemento de **caixa de correio** representa o usuário de caixa de correio para um SetUserOofSettings ou GetUserOofSettings solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef61a-104">The **Mailbox** element represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span> 
  
```xml
<Mailbox>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Mailbox>
```

<span data-ttu-id="ef61a-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="ef61a-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ef61a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ef61a-106">Attributes and elements</span></span>

<span data-ttu-id="ef61a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ef61a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef61a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ef61a-108">Attributes</span></span>

<span data-ttu-id="ef61a-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ef61a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ef61a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ef61a-110">Child elements</span></span>

|<span data-ttu-id="ef61a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ef61a-111">**Element**</span></span>|<span data-ttu-id="ef61a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ef61a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef61a-113">Nome (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="ef61a-113">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="ef61a-114">Representa o nome de exibição do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ef61a-114">Represents the display name of the mailbox user.</span></span> <span data-ttu-id="ef61a-115">Esse elemento é opcional a SetUserOofSettingsRequest.</span><span class="sxs-lookup"><span data-stu-id="ef61a-115">This element is optional in the SetUserOofSettingsRequest.</span></span> <span data-ttu-id="ef61a-116">O GetUserOofSettingsRequest retornará esse elemento.</span><span class="sxs-lookup"><span data-stu-id="ef61a-116">The GetUserOofSettingsRequest will return this element.</span></span>  <br/> |
|[<span data-ttu-id="ef61a-117">Endereço (string)</span><span class="sxs-lookup"><span data-stu-id="ef61a-117">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="ef61a-118">Representa o endereço de email do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ef61a-118">Represents the e-mail address of the mailbox user.</span></span> <span data-ttu-id="ef61a-119">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef61a-119">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="ef61a-120">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="ef61a-120">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="ef61a-121">Representa o protocolo de roteamento para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="ef61a-121">Represents the routing protocol for the message.</span></span> <span data-ttu-id="ef61a-122">Esse elemento é opcional a SetUserOofSettingsRequest.</span><span class="sxs-lookup"><span data-stu-id="ef61a-122">This element is optional in the SetUserOofSettingsRequest.</span></span> <span data-ttu-id="ef61a-123">O GetUserOofSettingsRequest retornará esse elemento.</span><span class="sxs-lookup"><span data-stu-id="ef61a-123">The GetUserOofSettingsRequest will return this element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ef61a-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ef61a-124">Parent elements</span></span>

|<span data-ttu-id="ef61a-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ef61a-125">**Element**</span></span>|<span data-ttu-id="ef61a-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ef61a-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef61a-127">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="ef61a-127">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md) <br/> |<span data-ttu-id="ef61a-128">Usado para fazer configurações de fora do escritório (OOF) e mensagens de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ef61a-128">Used to get a mailbox user's Out of Office (OOF) settings and messages.</span></span>  <br/> <span data-ttu-id="ef61a-129">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="ef61a-129">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[<span data-ttu-id="ef61a-130">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="ef61a-130">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md) <br/> |<span data-ttu-id="ef61a-131">Usada para definir configurações de ausência temporária e mensagens de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ef61a-131">Used to set a mailbox user's OOF settings and messages.</span></span>  <br/> <span data-ttu-id="ef61a-132">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="ef61a-132">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ef61a-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="ef61a-133">Remarks</span></span>

<span data-ttu-id="ef61a-134">O endereço de email é usado para identificar a pasta de calendário que contém as configurações de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="ef61a-134">The e-mail address is used to identify the calendar folder that contains the OOF settings.</span></span> 
  
<span data-ttu-id="ef61a-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="ef61a-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef61a-136">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ef61a-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef61a-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="ef61a-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ef61a-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ef61a-138">Schema Name</span></span>  <br/> |<span data-ttu-id="ef61a-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ef61a-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="ef61a-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ef61a-140">Validation File</span></span>  <br/> |<span data-ttu-id="ef61a-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ef61a-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ef61a-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ef61a-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="ef61a-143">False</span><span class="sxs-lookup"><span data-stu-id="ef61a-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef61a-144">Ver também</span><span class="sxs-lookup"><span data-stu-id="ef61a-144">See also</span></span>

- [<span data-ttu-id="ef61a-145">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="ef61a-145">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="ef61a-146">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="ef61a-146">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

