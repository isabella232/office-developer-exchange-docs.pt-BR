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
description: O elemento status fornece informações sobre o status de um membro da lista de distribuição no servidor.
ms.openlocfilehash: bfa0c349d6af51c1b2238c9749d2656541d31906
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465461"
---
# <a name="status-memberstatustype"></a><span data-ttu-id="1a0e7-103">Status (MemberStatusType)</span><span class="sxs-lookup"><span data-stu-id="1a0e7-103">Status (MemberStatusType)</span></span>

<span data-ttu-id="1a0e7-104">O elemento **status** fornece informações sobre o status de um membro da lista de distribuição no servidor.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-104">The **Status** element provides information about the status of a distribution list member on the server.</span></span> 
  
```
<Status>Unrecognized or Normal or Demoted</Status>
```

 <span data-ttu-id="1a0e7-105">**MemberStatusType**</span><span class="sxs-lookup"><span data-stu-id="1a0e7-105">**MemberStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a0e7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1a0e7-106">Attributes and elements</span></span>

<span data-ttu-id="1a0e7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a0e7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1a0e7-108">Attributes</span></span>

<span data-ttu-id="1a0e7-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a0e7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a0e7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1a0e7-110">Child elements</span></span>

<span data-ttu-id="1a0e7-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1a0e7-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1a0e7-112">Parent elements</span></span>

|<span data-ttu-id="1a0e7-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1a0e7-113">**Element**</span></span>|<span data-ttu-id="1a0e7-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1a0e7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a0e7-115">Membro</span><span class="sxs-lookup"><span data-stu-id="1a0e7-115">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1a0e7-116">Representa um membro de uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-116">Represents a member of a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1a0e7-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="1a0e7-117">Text value</span></span>

<span data-ttu-id="1a0e7-118">A tabela a seguir lista os valores possíveis para o elemento **status** .</span><span class="sxs-lookup"><span data-stu-id="1a0e7-118">The following table lists the possible values for the **Status** element.</span></span> 
  
<span data-ttu-id="1a0e7-119">**Valores do elemento status**</span><span class="sxs-lookup"><span data-stu-id="1a0e7-119">**Status element values**</span></span>

|<span data-ttu-id="1a0e7-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="1a0e7-120">**Value**</span></span>|<span data-ttu-id="1a0e7-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1a0e7-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1a0e7-122">Não reconhecido</span><span class="sxs-lookup"><span data-stu-id="1a0e7-122">Unrecognized</span></span>  <br/> |<span data-ttu-id="1a0e7-123">As informações do membro são inválidas ou não foram reconhecidas.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-123">Member information is invalid or unrecognized.</span></span>  <br/> |
|<span data-ttu-id="1a0e7-124">Normal</span><span class="sxs-lookup"><span data-stu-id="1a0e7-124">Normal</span></span>  <br/> |<span data-ttu-id="1a0e7-125">As informações de membro em uma lista de distribuição estão em sincronia com o objeto referenciado.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-125">Member information in a distribution list is in sync with the referenced object.</span></span>  <br/> |
|<span data-ttu-id="1a0e7-126">Rebaixado</span><span class="sxs-lookup"><span data-stu-id="1a0e7-126">Demoted</span></span>  <br/> |<span data-ttu-id="1a0e7-127">O objeto referenciado não está disponível.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-127">Referenced object is not available.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1a0e7-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="1a0e7-128">Remarks</span></span>

<span data-ttu-id="1a0e7-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a0e7-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1a0e7-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a0e7-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="1a0e7-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1a0e7-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1a0e7-132">Schema Name</span></span>  <br/> |<span data-ttu-id="1a0e7-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1a0e7-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="1a0e7-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1a0e7-134">Validation File</span></span>  <br/> |<span data-ttu-id="1a0e7-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1a0e7-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1a0e7-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1a0e7-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="1a0e7-137">False</span><span class="sxs-lookup"><span data-stu-id="1a0e7-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a0e7-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="1a0e7-138">See also</span></span>



- [<span data-ttu-id="1a0e7-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1a0e7-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

