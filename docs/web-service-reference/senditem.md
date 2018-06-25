---
title: SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItem
api_type:
- schema
ms.assetid: a966da19-b05a-4504-ac98-91acc1667b9a
description: O elemento SendItem é o elemento raiz em uma solicitação para enviar um item no armazenamento do Exchange.
ms.openlocfilehash: c5ce52ee4643219aa31ae59e8b7d40d7a904c8ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825340"
---
# <a name="senditem"></a><span data-ttu-id="2e61b-103">SendItem</span><span class="sxs-lookup"><span data-stu-id="2e61b-103">SendItem</span></span>

<span data-ttu-id="2e61b-104">O elemento **SendItem** é o elemento raiz em uma solicitação para enviar um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2e61b-104">The **SendItem** element is the root element in a request to send an item in the Exchange store.</span></span> 
  
```xml
<SendItem SaveItemToFolder="">
   <ItemIds/>
   <SavedItemFolderId/>
</SendItem>
```

 <span data-ttu-id="2e61b-105">**SendItemType**</span><span class="sxs-lookup"><span data-stu-id="2e61b-105">**SendItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2e61b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2e61b-106">Attributes and elements</span></span>

<span data-ttu-id="2e61b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2e61b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2e61b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2e61b-108">Attributes</span></span>

|<span data-ttu-id="2e61b-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="2e61b-109">**Attribute**</span></span>|<span data-ttu-id="2e61b-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2e61b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2e61b-111">**SaveItemToFolder**</span><span class="sxs-lookup"><span data-stu-id="2e61b-111">**SaveItemToFolder**</span></span> <br/> |<span data-ttu-id="2e61b-112">Identifica se uma cópia do item enviado é salva.</span><span class="sxs-lookup"><span data-stu-id="2e61b-112">Identifies whether a copy of the sent item is saved.</span></span> <span data-ttu-id="2e61b-113">Salvar ação depende do valor de **SaveItemToFolder** e se um elemento [SavedItemFolderId](saveditemfolderid.md) está presente na solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e61b-113">The save action depends on the value of **SaveItemToFolder** and whether a [SavedItemFolderId](saveditemfolderid.md) element is present in the request.</span></span> <span data-ttu-id="2e61b-114">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e61b-114">This element is required.</span></span>  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a><span data-ttu-id="2e61b-115">Atributo SaveItemToFolder</span><span class="sxs-lookup"><span data-stu-id="2e61b-115">SaveItemToFolder Attribute</span></span>

|<span data-ttu-id="2e61b-116">**Valor**</span><span class="sxs-lookup"><span data-stu-id="2e61b-116">**Value**</span></span>|<span data-ttu-id="2e61b-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2e61b-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2e61b-118">**True**</span><span class="sxs-lookup"><span data-stu-id="2e61b-118">**true**</span></span> <br/> |<span data-ttu-id="2e61b-119">Se o elemento [SavedItemFolderId](saveditemfolderid.md) não estiver presente, o item é salvo na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="2e61b-119">If the [SavedItemFolderId](saveditemfolderid.md) element is not present, the item is saved in the Sent Items folder.</span></span> <span data-ttu-id="2e61b-120">Se o elemento [SavedItemFolderId](saveditemfolderid.md) estiver presente, o item é salvo na pasta especificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="2e61b-120">If the [SavedItemFolderId](saveditemfolderid.md) element is present, the item is saved in the folder that is specified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
|<span data-ttu-id="2e61b-121">**False**</span><span class="sxs-lookup"><span data-stu-id="2e61b-121">**false**</span></span> <br/> |<span data-ttu-id="2e61b-122">Se o elemento [SavedItemFolderId](saveditemfolderid.md) não estiver presente, o item não é salvo.</span><span class="sxs-lookup"><span data-stu-id="2e61b-122">If the [SavedItemFolderId](saveditemfolderid.md) element is not present, the item is not saved.</span></span> <span data-ttu-id="2e61b-123">Se o elemento [SavedItemFolderId](saveditemfolderid.md) estiver presente, uma resposta de erro será retornada com um elemento [ResponseCode](responsecode.md) que contém o valor de **ErrorInvalidSendItemSaveSettings** .</span><span class="sxs-lookup"><span data-stu-id="2e61b-123">If the [SavedItemFolderId](saveditemfolderid.md) element is present, an error response will be returned with a [ResponseCode](responsecode.md) element that contains the **ErrorInvalidSendItemSaveSettings** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2e61b-124">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2e61b-124">Child elements</span></span>

|<span data-ttu-id="2e61b-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2e61b-125">**Element**</span></span>|<span data-ttu-id="2e61b-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2e61b-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e61b-127">ItemIds</span><span class="sxs-lookup"><span data-stu-id="2e61b-127">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="2e61b-128">Contém as identidades exclusivas dos itens, itens de ocorrência e itens recorrentes de mestres que são usados para excluir, enviar, obter, mover ou copiar itens no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2e61b-128">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2e61b-129">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="2e61b-129">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="2e61b-130">Identifica a pasta de destino para operações de atualização, enviar e crie itens no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2e61b-130">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2e61b-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2e61b-131">Parent elements</span></span>

<span data-ttu-id="2e61b-132">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2e61b-132">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2e61b-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="2e61b-133">Remarks</span></span>

<span data-ttu-id="2e61b-134">Se um item na pasta Itens enviados é enviado, o item enviado será excluído e uma cópia dele é colocada na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="2e61b-134">If an item in the Sent Items folder is sent, the sent item is deleted and a copy of it is put in the Sent Items folder.</span></span>
  
<span data-ttu-id="2e61b-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="2e61b-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2e61b-136">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2e61b-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2e61b-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="2e61b-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2e61b-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2e61b-138">Schema Name</span></span>  <br/> |<span data-ttu-id="2e61b-139">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="2e61b-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2e61b-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2e61b-140">Validation File</span></span>  <br/> |<span data-ttu-id="2e61b-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2e61b-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2e61b-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2e61b-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="2e61b-143">False</span><span class="sxs-lookup"><span data-stu-id="2e61b-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2e61b-144">Ver também</span><span class="sxs-lookup"><span data-stu-id="2e61b-144">See also</span></span>



[<span data-ttu-id="2e61b-145">Operação SendItem</span><span class="sxs-lookup"><span data-stu-id="2e61b-145">SendItem operation</span></span>](senditem-operation.md)

