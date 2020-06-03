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
description: O elemento RequestServerVersion contém as informações de controle de versão que identificam a versão do esquema para direcionar uma solicitação.
ms.openlocfilehash: c4ae59a03c812d21153e4338734185d933d914ec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468317"
---
# <a name="requestserverversion"></a><span data-ttu-id="dbef3-103">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="dbef3-103">RequestServerVersion</span></span>

<span data-ttu-id="dbef3-104">O elemento **RequestServerVersion** contém as informações de controle de versão que identificam a versão do esquema para direcionar uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbef3-104">The **RequestServerVersion** element contains the versioning information that identifies the schema version to target for a request.</span></span> 
  
```XML
<RequestServerVersion Version=""/>
```

 <span data-ttu-id="dbef3-105">**ExchangeVersionType**</span><span class="sxs-lookup"><span data-stu-id="dbef3-105">**ExchangeVersionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dbef3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="dbef3-106">Attributes and elements</span></span>

<span data-ttu-id="dbef3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dbef3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dbef3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="dbef3-108">Attributes</span></span>

|<span data-ttu-id="dbef3-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="dbef3-109">**Attribute**</span></span>|<span data-ttu-id="dbef3-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dbef3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dbef3-111">Versão</span><span class="sxs-lookup"><span data-stu-id="dbef3-111">Version</span></span>  <br/> |<span data-ttu-id="dbef3-112">Descreve a versão a ser direcionada para a solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbef3-112">Describes the version to target for the request.</span></span> <span data-ttu-id="dbef3-113">Este atributo é obrigatório quando a versão do servidor de destino é uma versão do Exchange que começa com o Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="dbef3-113">This attribute is required when the target server version is a version of Exchange starting with Exchange Server 2010.</span></span>  <br/> |
   
#### <a name="version-attribute-values"></a><span data-ttu-id="dbef3-114">Valores de atributo de versão</span><span class="sxs-lookup"><span data-stu-id="dbef3-114">Version attribute values</span></span>

|<span data-ttu-id="dbef3-115">**Valor**</span><span class="sxs-lookup"><span data-stu-id="dbef3-115">**Value**</span></span>|<span data-ttu-id="dbef3-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dbef3-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dbef3-117">Exchange2007</span><span class="sxs-lookup"><span data-stu-id="dbef3-117">Exchange2007</span></span>  <br/> |<span data-ttu-id="dbef3-118">Direcione os arquivos de esquema para a versão inicial do Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="dbef3-118">Target the schema files for the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="dbef3-119">Exchange2007_SP1</span><span class="sxs-lookup"><span data-stu-id="dbef3-119">Exchange2007_SP1</span></span>  <br/> |<span data-ttu-id="dbef3-120">Direcione os arquivos de esquema para o Exchange 2007 Service Pack 1 (SP1), o Exchange 2007 Service Pack 2 (SP2) e o Exchange 2007 Service Pack 3 (SP3).</span><span class="sxs-lookup"><span data-stu-id="dbef3-120">Target the schema files for Exchange 2007 Service Pack 1 (SP1), Exchange 2007 Service Pack 2 (SP2), and Exchange 2007 Service Pack 3 (SP3).</span></span>  <br/> |
|<span data-ttu-id="dbef3-121">Exchange2010</span><span class="sxs-lookup"><span data-stu-id="dbef3-121">Exchange2010</span></span>  <br/> |<span data-ttu-id="dbef3-122">Direcione os arquivos de esquema para o Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="dbef3-122">Target the schema files for Exchange 2010.</span></span>  <br/> |
|<span data-ttu-id="dbef3-123">Exchange2010_SP1</span><span class="sxs-lookup"><span data-stu-id="dbef3-123">Exchange2010_SP1</span></span>  <br/> |<span data-ttu-id="dbef3-124">Direcione os arquivos de esquema para o Exchange 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="dbef3-124">Target the schema files for Exchange 2010 Service Pack 1 (SP1).</span></span>  <br/> |
|<span data-ttu-id="dbef3-125">Exchange2010_SP2</span><span class="sxs-lookup"><span data-stu-id="dbef3-125">Exchange2010_SP2</span></span>  <br/> |<span data-ttu-id="dbef3-126">Direcione os arquivos de esquema para o Exchange 2010 Service Pack 2 (SP2) e o Exchange 2010 Service Pack 3 (SP3).</span><span class="sxs-lookup"><span data-stu-id="dbef3-126">Target the schema files for Exchange 2010 Service Pack 2 (SP2) and Exchange 2010 Service Pack 3 (SP3).</span></span>  <br/> |
|<span data-ttu-id="dbef3-127">Exchange2013</span><span class="sxs-lookup"><span data-stu-id="dbef3-127">Exchange2013</span></span>  <br/> |<span data-ttu-id="dbef3-128">Direcione os arquivos de esquema para o Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="dbef3-128">Target the schema files for Exchange 2013.</span></span>  <br/> |
|<span data-ttu-id="dbef3-129">Exchange2013_SP1</span><span class="sxs-lookup"><span data-stu-id="dbef3-129">Exchange2013_SP1</span></span>  <br/> |<span data-ttu-id="dbef3-130">Direcione os arquivos de esquema para o Exchange 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="dbef3-130">Target the schema files for Exchange 2013 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="dbef3-131">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dbef3-131">Child elements</span></span>

<span data-ttu-id="dbef3-132">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="dbef3-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dbef3-133">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dbef3-133">Parent elements</span></span>

<span data-ttu-id="dbef3-134">O elemento **RequestServerVersion** está localizado no cabeçalho SOAP.</span><span class="sxs-lookup"><span data-stu-id="dbef3-134">The **RequestServerVersion** element is located in the SOAP header.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="dbef3-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="dbef3-135">Remarks</span></span>

<span data-ttu-id="dbef3-136">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="dbef3-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dbef3-137">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="dbef3-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dbef3-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="dbef3-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dbef3-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dbef3-139">Schema Name</span></span>  <br/> |<span data-ttu-id="dbef3-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="dbef3-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="dbef3-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dbef3-141">Validation File</span></span>  <br/> |<span data-ttu-id="dbef3-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="dbef3-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dbef3-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="dbef3-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="dbef3-144">False</span><span class="sxs-lookup"><span data-stu-id="dbef3-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dbef3-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="dbef3-145">See also</span></span>



- [<span data-ttu-id="dbef3-146">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="dbef3-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="dbef3-147">Solicitações de controle de versão</span><span class="sxs-lookup"><span data-stu-id="dbef3-147">Versioning Requests</span></span>](https://msdn.microsoft.com/library/76877b0a-d2e5-4c74-9295-7b445a41d46a%28Office.15%29.aspx)

