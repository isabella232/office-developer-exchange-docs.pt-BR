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
description: O elemento GetFolder define uma solicitação para obter uma pasta de uma caixa de correio no repositório do Exchange.
ms.openlocfilehash: 41d2b1ab5fcd5d2d60c399e8070ca957ee4b66e7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458702"
---
# <a name="getfolder"></a><span data-ttu-id="7ed8c-103">GetFolder</span><span class="sxs-lookup"><span data-stu-id="7ed8c-103">GetFolder</span></span>

<span data-ttu-id="7ed8c-104">O elemento **GetFolder** define uma solicitação para obter uma pasta de uma caixa de correio no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-104">The **GetFolder** element defines a request to get a folder from a mailbox in the Exchange store.</span></span> 
  
```xml
<GetFolder>
   <FolderShape/>
   <FolderIds/>
</GetFolder>
```

 <span data-ttu-id="7ed8c-105">**GetFolderType**</span><span class="sxs-lookup"><span data-stu-id="7ed8c-105">**GetFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ed8c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="7ed8c-106">Attributes and elements</span></span>

<span data-ttu-id="7ed8c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ed8c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7ed8c-108">Attributes</span></span>

<span data-ttu-id="7ed8c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ed8c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ed8c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7ed8c-110">Child elements</span></span>

|<span data-ttu-id="7ed8c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7ed8c-111">**Element**</span></span>|<span data-ttu-id="7ed8c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7ed8c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ed8c-113">FolderShape</span><span class="sxs-lookup"><span data-stu-id="7ed8c-113">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="7ed8c-114">Identifica as propriedades a serem obtidas para cada pasta identificada no elemento [FolderIds](folderids.md) .</span><span class="sxs-lookup"><span data-stu-id="7ed8c-114">Identifies the properties to get for each folder identified in the [FolderIds](folderids.md) element.</span></span>  <br/> |
|[<span data-ttu-id="7ed8c-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="7ed8c-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="7ed8c-116">Contém uma matriz de identificadores de pasta que são usados para identificar pastas a serem obtidas de uma caixa de correio no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-116">Contains an array of folder identifiers that are used to identify folders to get from a mailbox in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7ed8c-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7ed8c-117">Parent elements</span></span>

<span data-ttu-id="7ed8c-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ed8c-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7ed8c-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="7ed8c-119">Remarks</span></span>

<span data-ttu-id="7ed8c-120">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ed8c-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="7ed8c-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ed8c-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="7ed8c-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7ed8c-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7ed8c-123">Schema Name</span></span>  <br/> |<span data-ttu-id="7ed8c-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="7ed8c-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="7ed8c-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7ed8c-125">Validation File</span></span>  <br/> |<span data-ttu-id="7ed8c-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7ed8c-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7ed8c-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7ed8c-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="7ed8c-128">False</span><span class="sxs-lookup"><span data-stu-id="7ed8c-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ed8c-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="7ed8c-129">See also</span></span>



[<span data-ttu-id="7ed8c-130">Operação GetFolder</span><span class="sxs-lookup"><span data-stu-id="7ed8c-130">GetFolder operation</span></span>](getfolder-operation.md)

