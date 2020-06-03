---
title: CanModifyPermissions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9693de1a-0c76-4898-8f4d-a8693fb005b3
description: O elemento CanModifyPermissions indica se um usuário pode modificar permissões de acesso a um local de compartilhamento de documentos.
ms.openlocfilehash: bf21b80a738498176bac41feea001ff859a54c2b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461580"
---
# <a name="canmodifypermissions-soap"></a><span data-ttu-id="4452c-103">CanModifyPermissions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4452c-103">CanModifyPermissions (SOAP)</span></span>

<span data-ttu-id="4452c-104">O elemento **CanModifyPermissions** indica se um usuário pode modificar permissões de acesso a um local de compartilhamento de documentos.</span><span class="sxs-lookup"><span data-stu-id="4452c-104">The **CanModifyPermissions** element indicates whether a user can modify access permissions to a document sharing location.</span></span> 
  
```XML
<CanModifyPermissions /> 
```

 <span data-ttu-id="4452c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="4452c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4452c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4452c-106">Attributes and elements</span></span>

<span data-ttu-id="4452c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4452c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4452c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4452c-108">Attributes</span></span>

<span data-ttu-id="4452c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4452c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4452c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4452c-110">Child elements</span></span>

<span data-ttu-id="4452c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4452c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4452c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4452c-112">Parent elements</span></span>

|<span data-ttu-id="4452c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4452c-113">**Element**</span></span>|<span data-ttu-id="4452c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4452c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4452c-115">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4452c-115">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="4452c-116">Representa informações de localização e metadados de um local de compartilhamento de documentos.</span><span class="sxs-lookup"><span data-stu-id="4452c-116">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4452c-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="4452c-117">Text value</span></span>

<span data-ttu-id="4452c-118">O valor booliano do elemento **CanModifyPermissions** indica se os usuários podem modificar as permissões de acesso para o local de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="4452c-118">The Boolean value of the **CanModifyPermissions** element indicates whether users can modify access permissions to the sharing location.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="4452c-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4452c-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4452c-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="4452c-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="4452c-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4452c-121">Schema Name</span></span>  <br/> |<span data-ttu-id="4452c-122">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="4452c-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="4452c-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4452c-123">Validation File</span></span>  <br/> |<span data-ttu-id="4452c-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4452c-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4452c-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4452c-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="4452c-126">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="4452c-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4452c-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="4452c-127">See also</span></span>



[<span data-ttu-id="4452c-128">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4452c-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="4452c-129">Referência do serviço Web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="4452c-129">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="4452c-130">Elementos XML de descoberta automática SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="4452c-130">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

