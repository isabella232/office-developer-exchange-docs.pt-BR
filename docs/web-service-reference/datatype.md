---
title: Tipo de dados
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DataType
api_type:
- schema
ms.assetid: 267fe5aa-f9b1-4d4c-ac11-0f2e50ec2627
description: O elemento DataType descreve o tipo de dados que são compartilhados por uma pasta compartilhada.
ms.openlocfilehash: b1adac8e3029abd64df96ab1560706babe4b12f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751688"
---
# <a name="datatype"></a><span data-ttu-id="a9eda-103">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="a9eda-103">DataType</span></span>

<span data-ttu-id="a9eda-104">O elemento **DataType** descreve o tipo de dados que são compartilhados por uma pasta compartilhada.</span><span class="sxs-lookup"><span data-stu-id="a9eda-104">The **DataType** element describes the type of data that is shared by a shared folder.</span></span> 
  
```xml
<DataType>Calendar or Contacts</DataType>
```

<span data-ttu-id="a9eda-105">**SharingDataType**</span><span class="sxs-lookup"><span data-stu-id="a9eda-105">**SharingDataType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a9eda-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a9eda-106">Attributes and elements</span></span>

<span data-ttu-id="a9eda-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a9eda-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a9eda-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a9eda-108">Attributes</span></span>

<span data-ttu-id="a9eda-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a9eda-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a9eda-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a9eda-110">Child elements</span></span>

<span data-ttu-id="a9eda-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a9eda-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a9eda-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a9eda-112">Parent elements</span></span>

|<span data-ttu-id="a9eda-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a9eda-113">**Element**</span></span>|<span data-ttu-id="a9eda-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a9eda-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9eda-115">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="a9eda-115">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="a9eda-116">Define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada.</span><span class="sxs-lookup"><span data-stu-id="a9eda-116">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a9eda-117">Text value</span><span class="sxs-lookup"><span data-stu-id="a9eda-117">Text value</span></span>

<span data-ttu-id="a9eda-118">A tabela a seguir lista os valores possíveis para o elemento de **tipo de dados** .</span><span class="sxs-lookup"><span data-stu-id="a9eda-118">The following table lists the possible values for the **DataType** element.</span></span> 
  
<span data-ttu-id="a9eda-119">**Valores de elemento DataType**</span><span class="sxs-lookup"><span data-stu-id="a9eda-119">**DataType element values**</span></span>

|<span data-ttu-id="a9eda-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="a9eda-120">**Value**</span></span>|<span data-ttu-id="a9eda-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a9eda-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a9eda-122">Calendário</span><span class="sxs-lookup"><span data-stu-id="a9eda-122">Calendar</span></span>  <br/> |<span data-ttu-id="a9eda-123">Indica que a pasta compartilhada contém informações de calendário.</span><span class="sxs-lookup"><span data-stu-id="a9eda-123">Indicates that the shared folder contains calendar information.</span></span>  <br/> |
|<span data-ttu-id="a9eda-124">Contatos</span><span class="sxs-lookup"><span data-stu-id="a9eda-124">Contacts</span></span>  <br/> |<span data-ttu-id="a9eda-125">Indica que a pasta compartilhada contém informações de contato.</span><span class="sxs-lookup"><span data-stu-id="a9eda-125">Indicates that the shared folder contains contact information.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a9eda-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="a9eda-126">Remarks</span></span>

<span data-ttu-id="a9eda-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a9eda-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a9eda-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a9eda-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a9eda-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="a9eda-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a9eda-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a9eda-130">Schema Name</span></span>  <br/> |<span data-ttu-id="a9eda-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a9eda-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a9eda-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a9eda-132">Validation File</span></span>  <br/> |<span data-ttu-id="a9eda-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a9eda-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a9eda-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a9eda-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="a9eda-135">False</span><span class="sxs-lookup"><span data-stu-id="a9eda-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a9eda-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="a9eda-136">See also</span></span>

- [<span data-ttu-id="a9eda-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a9eda-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

