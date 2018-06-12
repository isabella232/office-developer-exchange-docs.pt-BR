---
title: Ler
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Read
api_type:
- schema
ms.assetid: b14637e9-1695-4b7e-b078-ae527c2e4303
description: O elemento de leitura indica se um cliente pode ler uma pasta ou item. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: cd9c2c9802c78b202418e3947f5b5718b0f676cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824948"
---
# <a name="read"></a><span data-ttu-id="16083-104">Ler</span><span class="sxs-lookup"><span data-stu-id="16083-104">Read</span></span>

<span data-ttu-id="16083-105">O elemento de **leitura** indica se um cliente pode ler uma pasta ou item.</span><span class="sxs-lookup"><span data-stu-id="16083-105">The **Read** element indicates whether a client can read a folder or item.</span></span> <span data-ttu-id="16083-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="16083-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Read>true or false</Read>
```

 <span data-ttu-id="16083-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="16083-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16083-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="16083-108">Attributes and elements</span></span>

<span data-ttu-id="16083-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="16083-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16083-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="16083-110">Attributes</span></span>

<span data-ttu-id="16083-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="16083-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="16083-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="16083-112">Child elements</span></span>

<span data-ttu-id="16083-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="16083-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="16083-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="16083-114">Parent elements</span></span>

|<span data-ttu-id="16083-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="16083-115">**Element**</span></span>|<span data-ttu-id="16083-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="16083-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16083-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="16083-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="16083-118">Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="16083-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="16083-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="16083-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="16083-120">Text value</span><span class="sxs-lookup"><span data-stu-id="16083-120">Text value</span></span>

<span data-ttu-id="16083-121">Um valor de texto de **true** indica que um cliente pode ler um item da pasta.</span><span class="sxs-lookup"><span data-stu-id="16083-121">A text value of **true** indicates that a client can read an item of folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="16083-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="16083-122">Remarks</span></span>

<span data-ttu-id="16083-123">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="16083-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="16083-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="16083-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16083-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="16083-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="16083-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="16083-126">Schema Name</span></span>  <br/> |<span data-ttu-id="16083-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="16083-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="16083-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="16083-128">Validation File</span></span>  <br/> |<span data-ttu-id="16083-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="16083-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="16083-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="16083-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="16083-131">False</span><span class="sxs-lookup"><span data-stu-id="16083-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="16083-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="16083-132">See also</span></span>



- [<span data-ttu-id="16083-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="16083-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="16083-134">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="16083-134">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

