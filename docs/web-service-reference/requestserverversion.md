---
title: RequestServerVersion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestServerVersion
api_type:
- schema
ms.assetid: af4032d5-42b3-463e-9d0a-8236d78e5b75
description: O elemento RequestServerVersion contém as informações de controle de versão que identifica a versão do esquema de destino para uma solicitação.
ms.openlocfilehash: 0092d90a5fc479363f6d774b793c7148ad29f21c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825143"
---
# <a name="requestserverversion"></a><span data-ttu-id="36561-103">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="36561-103">RequestServerVersion</span></span>

<span data-ttu-id="36561-104">O elemento **RequestServerVersion** contém as informações de controle de versão que identifica a versão do esquema de destino para uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="36561-104">The **RequestServerVersion** element contains the versioning information that identifies the schema version to target for a request.</span></span> 
  
```XML
<RequestServerVersion Version=""/>
```

 <span data-ttu-id="36561-105">**ExchangeVersionType**</span><span class="sxs-lookup"><span data-stu-id="36561-105">**ExchangeVersionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36561-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="36561-106">Attributes and elements</span></span>

<span data-ttu-id="36561-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="36561-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36561-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="36561-108">Attributes</span></span>

|<span data-ttu-id="36561-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="36561-109">**Attribute**</span></span>|<span data-ttu-id="36561-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="36561-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="36561-111">Versão</span><span class="sxs-lookup"><span data-stu-id="36561-111">Version</span></span>  <br/> |<span data-ttu-id="36561-112">Descreve a versão de destino para a solicitação.</span><span class="sxs-lookup"><span data-stu-id="36561-112">Describes the version to target for the request.</span></span> <span data-ttu-id="36561-113">Este atributo é necessário quando a versão do servidor de destino for uma versão do Exchange, começando com o Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="36561-113">This attribute is required when the target server version is a version of Exchange starting with Exchange Server 2010.</span></span>  <br/> |
   
#### <a name="version-attribute-values"></a><span data-ttu-id="36561-114">Valores de atributos de versão</span><span class="sxs-lookup"><span data-stu-id="36561-114">Version attribute values</span></span>

|<span data-ttu-id="36561-115">**Valor**</span><span class="sxs-lookup"><span data-stu-id="36561-115">**Value**</span></span>|<span data-ttu-id="36561-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="36561-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="36561-117">Exchange2007</span><span class="sxs-lookup"><span data-stu-id="36561-117">Exchange2007</span></span>  <br/> |<span data-ttu-id="36561-118">Direcione os arquivos de esquema para a versão de lançamento inicial do Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="36561-118">Target the schema files for the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="36561-119">Exchange2007_SP1</span><span class="sxs-lookup"><span data-stu-id="36561-119">Exchange2007_SP1</span></span>  <br/> |<span data-ttu-id="36561-120">Direcione os arquivos de esquema para o Exchange 2007 Service Pack 1 (SP1) do Exchange 2007 Service Pack 2 (SP2) e Exchange 2007 Service Pack 3 (SP3).</span><span class="sxs-lookup"><span data-stu-id="36561-120">Target the schema files for Exchange 2007 Service Pack 1 (SP1), Exchange 2007 Service Pack 2 (SP2), and Exchange 2007 Service Pack 3 (SP3).</span></span>  <br/> |
|<span data-ttu-id="36561-121">Exchange2010</span><span class="sxs-lookup"><span data-stu-id="36561-121">Exchange2010</span></span>  <br/> |<span data-ttu-id="36561-122">Direcione os arquivos de esquema para o Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="36561-122">Target the schema files for Exchange 2010.</span></span>  <br/> |
|<span data-ttu-id="36561-123">Exchange2010_SP1</span><span class="sxs-lookup"><span data-stu-id="36561-123">Exchange2010_SP1</span></span>  <br/> |<span data-ttu-id="36561-124">Direcione os arquivos de esquema para o Exchange 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="36561-124">Target the schema files for Exchange 2010 Service Pack 1 (SP1).</span></span>  <br/> |
|<span data-ttu-id="36561-125">Exchange2010_SP2</span><span class="sxs-lookup"><span data-stu-id="36561-125">Exchange2010_SP2</span></span>  <br/> |<span data-ttu-id="36561-126">Direcione os arquivos de esquema para o Exchange 2010 Service Pack 2 (SP2) e Exchange 2010 Service Pack 3 (SP3).</span><span class="sxs-lookup"><span data-stu-id="36561-126">Target the schema files for Exchange 2010 Service Pack 2 (SP2) and Exchange 2010 Service Pack 3 (SP3).</span></span>  <br/> |
|<span data-ttu-id="36561-127">Exchange2013</span><span class="sxs-lookup"><span data-stu-id="36561-127">Exchange2013</span></span>  <br/> |<span data-ttu-id="36561-128">Direcione os arquivos de esquema para o Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="36561-128">Target the schema files for Exchange 2013.</span></span>  <br/> |
|<span data-ttu-id="36561-129">Exchange2013_SP1</span><span class="sxs-lookup"><span data-stu-id="36561-129">Exchange2013_SP1</span></span>  <br/> |<span data-ttu-id="36561-130">Direcione os arquivos de esquema para o Exchange 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="36561-130">Target the schema files for Exchange 2013 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="36561-131">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="36561-131">Child elements</span></span>

<span data-ttu-id="36561-132">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="36561-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="36561-133">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="36561-133">Parent elements</span></span>

<span data-ttu-id="36561-134">O elemento **RequestServerVersion** está localizado no cabeçalho SOAP.</span><span class="sxs-lookup"><span data-stu-id="36561-134">The **RequestServerVersion** element is located in the SOAP header.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="36561-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="36561-135">Remarks</span></span>

<span data-ttu-id="36561-136">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="36561-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36561-137">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="36561-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36561-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="36561-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36561-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="36561-139">Schema Name</span></span>  <br/> |<span data-ttu-id="36561-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="36561-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="36561-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="36561-141">Validation File</span></span>  <br/> |<span data-ttu-id="36561-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="36561-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36561-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="36561-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="36561-144">False</span><span class="sxs-lookup"><span data-stu-id="36561-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36561-145">Ver também</span><span class="sxs-lookup"><span data-stu-id="36561-145">See also</span></span>



- [<span data-ttu-id="36561-146">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="36561-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="36561-147">Solicitações de controle de versão</span><span class="sxs-lookup"><span data-stu-id="36561-147">Versioning Requests</span></span>](http://msdn.microsoft.com/library/76877b0a-d2e5-4c74-9295-7b445a41d46a%28Office.15%29.aspx)

