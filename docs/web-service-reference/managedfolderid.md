---
title: ManagedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ManagedFolderId
api_type:
- schema
ms.assetid: 3efb7abb-0e91-4d8a-9fa2-3dec8bd17c30
description: O elemento ManagedFolderId contém a ID de pasta da pasta gerenciada.
ms.openlocfilehash: eacfe580342e6667fd9fc84ad953a5e4070b6ed7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465818"
---
# <a name="managedfolderid"></a><span data-ttu-id="bea32-103">ManagedFolderId</span><span class="sxs-lookup"><span data-stu-id="bea32-103">ManagedFolderId</span></span>

<span data-ttu-id="bea32-104">O elemento **ManagedFolderId** contém a ID de pasta da pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="bea32-104">The **ManagedFolderId** element contains the folder ID of the managed folder.</span></span> 
  
```xml
<ManagedFolderId/>
```

 <span data-ttu-id="bea32-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="bea32-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bea32-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="bea32-106">Attributes and elements</span></span>

<span data-ttu-id="bea32-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bea32-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bea32-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="bea32-108">Attributes</span></span>

<span data-ttu-id="bea32-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bea32-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bea32-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bea32-110">Child elements</span></span>

<span data-ttu-id="bea32-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bea32-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bea32-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bea32-112">Parent elements</span></span>

|<span data-ttu-id="bea32-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bea32-113">**Element**</span></span>|<span data-ttu-id="bea32-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bea32-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bea32-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="bea32-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="bea32-116">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="bea32-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bea32-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="bea32-117">Text value</span></span>

<span data-ttu-id="bea32-118">Um valor de texto é necessário para este elemento.</span><span class="sxs-lookup"><span data-stu-id="bea32-118">A text value is required for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bea32-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="bea32-119">Remarks</span></span>

<span data-ttu-id="bea32-120">O valor do identificador **ManagedFolderId** é o equivalente da propriedade **GUID** que é recuperada pelo `Get-ManagedFolder` comando do Microsoft Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bea32-120">The **ManagedFolderId** identifier value is the equivalent of the **Guid** property that is retrieved by the  `Get-ManagedFolder` Microsoft Windows Powershell command.</span></span> <span data-ttu-id="bea32-121">Também é o valor do atributo **objectGUID** da pasta gerenciada no serviço de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bea32-121">It is also the value of the **objectGUID** attribute for the managed folder in the Active Directory directory service.</span></span> 
  
<span data-ttu-id="bea32-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="bea32-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bea32-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="bea32-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bea32-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="bea32-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bea32-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bea32-125">Schema name</span></span>  <br/> |<span data-ttu-id="bea32-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="bea32-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="bea32-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bea32-127">Validation file</span></span>  <br/> |<span data-ttu-id="bea32-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bea32-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bea32-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="bea32-129">Can be empty</span></span>  <br/> |<span data-ttu-id="bea32-130">False</span><span class="sxs-lookup"><span data-stu-id="bea32-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bea32-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="bea32-131">See also</span></span>



[<span data-ttu-id="bea32-132">Operação CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="bea32-132">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="bea32-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bea32-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="bea32-134">Excluindo pastas</span><span class="sxs-lookup"><span data-stu-id="bea32-134">Deleting Folders</span></span>](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)
  
[<span data-ttu-id="bea32-135">Adicionando pastas gerenciadas</span><span class="sxs-lookup"><span data-stu-id="bea32-135">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

