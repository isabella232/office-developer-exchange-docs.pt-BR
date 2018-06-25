---
title: Ignorar
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Ignore
api_type:
- schema
ms.assetid: 7789eec5-ceec-43f2-84d5-d0d15b734076
description: O elemento ignorar identifica os itens a serem ignorados durante a sincronização.
ms.openlocfilehash: 0ecff9bfeb1257552b7e52c0115e9e814edecd4b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823858"
---
# <a name="ignore"></a><span data-ttu-id="60a3f-103">Ignorar</span><span class="sxs-lookup"><span data-stu-id="60a3f-103">Ignore</span></span>

<span data-ttu-id="60a3f-104">O elemento **Ignorar** identifica os itens a serem ignorados durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="60a3f-104">The **Ignore** element identifies items to skip during synchronization.</span></span> 
  
[<span data-ttu-id="60a3f-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="60a3f-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="60a3f-106">Ignore</span><span class="sxs-lookup"><span data-stu-id="60a3f-106">Ignore</span></span>](ignore.md)
  
```xml
<Ignore>
   <ItemId/>
</Ignore>
```

 <span data-ttu-id="60a3f-107">**ArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="60a3f-107">**ArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60a3f-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="60a3f-108">Attributes and elements</span></span>

<span data-ttu-id="60a3f-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="60a3f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60a3f-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="60a3f-110">Attributes</span></span>

<span data-ttu-id="60a3f-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="60a3f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="60a3f-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="60a3f-112">Child elements</span></span>

|<span data-ttu-id="60a3f-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="60a3f-113">**Element**</span></span>|<span data-ttu-id="60a3f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="60a3f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60a3f-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="60a3f-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="60a3f-116">Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="60a3f-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="60a3f-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="60a3f-117">Parent elements</span></span>

|<span data-ttu-id="60a3f-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="60a3f-118">**Element**</span></span>|<span data-ttu-id="60a3f-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="60a3f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60a3f-120">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="60a3f-120">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="60a3f-121">Define uma solicitação para sincronizar os itens em uma pasta de repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="60a3f-121">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="60a3f-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="60a3f-122">Remarks</span></span>

<span data-ttu-id="60a3f-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="60a3f-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60a3f-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="60a3f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60a3f-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="60a3f-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="60a3f-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="60a3f-126">Schema name</span></span>  <br/> |<span data-ttu-id="60a3f-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="60a3f-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="60a3f-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="60a3f-128">Validation file</span></span>  <br/> |<span data-ttu-id="60a3f-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="60a3f-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="60a3f-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="60a3f-130">Can be empty</span></span>  <br/> |<span data-ttu-id="60a3f-131">False</span><span class="sxs-lookup"><span data-stu-id="60a3f-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="60a3f-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="60a3f-132">See also</span></span>



[<span data-ttu-id="60a3f-133">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="60a3f-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="60a3f-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="60a3f-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

