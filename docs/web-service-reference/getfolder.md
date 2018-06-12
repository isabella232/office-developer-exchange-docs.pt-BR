---
title: GetFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetFolder
api_type:
- schema
ms.assetid: 34e4c9ea-adcd-46bd-ae8f-7abb256c585a
description: O elemento de GetFolder define uma solicitação para fazer uma pasta a partir de uma caixa de correio no armazenamento do Exchange.
ms.openlocfilehash: 233da6ce57683350d4a13f6585593ac09438f0e6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752507"
---
# <a name="getfolder"></a><span data-ttu-id="d0683-103">GetFolder</span><span class="sxs-lookup"><span data-stu-id="d0683-103">GetFolder</span></span>

<span data-ttu-id="d0683-104">O elemento de **GetFolder** define uma solicitação para fazer uma pasta a partir de uma caixa de correio no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0683-104">The **GetFolder** element defines a request to get a folder from a mailbox in the Exchange store.</span></span> 
  
```xml
<GetFolder>
   <FolderShape/>
   <FolderIds/>
</GetFolder>
```

 <span data-ttu-id="d0683-105">**GetFolderType**</span><span class="sxs-lookup"><span data-stu-id="d0683-105">**GetFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0683-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d0683-106">Attributes and elements</span></span>

<span data-ttu-id="d0683-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d0683-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0683-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d0683-108">Attributes</span></span>

<span data-ttu-id="d0683-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d0683-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0683-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d0683-110">Child elements</span></span>

|<span data-ttu-id="d0683-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d0683-111">**Element**</span></span>|<span data-ttu-id="d0683-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d0683-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0683-113">FolderShape</span><span class="sxs-lookup"><span data-stu-id="d0683-113">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="d0683-114">Identifica as propriedades para obter para cada pasta identificada no elemento [FolderIds](folderids.md) .</span><span class="sxs-lookup"><span data-stu-id="d0683-114">Identifies the properties to get for each folder identified in the [FolderIds](folderids.md) element.</span></span>  <br/> |
|[<span data-ttu-id="d0683-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="d0683-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="d0683-116">Contém uma matriz de identificadores de pasta que são usados para identificar pastas para fazer a partir de uma caixa de correio no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0683-116">Contains an array of folder identifiers that are used to identify folders to get from a mailbox in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d0683-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d0683-117">Parent elements</span></span>

<span data-ttu-id="d0683-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d0683-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d0683-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="d0683-119">Remarks</span></span>

<span data-ttu-id="d0683-120">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d0683-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0683-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d0683-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0683-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="d0683-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d0683-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d0683-123">Schema Name</span></span>  <br/> |<span data-ttu-id="d0683-124">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="d0683-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="d0683-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d0683-125">Validation File</span></span>  <br/> |<span data-ttu-id="d0683-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d0683-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d0683-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d0683-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="d0683-128">False</span><span class="sxs-lookup"><span data-stu-id="d0683-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0683-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="d0683-129">See also</span></span>



[<span data-ttu-id="d0683-130">Operação GetFolder</span><span class="sxs-lookup"><span data-stu-id="d0683-130">GetFolder operation</span></span>](getfolder-operation.md)

