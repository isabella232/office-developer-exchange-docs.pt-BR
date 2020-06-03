---
title: DataType
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
description: O elemento DataType descreve o tipo de dados que é compartilhado por uma pasta compartilhada.
ms.openlocfilehash: a7df8d38e10f0ab31038d790d8f35208d1be66d5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458828"
---
# <a name="datatype"></a><span data-ttu-id="2c5ab-103">DataType</span><span class="sxs-lookup"><span data-stu-id="2c5ab-103">DataType</span></span>

<span data-ttu-id="2c5ab-104">O elemento **DataType** descreve o tipo de dados que é compartilhado por uma pasta compartilhada.</span><span class="sxs-lookup"><span data-stu-id="2c5ab-104">The **DataType** element describes the type of data that is shared by a shared folder.</span></span> 
  
```xml
<DataType>Calendar or Contacts</DataType>
```

<span data-ttu-id="2c5ab-105">**SharingDataType**</span><span class="sxs-lookup"><span data-stu-id="2c5ab-105">**SharingDataType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2c5ab-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2c5ab-106">Attributes and elements</span></span>

<span data-ttu-id="2c5ab-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2c5ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c5ab-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2c5ab-108">Attributes</span></span>

<span data-ttu-id="2c5ab-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c5ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c5ab-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2c5ab-110">Child elements</span></span>

<span data-ttu-id="2c5ab-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2c5ab-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2c5ab-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2c5ab-112">Parent elements</span></span>

|<span data-ttu-id="2c5ab-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2c5ab-113">**Element**</span></span>|<span data-ttu-id="2c5ab-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2c5ab-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c5ab-115">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="2c5ab-115">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="2c5ab-116">Define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada.</span><span class="sxs-lookup"><span data-stu-id="2c5ab-116">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2c5ab-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="2c5ab-117">Text value</span></span>

<span data-ttu-id="2c5ab-118">A tabela a seguir lista os valores possíveis para o elemento **DataType** .</span><span class="sxs-lookup"><span data-stu-id="2c5ab-118">The following table lists the possible values for the **DataType** element.</span></span> 
  
<span data-ttu-id="2c5ab-119">**Valores do elemento DataType**</span><span class="sxs-lookup"><span data-stu-id="2c5ab-119">**DataType element values**</span></span>

|<span data-ttu-id="2c5ab-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="2c5ab-120">**Value**</span></span>|<span data-ttu-id="2c5ab-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2c5ab-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2c5ab-122">Calendário</span><span class="sxs-lookup"><span data-stu-id="2c5ab-122">Calendar</span></span>  <br/> |<span data-ttu-id="2c5ab-123">Indica que a pasta compartilhada contém informações do calendário.</span><span class="sxs-lookup"><span data-stu-id="2c5ab-123">Indicates that the shared folder contains calendar information.</span></span>  <br/> |
|<span data-ttu-id="2c5ab-124">Contatos</span><span class="sxs-lookup"><span data-stu-id="2c5ab-124">Contacts</span></span>  <br/> |<span data-ttu-id="2c5ab-125">Indica que a pasta compartilhada contém informações de contato.</span><span class="sxs-lookup"><span data-stu-id="2c5ab-125">Indicates that the shared folder contains contact information.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2c5ab-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="2c5ab-126">Remarks</span></span>

<span data-ttu-id="2c5ab-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2c5ab-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c5ab-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2c5ab-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c5ab-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="2c5ab-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2c5ab-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2c5ab-130">Schema Name</span></span>  <br/> |<span data-ttu-id="2c5ab-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="2c5ab-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2c5ab-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2c5ab-132">Validation File</span></span>  <br/> |<span data-ttu-id="2c5ab-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2c5ab-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2c5ab-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2c5ab-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="2c5ab-135">False</span><span class="sxs-lookup"><span data-stu-id="2c5ab-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2c5ab-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="2c5ab-136">See also</span></span>

- [<span data-ttu-id="2c5ab-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2c5ab-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

