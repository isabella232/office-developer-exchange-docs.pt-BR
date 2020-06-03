---
title: UnresolvedEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnresolvedEntry
api_type:
- schema
ms.assetid: 5ac6116a-3b24-40f8-a877-dbe9a6935919
description: O elemento UnresolvedEntry contém o nome de um contato ou de uma lista de distribuição a ser resolvida.
ms.openlocfilehash: 0f157c1be6c327187456a795c4c1000b8c35b620
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459837"
---
# <a name="unresolvedentry"></a><span data-ttu-id="ecde8-103">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="ecde8-103">UnresolvedEntry</span></span>

<span data-ttu-id="ecde8-104">O elemento **UnresolvedEntry** contém o nome de um contato ou de uma lista de distribuição a ser resolvida.</span><span class="sxs-lookup"><span data-stu-id="ecde8-104">The **UnresolvedEntry** element contains the name of a contact or distribution list to resolve.</span></span> 
  
[<span data-ttu-id="ecde8-105">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="ecde8-105">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="ecde8-106">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="ecde8-106">UnresolvedEntry</span></span>](unresolvedentry.md)
  
```xml
<UnresolvedEntry/>
```

 <span data-ttu-id="ecde8-107">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="ecde8-107">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ecde8-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ecde8-108">Attributes and elements</span></span>

<span data-ttu-id="ecde8-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ecde8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ecde8-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="ecde8-110">Attributes</span></span>

<span data-ttu-id="ecde8-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ecde8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ecde8-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ecde8-112">Child elements</span></span>

<span data-ttu-id="ecde8-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ecde8-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ecde8-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ecde8-114">Parent elements</span></span>

|<span data-ttu-id="ecde8-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ecde8-115">**Element**</span></span>|<span data-ttu-id="ecde8-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ecde8-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ecde8-117">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="ecde8-117">ResolveNames</span></span>](resolvenames.md) <br/> |<span data-ttu-id="ecde8-118">Define uma solicitação para resolver nomes ambíguos.</span><span class="sxs-lookup"><span data-stu-id="ecde8-118">Defines a request to resolve ambiguous names.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ecde8-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ecde8-119">Text value</span></span>

<span data-ttu-id="ecde8-120">O valor de texto representa o nome de um contato público ou de uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="ecde8-120">The text value represents the name of a public contact or distribution list.</span></span> <span data-ttu-id="ecde8-121">O comprimento mínimo da cadeia de caracteres é um caractere.</span><span class="sxs-lookup"><span data-stu-id="ecde8-121">The minimum length of the string is one character.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ecde8-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="ecde8-122">Remarks</span></span>

<span data-ttu-id="ecde8-123">O valor de texto desse elemento é usado para resolver nomes nos seguintes campos:</span><span class="sxs-lookup"><span data-stu-id="ecde8-123">The text value of this element is used to resolve names against the following fields:</span></span>
  
- <span data-ttu-id="ecde8-124">Nome</span><span class="sxs-lookup"><span data-stu-id="ecde8-124">First name</span></span>
    
- <span data-ttu-id="ecde8-125">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="ecde8-125">Last name</span></span>
    
- <span data-ttu-id="ecde8-126">Nome diferenciado (DN)</span><span class="sxs-lookup"><span data-stu-id="ecde8-126">Display name</span></span>
    
- <span data-ttu-id="ecde8-127">Nome completo</span><span class="sxs-lookup"><span data-stu-id="ecde8-127">Full name</span></span>
    
- <span data-ttu-id="ecde8-128">Office</span><span class="sxs-lookup"><span data-stu-id="ecde8-128">Office</span></span>
    
- <span data-ttu-id="ecde8-129">Alias</span><span class="sxs-lookup"><span data-stu-id="ecde8-129">Alias</span></span>
    
- <span data-ttu-id="ecde8-130">Endereço SMTP</span><span class="sxs-lookup"><span data-stu-id="ecde8-130">SMTP address</span></span>
    
<span data-ttu-id="ecde8-131">Os endereços de email com tipos de roteamento prefixos, como SMTP ou SIP, são salvos em uma matriz de vários valores.</span><span class="sxs-lookup"><span data-stu-id="ecde8-131">Email addresses with prefixed routing types, such as smtp or sip, are saved in a multivalue array.</span></span> <span data-ttu-id="ecde8-132">A [operação ResolveNames](resolvenames-operation.md) executa uma correspondência parcial em relação a cada valor dessa matriz quando você adiciona o tipo de roteamento no início do nome não resolvido, como "SIP:User1@Contoso.com".</span><span class="sxs-lookup"><span data-stu-id="ecde8-132">The [ResolveNames operation](resolvenames-operation.md) performs a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1@Contoso.com".</span></span> <span data-ttu-id="ecde8-133">Se você não especificar um tipo de roteamento, a operação **ResolveNames** usará como padrão o tipo de roteamento do SMTP, o corresponderá a uma propriedade de endereço SMTP primária e não pesquisará a matriz de vários valores.</span><span class="sxs-lookup"><span data-stu-id="ecde8-133">If you don't specify a routing type, the **ResolveNames** operation will default to the routing type of smtp, match it to a primary SMTP address property, and not search the multivalue array.</span></span> 
  
<span data-ttu-id="ecde8-134">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ecde8-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ecde8-135">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ecde8-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ecde8-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="ecde8-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ecde8-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ecde8-137">Schema Name</span></span>  <br/> |<span data-ttu-id="ecde8-138">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ecde8-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ecde8-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ecde8-139">Validation File</span></span>  <br/> |<span data-ttu-id="ecde8-140">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ecde8-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ecde8-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ecde8-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="ecde8-142">False</span><span class="sxs-lookup"><span data-stu-id="ecde8-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ecde8-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="ecde8-143">See also</span></span>



[<span data-ttu-id="ecde8-144">Operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="ecde8-144">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="ecde8-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ecde8-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

