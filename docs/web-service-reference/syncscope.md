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
description: O elemento SyncScope Especifica se apenas itens ou itens e informações de pasta associada são retornados em uma resposta de sincronização.
ms.openlocfilehash: 847c0244a8847364e29ea584b0c0b721f00d3064
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837690"
---
# <a name="syncscope"></a><span data-ttu-id="30541-103">SyncScope</span><span class="sxs-lookup"><span data-stu-id="30541-103">SyncScope</span></span>

<span data-ttu-id="30541-104">O elemento **SyncScope** Especifica se apenas itens ou itens e informações de pasta associada são retornados em uma resposta de sincronização.</span><span class="sxs-lookup"><span data-stu-id="30541-104">The **SyncScope** element specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> 
  
```xml
<SyncScope>NormalItems or NormalAndAssociatedItems</SyncScope>
```

 <span data-ttu-id="30541-105">**SyncFolderItemsScopeType**</span><span class="sxs-lookup"><span data-stu-id="30541-105">**SyncFolderItemsScopeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30541-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="30541-106">Attributes and elements</span></span>

<span data-ttu-id="30541-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="30541-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30541-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="30541-108">Attributes</span></span>

<span data-ttu-id="30541-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="30541-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30541-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="30541-110">Child elements</span></span>

<span data-ttu-id="30541-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="30541-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="30541-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="30541-112">Parent elements</span></span>

|<span data-ttu-id="30541-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="30541-113">**Element**</span></span>|<span data-ttu-id="30541-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="30541-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30541-115">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="30541-115">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="30541-116">O elemento que define uma solicitação para sincronizar os itens em uma pasta de repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="30541-116">The element that defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> <span data-ttu-id="30541-117">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="30541-117">The following is the XPath expression to this element:</span></span>  <br/> <span data-ttu-id="30541-118">/ SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="30541-118">/SyncFolderItems</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="30541-119">Text value</span><span class="sxs-lookup"><span data-stu-id="30541-119">Text value</span></span>

<span data-ttu-id="30541-120">A tabela a seguir lista os valores possíveis para o elemento **SyncScope** .</span><span class="sxs-lookup"><span data-stu-id="30541-120">The following table lists the possible values for the **SyncScope** element.</span></span> 
  
<span data-ttu-id="30541-121">**Valores de elemento SyncScope**</span><span class="sxs-lookup"><span data-stu-id="30541-121">**SyncScope element values**</span></span>

|<span data-ttu-id="30541-122">**Valor**</span><span class="sxs-lookup"><span data-stu-id="30541-122">**Value**</span></span>|<span data-ttu-id="30541-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="30541-123">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="30541-124">NormalItems</span><span class="sxs-lookup"><span data-stu-id="30541-124">NormalItems</span></span>  <br/> |<span data-ttu-id="30541-125">Especifica que apenas os itens na pasta são retornados em uma resposta de sincronização.</span><span class="sxs-lookup"><span data-stu-id="30541-125">Specifies that only items in the folder are returned in a synchronization response.</span></span>  <br/> |
|<span data-ttu-id="30541-126">NormalAndAssociatedItems</span><span class="sxs-lookup"><span data-stu-id="30541-126">NormalAndAssociatedItems</span></span>  <br/> |<span data-ttu-id="30541-127">Especifica que ambos os itens da pasta e as informações da pasta associada são retornados em uma resposta de sincronização.</span><span class="sxs-lookup"><span data-stu-id="30541-127">Specifies that both items in the folder and folder associated information are returned in a synchronization response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="30541-128">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="30541-128">Remarks</span></span>

<span data-ttu-id="30541-129">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="30541-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30541-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="30541-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30541-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="30541-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="30541-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="30541-132">Schema Name</span></span>  <br/> |<span data-ttu-id="30541-133">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="30541-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="30541-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="30541-134">Validation File</span></span>  <br/> |<span data-ttu-id="30541-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="30541-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="30541-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="30541-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="30541-137">False</span><span class="sxs-lookup"><span data-stu-id="30541-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="30541-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="30541-138">See also</span></span>



[<span data-ttu-id="30541-139">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="30541-139">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="30541-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="30541-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

