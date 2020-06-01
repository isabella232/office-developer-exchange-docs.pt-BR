---
title: UnknownEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnknownEntry
api_type:
- schema
ms.assetid: 3cb4c62e-052a-4326-8639-8c41dfd047b2
description: O elemento UnknownEntry representa uma única entrada de permissão desconhecida que não pode ser resolvida no serviço de diretório do Active Directory. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 452857690f719ba3ee9dffa29e576ca4f3b2b945
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459395"
---
# <a name="unknownentry"></a><span data-ttu-id="c8bf4-104">UnknownEntry</span><span class="sxs-lookup"><span data-stu-id="c8bf4-104">UnknownEntry</span></span>

<span data-ttu-id="c8bf4-105">O elemento **UnknownEntry** representa uma única entrada de permissão desconhecida que não pode ser resolvida no serviço de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c8bf4-105">The **UnknownEntry** element represents a single unknown permission entry that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="c8bf4-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c8bf4-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UnknownEntry/>
```

 <span data-ttu-id="c8bf4-107">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="c8bf4-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c8bf4-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c8bf4-108">Attributes and elements</span></span>

<span data-ttu-id="c8bf4-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c8bf4-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8bf4-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="c8bf4-110">Attributes</span></span>

<span data-ttu-id="c8bf4-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8bf4-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c8bf4-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c8bf4-112">Child elements</span></span>

<span data-ttu-id="c8bf4-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c8bf4-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c8bf4-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c8bf4-114">Parent elements</span></span>

|<span data-ttu-id="c8bf4-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c8bf4-115">**Element**</span></span>|<span data-ttu-id="c8bf4-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c8bf4-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8bf4-117">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="c8bf4-117">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="c8bf4-118">Contém uma matriz de entradas de permissão desconhecidas que não podem ser resolvidas no Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c8bf4-118">Contains an array of unknown permission entries that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="c8bf4-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="c8bf4-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c8bf4-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c8bf4-120">Text value</span></span>

<span data-ttu-id="c8bf4-121">O valor de texto representa uma entrada de permissão que não pode ser resolvida no Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c8bf4-121">The text value represents a permission entry that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="c8bf4-122">O valor de texto representa um identificador de segurança (SID).</span><span class="sxs-lookup"><span data-stu-id="c8bf4-122">The text value represents a security identifier (SID).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c8bf4-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="c8bf4-123">Remarks</span></span>

<span data-ttu-id="c8bf4-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="c8bf4-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c8bf4-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c8bf4-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c8bf4-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="c8bf4-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c8bf4-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c8bf4-127">Schema Name</span></span>  <br/> |<span data-ttu-id="c8bf4-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c8bf4-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="c8bf4-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c8bf4-129">Validation File</span></span>  <br/> |<span data-ttu-id="c8bf4-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c8bf4-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c8bf4-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c8bf4-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="c8bf4-132">False</span><span class="sxs-lookup"><span data-stu-id="c8bf4-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c8bf4-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="c8bf4-133">See also</span></span>



- [<span data-ttu-id="c8bf4-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c8bf4-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="c8bf4-135">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="c8bf4-135">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

