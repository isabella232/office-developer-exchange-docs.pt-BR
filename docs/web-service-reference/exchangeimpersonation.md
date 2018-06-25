---
title: ExchangeImpersonation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExchangeImpersonation
api_type:
- schema
ms.assetid: d8cbac49-47d0-4745-a2a7-545d33f8da93
description: O elemento ExchangeImpersonation é usado no cabeçalho de uma solicitação SOAP. Quando esse elemento estiver presente, o chamador está tentando representar a conta que está contida no elemento ExchangeImpersonation.
ms.openlocfilehash: aedeff22cda865ce1eec80dab9760d49fdc178f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752125"
---
# <a name="exchangeimpersonation"></a><span data-ttu-id="44d86-104">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="44d86-104">ExchangeImpersonation</span></span>

<span data-ttu-id="44d86-105">O elemento **ExchangeImpersonation** é usado no cabeçalho de uma solicitação SOAP.</span><span class="sxs-lookup"><span data-stu-id="44d86-105">The **ExchangeImpersonation** element is used in the SOAP header of a request.</span></span> <span data-ttu-id="44d86-106">Quando esse elemento estiver presente, o chamador está tentando representar a conta que está contida no elemento **ExchangeImpersonation** .</span><span class="sxs-lookup"><span data-stu-id="44d86-106">When this element is present, the caller is trying to impersonate the account that is contained within the **ExchangeImpersonation** element.</span></span> 
  
[<span data-ttu-id="44d86-107">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="44d86-107">ExchangeImpersonation</span></span>](exchangeimpersonation.md)
  
```xml
<ExchangeImpersonation>
   <ConnectingSID/>
</ExchangeImpersonation>
```

 <span data-ttu-id="44d86-108">**ExchangeImpersonationType**</span><span class="sxs-lookup"><span data-stu-id="44d86-108">**ExchangeImpersonationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="44d86-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="44d86-109">Attributes and elements</span></span>

<span data-ttu-id="44d86-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="44d86-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="44d86-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="44d86-111">Attributes</span></span>

<span data-ttu-id="44d86-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="44d86-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="44d86-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="44d86-113">Child elements</span></span>

|<span data-ttu-id="44d86-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="44d86-114">**Element**</span></span>|<span data-ttu-id="44d86-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="44d86-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44d86-116">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="44d86-116">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="44d86-117">Representa uma conta para representar quando você estiver usando o cabeçalho SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="44d86-117">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="44d86-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="44d86-118">Parent elements</span></span>

<span data-ttu-id="44d86-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="44d86-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="44d86-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="44d86-120">Remarks</span></span>

<span data-ttu-id="44d86-121">A chamada conta deve ter o **ms-exch-impersonation** direto no servidor de acesso para cliente e o **ms-exch-MayImpersonate** direito em ou o banco de dados de caixa de correio que contém a caixa de correio para representar ou o usuário/contato do Active Directory objeto.</span><span class="sxs-lookup"><span data-stu-id="44d86-121">The calling account must have the **ms-exch-impersonation** right on the Client Access server and the **ms-exch-MayImpersonate** right on either the mailbox database that contains the mailbox to impersonate or the Active Directory User/Contact object.</span></span> 
  
<span data-ttu-id="44d86-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="44d86-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="44d86-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="44d86-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="44d86-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="44d86-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="44d86-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="44d86-125">Schema name</span></span>  <br/> |<span data-ttu-id="44d86-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="44d86-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="44d86-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="44d86-127">Validation file</span></span>  <br/> |<span data-ttu-id="44d86-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="44d86-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="44d86-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="44d86-129">Can be empty</span></span>  <br/> |<span data-ttu-id="44d86-130">False</span><span class="sxs-lookup"><span data-stu-id="44d86-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="44d86-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="44d86-131">See also</span></span>



[<span data-ttu-id="44d86-132">Autorização de servidor-para-servidor no EWS</span><span class="sxs-lookup"><span data-stu-id="44d86-132">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

