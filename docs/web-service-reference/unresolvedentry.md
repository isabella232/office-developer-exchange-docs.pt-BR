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
description: O elemento UnresolvedEntry contém o nome de uma lista de contatos ou de distribuição para resolver.
ms.openlocfilehash: 98b447cd49685b49f73f75f12d921a65749be245
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837860"
---
# <a name="unresolvedentry"></a><span data-ttu-id="6ff30-103">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="6ff30-103">UnresolvedEntry</span></span>

<span data-ttu-id="6ff30-104">O elemento **UnresolvedEntry** contém o nome de uma lista de contatos ou de distribuição para resolver.</span><span class="sxs-lookup"><span data-stu-id="6ff30-104">The **UnresolvedEntry** element contains the name of a contact or distribution list to resolve.</span></span> 
  
[<span data-ttu-id="6ff30-105">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="6ff30-105">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="6ff30-106">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="6ff30-106">UnresolvedEntry</span></span>](unresolvedentry.md)
  
```xml
<UnresolvedEntry/>
```

 <span data-ttu-id="6ff30-107">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="6ff30-107">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6ff30-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6ff30-108">Attributes and elements</span></span>

<span data-ttu-id="6ff30-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6ff30-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ff30-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="6ff30-110">Attributes</span></span>

<span data-ttu-id="6ff30-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6ff30-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6ff30-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6ff30-112">Child elements</span></span>

<span data-ttu-id="6ff30-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6ff30-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6ff30-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6ff30-114">Parent elements</span></span>

|<span data-ttu-id="6ff30-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6ff30-115">**Element**</span></span>|<span data-ttu-id="6ff30-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6ff30-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ff30-117">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="6ff30-117">ResolveNames</span></span>](resolvenames.md) <br/> |<span data-ttu-id="6ff30-118">Define uma solicitação para resolver nomes de ambíguos.</span><span class="sxs-lookup"><span data-stu-id="6ff30-118">Defines a request to resolve ambiguous names.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6ff30-119">Text value</span><span class="sxs-lookup"><span data-stu-id="6ff30-119">Text value</span></span>

<span data-ttu-id="6ff30-120">O valor de texto representa o nome de uma lista de contatos ou de distribuição pública.</span><span class="sxs-lookup"><span data-stu-id="6ff30-120">The text value represents the name of a public contact or distribution list.</span></span> <span data-ttu-id="6ff30-121">O comprimento mínimo da cadeia de caracteres é um caractere.</span><span class="sxs-lookup"><span data-stu-id="6ff30-121">The minimum length of the string is one character.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6ff30-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="6ff30-122">Remarks</span></span>

<span data-ttu-id="6ff30-123">O valor de texto deste elemento é usado para resolver nomes com os seguintes campos:</span><span class="sxs-lookup"><span data-stu-id="6ff30-123">The text value of this element is used to resolve names against the following fields:</span></span>
  
- <span data-ttu-id="6ff30-124">Nome</span><span class="sxs-lookup"><span data-stu-id="6ff30-124">First name</span></span>
    
- <span data-ttu-id="6ff30-125">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="6ff30-125">Last name</span></span>
    
- <span data-ttu-id="6ff30-126">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="6ff30-126">Display name</span></span>
    
- <span data-ttu-id="6ff30-127">Nome completo</span><span class="sxs-lookup"><span data-stu-id="6ff30-127">Full name</span></span>
    
- <span data-ttu-id="6ff30-128">Office</span><span class="sxs-lookup"><span data-stu-id="6ff30-128">Office</span></span>
    
- <span data-ttu-id="6ff30-129">Alias</span><span class="sxs-lookup"><span data-stu-id="6ff30-129">Alias</span></span>
    
- <span data-ttu-id="6ff30-130">Endereço SMTP</span><span class="sxs-lookup"><span data-stu-id="6ff30-130">SMTP address</span></span>
    
<span data-ttu-id="6ff30-131">Endereços de email com tipos de roteamento de prefixados, como smtp ou sip, são salvas em uma matriz de valores múltiplos.</span><span class="sxs-lookup"><span data-stu-id="6ff30-131">Email addresses with prefixed routing types, such as smtp or sip, are saved in a multivalue array.</span></span> <span data-ttu-id="6ff30-132">A [operação ResolveNames](resolvenames-operation.md) realiza uma correspondência parcial contra cada valor dessa matriz, quando você adiciona o tipo de roteamento no início do nome não resolvido, como "sip:User1@Contoso.com".</span><span class="sxs-lookup"><span data-stu-id="6ff30-132">The [ResolveNames operation](resolvenames-operation.md) performs a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1@Contoso.com".</span></span> <span data-ttu-id="6ff30-133">Se você não especificar um tipo de roteamento, a operação **ResolveNames** padrão para o tipo de roteamento de smtp, associá-lo a uma propriedade de endereço SMTP principal e não a matriz de vários valores de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6ff30-133">If you don't specify a routing type, the **ResolveNames** operation will default to the routing type of smtp, match it to a primary SMTP address property, and not search the multivalue array.</span></span> 
  
<span data-ttu-id="6ff30-134">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6ff30-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6ff30-135">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6ff30-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ff30-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="6ff30-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6ff30-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6ff30-137">Schema Name</span></span>  <br/> |<span data-ttu-id="6ff30-138">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6ff30-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6ff30-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6ff30-139">Validation File</span></span>  <br/> |<span data-ttu-id="6ff30-140">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6ff30-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6ff30-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6ff30-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="6ff30-142">False</span><span class="sxs-lookup"><span data-stu-id="6ff30-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6ff30-143">Ver também</span><span class="sxs-lookup"><span data-stu-id="6ff30-143">See also</span></span>



[<span data-ttu-id="6ff30-144">Operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="6ff30-144">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="6ff30-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6ff30-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

