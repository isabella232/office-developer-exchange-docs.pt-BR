---
title: IsInError
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsInError
api_type:
- schema
ms.assetid: f56e6c31-a566-4761-8755-d90ffe6fe790
description: O elemento IsInError indica se a regra está em uma condição de erro.
ms.openlocfilehash: 9e642c9f89434bdcad97b0c16dc35f99196051d7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464214"
---
# <a name="isinerror"></a><span data-ttu-id="bce05-103">IsInError</span><span class="sxs-lookup"><span data-stu-id="bce05-103">IsInError</span></span>

<span data-ttu-id="bce05-104">O elemento **IsInError** indica se a regra está em uma condição de erro.</span><span class="sxs-lookup"><span data-stu-id="bce05-104">The **IsInError** element indicates whether the rule is in an error condition.</span></span> 
  
```XML
<IsInError/>
```

 <span data-ttu-id="bce05-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="bce05-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bce05-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="bce05-106">Attributes and elements</span></span>

<span data-ttu-id="bce05-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bce05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bce05-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="bce05-108">Attributes</span></span>

<span data-ttu-id="bce05-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bce05-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bce05-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bce05-110">Child elements</span></span>

<span data-ttu-id="bce05-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bce05-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bce05-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bce05-112">Parent elements</span></span>

|<span data-ttu-id="bce05-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bce05-113">**Element**</span></span>|<span data-ttu-id="bce05-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bce05-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bce05-115">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="bce05-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="bce05-116">Representa uma regra na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="bce05-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bce05-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="bce05-117">Text value</span></span>

<span data-ttu-id="bce05-118">Um valor de texto **true** indica que a regra está em uma condição de erro.</span><span class="sxs-lookup"><span data-stu-id="bce05-118">A text value of **true** indicates that the rule is in an error condition.</span></span> <span data-ttu-id="bce05-119">Um valor **false** indica que a regra não está em uma condição de erro.</span><span class="sxs-lookup"><span data-stu-id="bce05-119">A value of **false** indicates that the rule is not in an error condition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bce05-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="bce05-120">Remarks</span></span>

<span data-ttu-id="bce05-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="bce05-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bce05-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="bce05-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bce05-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="bce05-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bce05-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bce05-124">Schema Name</span></span>  <br/> |<span data-ttu-id="bce05-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="bce05-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bce05-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bce05-126">Validation File</span></span>  <br/> |<span data-ttu-id="bce05-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bce05-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bce05-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="bce05-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="bce05-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="bce05-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bce05-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="bce05-130">See also</span></span>



- [<span data-ttu-id="bce05-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bce05-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

