---
title: Nomes de pastas
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderNames
api_type:
- schema
ms.assetid: 6cbe4083-5705-4695-a54e-8dab3e472662
description: O elemento de nomes de pastas contém uma matriz de nomeada pastas gerenciadas para adicionar uma caixa de correio.
ms.openlocfilehash: 819b3c2df1cfcae3a5d4a48539e369a00b1f7229
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752336"
---
# <a name="foldernames"></a><span data-ttu-id="eac4c-103">Nomes de pastas</span><span class="sxs-lookup"><span data-stu-id="eac4c-103">FolderNames</span></span>

<span data-ttu-id="eac4c-104">O elemento de **nomes de pastas** contém uma matriz de nomeada pastas gerenciadas para adicionar uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="eac4c-104">The **FolderNames** element contains an array of named managed folders to add to a mailbox.</span></span> 
  
[<span data-ttu-id="eac4c-105">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="eac4c-105">CreateManagedFolder</span></span>](createmanagedfolder.md)
  
[<span data-ttu-id="eac4c-106">Nomes de pastas</span><span class="sxs-lookup"><span data-stu-id="eac4c-106">FolderNames</span></span>](foldernames.md)
  
```xml
<FolderNames>
   <FolderName/>
</FolderNames>
```

 <span data-ttu-id="eac4c-107">**NonEmptyArrayOfFolderNamesType**</span><span class="sxs-lookup"><span data-stu-id="eac4c-107">**NonEmptyArrayOfFolderNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eac4c-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="eac4c-108">Attributes and elements</span></span>

<span data-ttu-id="eac4c-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="eac4c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eac4c-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="eac4c-110">Attributes</span></span>

<span data-ttu-id="eac4c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="eac4c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eac4c-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="eac4c-112">Child elements</span></span>

|<span data-ttu-id="eac4c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eac4c-113">**Element**</span></span>|<span data-ttu-id="eac4c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eac4c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eac4c-115">FolderName</span><span class="sxs-lookup"><span data-stu-id="eac4c-115">FolderName</span></span>](foldername.md) <br/> |<span data-ttu-id="eac4c-116">Identifica uma única pasta gerenciada para adicionar à caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="eac4c-116">Identifies a single managed folder to add to mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eac4c-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="eac4c-117">Parent elements</span></span>

|<span data-ttu-id="eac4c-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eac4c-118">**Element**</span></span>|<span data-ttu-id="eac4c-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eac4c-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eac4c-120">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="eac4c-120">CreateManagedFolder</span></span>](createmanagedfolder.md) <br/> |<span data-ttu-id="eac4c-121">O elemento raiz em uma solicitação para adicionar uma pasta gerenciada a uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="eac4c-121">The root element in a request to add a managed folder to a mailbox.</span></span>  <br/> <span data-ttu-id="eac4c-122">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="eac4c-122">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateManagedFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eac4c-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="eac4c-123">Remarks</span></span>

<span data-ttu-id="eac4c-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="eac4c-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eac4c-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="eac4c-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eac4c-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="eac4c-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="eac4c-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="eac4c-127">Schema Name</span></span>  <br/> |<span data-ttu-id="eac4c-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="eac4c-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="eac4c-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="eac4c-129">Validation File</span></span>  <br/> |<span data-ttu-id="eac4c-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="eac4c-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="eac4c-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="eac4c-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="eac4c-132">False</span><span class="sxs-lookup"><span data-stu-id="eac4c-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eac4c-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="eac4c-133">See also</span></span>



[<span data-ttu-id="eac4c-134">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="eac4c-134">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="eac4c-135">Localizando pastas</span><span class="sxs-lookup"><span data-stu-id="eac4c-135">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="eac4c-136">Adicionando pastas gerenciadas</span><span class="sxs-lookup"><span data-stu-id="eac4c-136">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

