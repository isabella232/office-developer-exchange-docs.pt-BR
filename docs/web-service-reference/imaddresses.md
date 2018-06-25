---
title: ImAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ImAddresses
api_type:
- schema
ms.assetid: 29f614a7-7fe6-47fa-b5f2-8feff106aa99
description: O elemento ImAddresses representa uma coleção de endereços de mensagens instantâneas de um contato.
ms.openlocfilehash: e8c7a22e8537a4526594042905f7bb8454238bf1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823861"
---
# <a name="imaddresses"></a><span data-ttu-id="496be-103">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="496be-103">ImAddresses</span></span>

<span data-ttu-id="496be-104">O elemento **ImAddresses** representa uma coleção de endereços de mensagens instantâneas de um contato.</span><span class="sxs-lookup"><span data-stu-id="496be-104">The **ImAddresses** element represents a collection of instant messaging addresses for a contact.</span></span> 
  
```xml
<ImAddresses>
   <Entry/>
</ImAddresses>
```

 <span data-ttu-id="496be-105">**ImAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="496be-105">**ImAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="496be-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="496be-106">Attributes and elements</span></span>

<span data-ttu-id="496be-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="496be-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="496be-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="496be-108">Attributes</span></span>

<span data-ttu-id="496be-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="496be-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="496be-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="496be-110">Child elements</span></span>

|<span data-ttu-id="496be-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="496be-111">**Element**</span></span>|<span data-ttu-id="496be-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="496be-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="496be-113">Entrada (IMAddress)</span><span class="sxs-lookup"><span data-stu-id="496be-113">Entry (IMAddress)</span></span>](entry-imaddress.md) <br/> |<span data-ttu-id="496be-114">Representa um endereço para um contato de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="496be-114">Represents an instant messaging address for a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="496be-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="496be-115">Parent elements</span></span>

|<span data-ttu-id="496be-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="496be-116">**Element**</span></span>|<span data-ttu-id="496be-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="496be-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="496be-118">Contato</span><span class="sxs-lookup"><span data-stu-id="496be-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="496be-119">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="496be-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="496be-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="496be-120">Remarks</span></span>

<span data-ttu-id="496be-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="496be-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="496be-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="496be-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="496be-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="496be-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="496be-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="496be-124">Schema name</span></span>  <br/> |<span data-ttu-id="496be-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="496be-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="496be-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="496be-126">Validation file</span></span>  <br/> |<span data-ttu-id="496be-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="496be-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="496be-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="496be-128">Can be empty</span></span>  <br/> |<span data-ttu-id="496be-129">False</span><span class="sxs-lookup"><span data-stu-id="496be-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="496be-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="496be-130">See also</span></span>



- [<span data-ttu-id="496be-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="496be-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

