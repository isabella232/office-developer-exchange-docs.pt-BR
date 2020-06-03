---
title: Createassociado
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAssociated
api_type:
- schema
ms.assetid: 742a6136-6015-4924-bae4-f3868127e966
description: O elemento createassociado indica se um cliente pode criar uma tabela de conteúdo associada. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: e88d7670fd9ef848221dab8cc145395bcb11e5bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460789"
---
# <a name="createassociated"></a><span data-ttu-id="0d1a1-104">Createassociado</span><span class="sxs-lookup"><span data-stu-id="0d1a1-104">CreateAssociated</span></span>

<span data-ttu-id="0d1a1-105">O elemento **createassociado** indica se um cliente pode criar uma tabela de conteúdo associada.</span><span class="sxs-lookup"><span data-stu-id="0d1a1-105">The **CreateAssociated** element indicates whether a client can create an associated contents table.</span></span> <span data-ttu-id="0d1a1-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0d1a1-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CreateAssociated>true or false</CreateAssociated>
```

 <span data-ttu-id="0d1a1-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="0d1a1-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d1a1-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0d1a1-108">Attributes and elements</span></span>

<span data-ttu-id="0d1a1-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0d1a1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d1a1-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="0d1a1-110">Attributes</span></span>

<span data-ttu-id="0d1a1-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0d1a1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0d1a1-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0d1a1-112">Child elements</span></span>

<span data-ttu-id="0d1a1-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0d1a1-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0d1a1-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0d1a1-114">Parent elements</span></span>

|<span data-ttu-id="0d1a1-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0d1a1-115">**Element**</span></span>|<span data-ttu-id="0d1a1-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0d1a1-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d1a1-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="0d1a1-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="0d1a1-118">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="0d1a1-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="0d1a1-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="0d1a1-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0d1a1-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="0d1a1-120">Text value</span></span>

<span data-ttu-id="0d1a1-121">Um valor **true** indica que um cliente pode criar uma tabela de conteúdo associado.</span><span class="sxs-lookup"><span data-stu-id="0d1a1-121">A text value of **true** indicates that a client can create an associated contents table.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0d1a1-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="0d1a1-122">Remarks</span></span>

<span data-ttu-id="0d1a1-123">Esta propriedade só é usada em objetos Folder.</span><span class="sxs-lookup"><span data-stu-id="0d1a1-123">This property is only used on folder objects.</span></span>
  
<span data-ttu-id="0d1a1-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="0d1a1-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d1a1-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0d1a1-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d1a1-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="0d1a1-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0d1a1-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0d1a1-127">Schema Name</span></span>  <br/> |<span data-ttu-id="0d1a1-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0d1a1-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="0d1a1-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0d1a1-129">Validation File</span></span>  <br/> |<span data-ttu-id="0d1a1-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0d1a1-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0d1a1-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0d1a1-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="0d1a1-132">False</span><span class="sxs-lookup"><span data-stu-id="0d1a1-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0d1a1-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="0d1a1-133">See also</span></span>



- [<span data-ttu-id="0d1a1-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0d1a1-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="0d1a1-135">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="0d1a1-135">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

