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
description: O elemento SendItem é o elemento raiz em uma solicitação para enviar um item no repositório do Exchange.
ms.openlocfilehash: 28f0d484dd079146c998cb7317bd2d80c6739e19
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530562"
---
# <a name="senditem"></a><span data-ttu-id="ec4ce-103">SendItem</span><span class="sxs-lookup"><span data-stu-id="ec4ce-103">SendItem</span></span>

<span data-ttu-id="ec4ce-104">O elemento **SendItem** é o elemento raiz em uma solicitação para enviar um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec4ce-104">The **SendItem** element is the root element in a request to send an item in the Exchange store.</span></span> 
  
```xml
<SendItem SaveItemToFolder="">
   <ItemIds/>
   <SavedItemFolderId/>
</SendItem>
```

 <span data-ttu-id="ec4ce-105">**SendItemType**</span><span class="sxs-lookup"><span data-stu-id="ec4ce-105">**SendItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec4ce-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ec4ce-106">Attributes and elements</span></span>

<span data-ttu-id="ec4ce-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ec4ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec4ce-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ec4ce-108">Attributes</span></span>

|<span data-ttu-id="ec4ce-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="ec4ce-109">**Attribute**</span></span>|<span data-ttu-id="ec4ce-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ec4ce-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ec4ce-111">**SaveItemToFolder**</span><span class="sxs-lookup"><span data-stu-id="ec4ce-111">**SaveItemToFolder**</span></span> <br/> |<span data-ttu-id="ec4ce-112">Identifica se uma cópia do item enviado é salva.</span><span class="sxs-lookup"><span data-stu-id="ec4ce-112">Identifies whether a copy of the sent item is saved.</span></span> <span data-ttu-id="ec4ce-113">A ação salvar depende do valor de **SaveItemToFolder** e se um elemento [SavedItemFolderId](saveditemfolderid.md) está presente na solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec4ce-113">The save action depends on the value of **SaveItemToFolder** and whether a [SavedItemFolderId](saveditemfolderid.md) element is present in the request.</span></span> <span data-ttu-id="ec4ce-114">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec4ce-114">This element is required.</span></span>  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a><span data-ttu-id="ec4ce-115">Atributo SaveItemToFolder</span><span class="sxs-lookup"><span data-stu-id="ec4ce-115">SaveItemToFolder Attribute</span></span>

|<span data-ttu-id="ec4ce-116">**Valor**</span><span class="sxs-lookup"><span data-stu-id="ec4ce-116">**Value**</span></span>|<span data-ttu-id="ec4ce-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ec4ce-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ec4ce-118">**verdadeiro**</span><span class="sxs-lookup"><span data-stu-id="ec4ce-118">**true**</span></span> <br/> |<span data-ttu-id="ec4ce-119">Se o elemento [SavedItemFolderId](saveditemfolderid.md) não estiver presente, o item será salvo na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="ec4ce-119">If the [SavedItemFolderId](saveditemfolderid.md) element is not present, the item is saved in the Sent Items folder.</span></span> <span data-ttu-id="ec4ce-120">Se o elemento [SavedItemFolderId](saveditemfolderid.md) estiver presente, o item será salvo na pasta especificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="ec4ce-120">If the [SavedItemFolderId](saveditemfolderid.md) element is present, the item is saved in the folder that is specified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
|<span data-ttu-id="ec4ce-121">**false**</span><span class="sxs-lookup"><span data-stu-id="ec4ce-121">**false**</span></span> <br/> |<span data-ttu-id="ec4ce-122">Se o elemento [SavedItemFolderId](saveditemfolderid.md) não estiver presente, o item não será salvo.</span><span class="sxs-lookup"><span data-stu-id="ec4ce-122">If the [SavedItemFolderId](saveditemfolderid.md) element is not present, the item is not saved.</span></span> <span data-ttu-id="ec4ce-123">Se o elemento [SavedItemFolderId](saveditemfolderid.md) estiver presente, uma resposta de erro será retornada com um elemento [ResponseCode](responsecode.md) que contém o valor de **ErrorInvalidSendItemSaveSettings** .</span><span class="sxs-lookup"><span data-stu-id="ec4ce-123">If the [SavedItemFolderId](saveditemfolderid.md) element is present, an error response will be returned with a [ResponseCode](responsecode.md) element that contains the **ErrorInvalidSendItemSaveSettings** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ec4ce-124">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ec4ce-124">Child elements</span></span>

|<span data-ttu-id="ec4ce-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ec4ce-125">**Element**</span></span>|<span data-ttu-id="ec4ce-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ec4ce-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec4ce-127">ItemIds</span><span class="sxs-lookup"><span data-stu-id="ec4ce-127">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="ec4ce-128">Contém as identidades exclusivas de itens, itens de ocorrência e itens mestre recorrentes que são usados para excluir, enviar, obter, mover ou copiar itens no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec4ce-128">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ec4ce-129">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="ec4ce-129">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="ec4ce-130">Identifica a pasta de destino para operações que atualizam, enviam e criam itens no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec4ce-130">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ec4ce-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ec4ce-131">Parent elements</span></span>

<span data-ttu-id="ec4ce-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec4ce-132">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ec4ce-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="ec4ce-133">Remarks</span></span>

<span data-ttu-id="ec4ce-134">Se um item na pasta Itens enviados é enviado, o item enviado é excluído e uma cópia dele é colocada na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="ec4ce-134">If an item in the Sent Items folder is sent, the sent item is deleted and a copy of it is put in the Sent Items folder.</span></span>
  
<span data-ttu-id="ec4ce-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="ec4ce-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec4ce-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ec4ce-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec4ce-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="ec4ce-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ec4ce-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ec4ce-138">Schema Name</span></span>  <br/> |<span data-ttu-id="ec4ce-139">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ec4ce-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ec4ce-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ec4ce-140">Validation File</span></span>  <br/> |<span data-ttu-id="ec4ce-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ec4ce-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ec4ce-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ec4ce-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="ec4ce-143">False</span><span class="sxs-lookup"><span data-stu-id="ec4ce-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ec4ce-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="ec4ce-144">See also</span></span>



[<span data-ttu-id="ec4ce-145">Operação SendItem</span><span class="sxs-lookup"><span data-stu-id="ec4ce-145">SendItem operation</span></span>](senditem-operation.md)

