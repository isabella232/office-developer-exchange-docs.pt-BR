---
title: Status (MemberStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 4f8a860b-0a48-4a0d-9a7a-69a0304aa747
description: O elemento de Status fornece informações sobre o status de um membro da lista de distribuição no servidor.
ms.openlocfilehash: ef062433c80f0cca413c33012e1164b17e226faf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825580"
---
# <a name="status-memberstatustype"></a><span data-ttu-id="d4378-103">Status (MemberStatusType)</span><span class="sxs-lookup"><span data-stu-id="d4378-103">Status (MemberStatusType)</span></span>

<span data-ttu-id="d4378-104">O elemento de **Status** fornece informações sobre o status de um membro da lista de distribuição no servidor.</span><span class="sxs-lookup"><span data-stu-id="d4378-104">The **Status** element provides information about the status of a distribution list member on the server.</span></span> 
  
```
<Status>Unrecognized or Normal or Demoted</Status>
```

 <span data-ttu-id="d4378-105">**MemberStatusType**</span><span class="sxs-lookup"><span data-stu-id="d4378-105">**MemberStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4378-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d4378-106">Attributes and elements</span></span>

<span data-ttu-id="d4378-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d4378-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4378-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d4378-108">Attributes</span></span>

<span data-ttu-id="d4378-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d4378-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4378-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d4378-110">Child elements</span></span>

<span data-ttu-id="d4378-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d4378-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d4378-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d4378-112">Parent elements</span></span>

|<span data-ttu-id="d4378-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d4378-113">**Element**</span></span>|<span data-ttu-id="d4378-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d4378-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4378-115">Membro</span><span class="sxs-lookup"><span data-stu-id="d4378-115">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d4378-116">Representa um membro de uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="d4378-116">Represents a member of a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d4378-117">Text value</span><span class="sxs-lookup"><span data-stu-id="d4378-117">Text value</span></span>

<span data-ttu-id="d4378-118">A tabela a seguir lista os valores possíveis para o elemento de **Status** .</span><span class="sxs-lookup"><span data-stu-id="d4378-118">The following table lists the possible values for the **Status** element.</span></span> 
  
<span data-ttu-id="d4378-119">**Valores do elemento de status**</span><span class="sxs-lookup"><span data-stu-id="d4378-119">**Status element values**</span></span>

|<span data-ttu-id="d4378-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="d4378-120">**Value**</span></span>|<span data-ttu-id="d4378-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d4378-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d4378-122">Não reconhecido</span><span class="sxs-lookup"><span data-stu-id="d4378-122">Unrecognized</span></span>  <br/> |<span data-ttu-id="d4378-123">Informações do membro são inválido ou não reconhecido.</span><span class="sxs-lookup"><span data-stu-id="d4378-123">Member information is invalid or unrecognized.</span></span>  <br/> |
|<span data-ttu-id="d4378-124">Normal</span><span class="sxs-lookup"><span data-stu-id="d4378-124">Normal</span></span>  <br/> |<span data-ttu-id="d4378-125">Informações de membro em uma lista de distribuição são sincronizadas com o objeto referenciado.</span><span class="sxs-lookup"><span data-stu-id="d4378-125">Member information in a distribution list is in sync with the referenced object.</span></span>  <br/> |
|<span data-ttu-id="d4378-126">Rebaixado</span><span class="sxs-lookup"><span data-stu-id="d4378-126">Demoted</span></span>  <br/> |<span data-ttu-id="d4378-127">Objeto referenciado não está disponível.</span><span class="sxs-lookup"><span data-stu-id="d4378-127">Referenced object is not available.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d4378-128">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="d4378-128">Remarks</span></span>

<span data-ttu-id="d4378-129">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d4378-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4378-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d4378-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4378-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="d4378-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4378-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d4378-132">Schema Name</span></span>  <br/> |<span data-ttu-id="d4378-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d4378-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="d4378-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d4378-134">Validation File</span></span>  <br/> |<span data-ttu-id="d4378-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d4378-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4378-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d4378-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4378-137">False</span><span class="sxs-lookup"><span data-stu-id="d4378-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4378-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="d4378-138">See also</span></span>



- [<span data-ttu-id="d4378-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d4378-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

