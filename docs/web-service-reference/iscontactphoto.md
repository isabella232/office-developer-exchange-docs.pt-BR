---
title: IsContactPhoto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsContactPhoto
api_type:
- schema
ms.assetid: ae36b5f9-a787-4863-9dbc-258ad724801d
description: O elemento IsContactPhoto indica se o anexo de arquivo é uma imagem do contato.
ms.openlocfilehash: a015cd9bdb34ea9275952d5fe252a30cacf888ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823999"
---
# <a name="iscontactphoto"></a><span data-ttu-id="3eb37-103">IsContactPhoto</span><span class="sxs-lookup"><span data-stu-id="3eb37-103">IsContactPhoto</span></span>

<span data-ttu-id="3eb37-104">O elemento **IsContactPhoto** indica se o anexo de arquivo é uma imagem do contato.</span><span class="sxs-lookup"><span data-stu-id="3eb37-104">The **IsContactPhoto** element indicates whether the file attachment is a contact picture.</span></span> 
  
```xml
<IsContactPhoto>true or false</IsContactPhoto>
```

 <span data-ttu-id="3eb37-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="3eb37-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3eb37-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3eb37-106">Attributes and elements</span></span>

<span data-ttu-id="3eb37-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3eb37-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3eb37-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3eb37-108">Attributes</span></span>

<span data-ttu-id="3eb37-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3eb37-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3eb37-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3eb37-110">Child elements</span></span>

<span data-ttu-id="3eb37-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3eb37-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3eb37-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3eb37-112">Parent elements</span></span>

|<span data-ttu-id="3eb37-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3eb37-113">**Element**</span></span>|<span data-ttu-id="3eb37-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3eb37-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3eb37-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="3eb37-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="3eb37-116">Representa um arquivo anexado a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3eb37-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3eb37-117">Text value</span><span class="sxs-lookup"><span data-stu-id="3eb37-117">Text value</span></span>

<span data-ttu-id="3eb37-118">Esse elemento pode ser **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="3eb37-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="3eb37-119">O valor padrão é **false**.</span><span class="sxs-lookup"><span data-stu-id="3eb37-119">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3eb37-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="3eb37-120">Remarks</span></span>

<span data-ttu-id="3eb37-121">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="3eb37-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3eb37-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3eb37-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3eb37-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="3eb37-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3eb37-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3eb37-124">Schema Name</span></span>  <br/> |<span data-ttu-id="3eb37-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3eb37-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="3eb37-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3eb37-126">Validation File</span></span>  <br/> |<span data-ttu-id="3eb37-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3eb37-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3eb37-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3eb37-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="3eb37-129">False</span><span class="sxs-lookup"><span data-stu-id="3eb37-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3eb37-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="3eb37-130">See also</span></span>



- [<span data-ttu-id="3eb37-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3eb37-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

