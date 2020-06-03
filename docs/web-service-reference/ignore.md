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
description: O elemento ignore identifica itens que serão ignorados durante a sincronização.
ms.openlocfilehash: b65d11d8c7655279dac0e7d3cbd13f8a9317540c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458569"
---
# <a name="ignore"></a><span data-ttu-id="c8820-103">Ignorar</span><span class="sxs-lookup"><span data-stu-id="c8820-103">Ignore</span></span>

<span data-ttu-id="c8820-104">O elemento **ignore** identifica itens que serão ignorados durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="c8820-104">The **Ignore** element identifies items to skip during synchronization.</span></span> 
  
[<span data-ttu-id="c8820-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="c8820-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="c8820-106">Ignore</span><span class="sxs-lookup"><span data-stu-id="c8820-106">Ignore</span></span>](ignore.md)
  
```xml
<Ignore>
   <ItemId/>
</Ignore>
```

 <span data-ttu-id="c8820-107">**ArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="c8820-107">**ArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c8820-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c8820-108">Attributes and elements</span></span>

<span data-ttu-id="c8820-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c8820-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8820-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="c8820-110">Attributes</span></span>

<span data-ttu-id="c8820-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8820-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c8820-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c8820-112">Child elements</span></span>

|<span data-ttu-id="c8820-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c8820-113">**Element**</span></span>|<span data-ttu-id="c8820-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c8820-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8820-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="c8820-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="c8820-116">Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c8820-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c8820-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c8820-117">Parent elements</span></span>

|<span data-ttu-id="c8820-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c8820-118">**Element**</span></span>|<span data-ttu-id="c8820-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c8820-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8820-120">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="c8820-120">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="c8820-121">Define uma solicitação para sincronizar itens em uma pasta do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c8820-121">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c8820-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="c8820-122">Remarks</span></span>

<span data-ttu-id="c8820-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c8820-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c8820-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c8820-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c8820-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="c8820-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c8820-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c8820-126">Schema name</span></span>  <br/> |<span data-ttu-id="c8820-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c8820-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c8820-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c8820-128">Validation file</span></span>  <br/> |<span data-ttu-id="c8820-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c8820-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c8820-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c8820-130">Can be empty</span></span>  <br/> |<span data-ttu-id="c8820-131">False</span><span class="sxs-lookup"><span data-stu-id="c8820-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c8820-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="c8820-132">See also</span></span>



[<span data-ttu-id="c8820-133">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="c8820-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="c8820-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c8820-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

