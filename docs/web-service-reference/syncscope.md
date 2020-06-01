---
title: SyncScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncScope
api_type:
- schema
ms.assetid: e0ca231f-0374-4844-8d4c-ada8da167920
description: O elemento SyncScope especifica se apenas itens ou itens e informações associadas à pasta são retornados em uma resposta de sincronização.
ms.openlocfilehash: 5ede26204c823a452189222075c784f24e98d188
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463031"
---
# <a name="syncscope"></a><span data-ttu-id="cb4d6-103">SyncScope</span><span class="sxs-lookup"><span data-stu-id="cb4d6-103">SyncScope</span></span>

<span data-ttu-id="cb4d6-104">O elemento **SyncScope** especifica se apenas itens ou itens e informações associadas à pasta são retornados em uma resposta de sincronização.</span><span class="sxs-lookup"><span data-stu-id="cb4d6-104">The **SyncScope** element specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> 
  
```xml
<SyncScope>NormalItems or NormalAndAssociatedItems</SyncScope>
```

 <span data-ttu-id="cb4d6-105">**SyncFolderItemsScopeType**</span><span class="sxs-lookup"><span data-stu-id="cb4d6-105">**SyncFolderItemsScopeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cb4d6-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cb4d6-106">Attributes and elements</span></span>

<span data-ttu-id="cb4d6-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cb4d6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb4d6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cb4d6-108">Attributes</span></span>

<span data-ttu-id="cb4d6-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb4d6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cb4d6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cb4d6-110">Child elements</span></span>

<span data-ttu-id="cb4d6-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cb4d6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cb4d6-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cb4d6-112">Parent elements</span></span>

|<span data-ttu-id="cb4d6-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cb4d6-113">**Element**</span></span>|<span data-ttu-id="cb4d6-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cb4d6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb4d6-115">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="cb4d6-115">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="cb4d6-116">O elemento que define uma solicitação para sincronizar itens em uma pasta do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb4d6-116">The element that defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> <span data-ttu-id="cb4d6-117">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="cb4d6-117">The following is the XPath expression to this element:</span></span>  <br/> <span data-ttu-id="cb4d6-118">/SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="cb4d6-118">/SyncFolderItems</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cb4d6-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="cb4d6-119">Text value</span></span>

<span data-ttu-id="cb4d6-120">A tabela a seguir lista os valores possíveis para o elemento **SyncScope** .</span><span class="sxs-lookup"><span data-stu-id="cb4d6-120">The following table lists the possible values for the **SyncScope** element.</span></span> 
  
<span data-ttu-id="cb4d6-121">**Valores do elemento SyncScope**</span><span class="sxs-lookup"><span data-stu-id="cb4d6-121">**SyncScope element values**</span></span>

|<span data-ttu-id="cb4d6-122">**Valor**</span><span class="sxs-lookup"><span data-stu-id="cb4d6-122">**Value**</span></span>|<span data-ttu-id="cb4d6-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cb4d6-123">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cb4d6-124">NormalItems</span><span class="sxs-lookup"><span data-stu-id="cb4d6-124">NormalItems</span></span>  <br/> |<span data-ttu-id="cb4d6-125">Especifica que somente os itens na pasta são retornados em uma resposta de sincronização.</span><span class="sxs-lookup"><span data-stu-id="cb4d6-125">Specifies that only items in the folder are returned in a synchronization response.</span></span>  <br/> |
|<span data-ttu-id="cb4d6-126">NormalAndAssociatedItems</span><span class="sxs-lookup"><span data-stu-id="cb4d6-126">NormalAndAssociatedItems</span></span>  <br/> |<span data-ttu-id="cb4d6-127">Especifica que os dois itens na pasta e as informações associadas à pasta são retornados em uma resposta de sincronização.</span><span class="sxs-lookup"><span data-stu-id="cb4d6-127">Specifies that both items in the folder and folder associated information are returned in a synchronization response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cb4d6-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="cb4d6-128">Remarks</span></span>

<span data-ttu-id="cb4d6-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="cb4d6-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cb4d6-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cb4d6-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cb4d6-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="cb4d6-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cb4d6-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cb4d6-132">Schema Name</span></span>  <br/> |<span data-ttu-id="cb4d6-133">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="cb4d6-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cb4d6-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cb4d6-134">Validation File</span></span>  <br/> |<span data-ttu-id="cb4d6-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cb4d6-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cb4d6-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cb4d6-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="cb4d6-137">False</span><span class="sxs-lookup"><span data-stu-id="cb4d6-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cb4d6-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="cb4d6-138">See also</span></span>



[<span data-ttu-id="cb4d6-139">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="cb4d6-139">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="cb4d6-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cb4d6-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

