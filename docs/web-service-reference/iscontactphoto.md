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
description: O elemento IsContactPhoto indica se o anexo de arquivo é uma imagem de contato.
ms.openlocfilehash: f60e558ab4f20b59c1d5ae51f9dfca430feeff00
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455545"
---
# <a name="iscontactphoto"></a><span data-ttu-id="61c86-103">IsContactPhoto</span><span class="sxs-lookup"><span data-stu-id="61c86-103">IsContactPhoto</span></span>

<span data-ttu-id="61c86-104">O elemento **IsContactPhoto** indica se o anexo de arquivo é uma imagem de contato.</span><span class="sxs-lookup"><span data-stu-id="61c86-104">The **IsContactPhoto** element indicates whether the file attachment is a contact picture.</span></span> 
  
```xml
<IsContactPhoto>true or false</IsContactPhoto>
```

 <span data-ttu-id="61c86-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="61c86-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61c86-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="61c86-106">Attributes and elements</span></span>

<span data-ttu-id="61c86-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="61c86-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61c86-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="61c86-108">Attributes</span></span>

<span data-ttu-id="61c86-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61c86-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="61c86-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="61c86-110">Child elements</span></span>

<span data-ttu-id="61c86-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="61c86-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="61c86-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="61c86-112">Parent elements</span></span>

|<span data-ttu-id="61c86-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="61c86-113">**Element**</span></span>|<span data-ttu-id="61c86-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="61c86-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61c86-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="61c86-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="61c86-116">Representa um arquivo anexado a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="61c86-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="61c86-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="61c86-117">Text value</span></span>

<span data-ttu-id="61c86-118">Esse elemento pode ser **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="61c86-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="61c86-119">O valor padrão é **false**.</span><span class="sxs-lookup"><span data-stu-id="61c86-119">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="61c86-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="61c86-120">Remarks</span></span>

<span data-ttu-id="61c86-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="61c86-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="61c86-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="61c86-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61c86-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="61c86-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="61c86-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="61c86-124">Schema Name</span></span>  <br/> |<span data-ttu-id="61c86-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="61c86-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="61c86-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="61c86-126">Validation File</span></span>  <br/> |<span data-ttu-id="61c86-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="61c86-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="61c86-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="61c86-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="61c86-129">False</span><span class="sxs-lookup"><span data-stu-id="61c86-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="61c86-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="61c86-130">See also</span></span>



- [<span data-ttu-id="61c86-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="61c86-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

