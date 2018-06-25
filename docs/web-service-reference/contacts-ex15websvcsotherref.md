---
title: Contatos
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contacts
api_type:
- schema
ms.assetid: 0cc67cdf-9707-45e7-92c6-fa83a016cdbe
description: O elemento de contatos contém uma lista de contatos que estão associados uma tarefa.
ms.openlocfilehash: da7963d30f58f7da52e76e3f7f1d0f7fd68abf74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751440"
---
# <a name="contacts"></a><span data-ttu-id="f897b-103">Contatos</span><span class="sxs-lookup"><span data-stu-id="f897b-103">Contacts</span></span>

<span data-ttu-id="f897b-104">O elemento de **Contatos** contém uma lista de contatos que estão associados uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="f897b-104">The **Contacts** element contains a list of contacts that are associated with a task.</span></span> 
  
```xml
<Contacts>
   <String/>
</Contacts>
```

 <span data-ttu-id="f897b-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="f897b-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f897b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f897b-106">Attributes and elements</span></span>

<span data-ttu-id="f897b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f897b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f897b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f897b-108">Attributes</span></span>

<span data-ttu-id="f897b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f897b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f897b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f897b-110">Child elements</span></span>

|<span data-ttu-id="f897b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f897b-111">**Element**</span></span>|<span data-ttu-id="f897b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f897b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f897b-113">String</span><span class="sxs-lookup"><span data-stu-id="f897b-113">String</span></span>](string.md) <br/> |<span data-ttu-id="f897b-114">Representa uma lista separada por vírgulas de nomes de contato.</span><span class="sxs-lookup"><span data-stu-id="f897b-114">Represents a comma-separated list of contact names.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f897b-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f897b-115">Parent elements</span></span>

|<span data-ttu-id="f897b-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f897b-116">**Element**</span></span>|<span data-ttu-id="f897b-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f897b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f897b-118">Task</span><span class="sxs-lookup"><span data-stu-id="f897b-118">Task</span></span>](task.md) <br/> |<span data-ttu-id="f897b-119">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f897b-119">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f897b-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="f897b-120">Remarks</span></span>

<span data-ttu-id="f897b-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="f897b-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f897b-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f897b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f897b-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="f897b-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f897b-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f897b-124">Schema name</span></span>  <br/> |<span data-ttu-id="f897b-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f897b-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="f897b-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f897b-126">Validation file</span></span>  <br/> |<span data-ttu-id="f897b-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f897b-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f897b-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f897b-128">Can be empty</span></span>  <br/> |<span data-ttu-id="f897b-129">False</span><span class="sxs-lookup"><span data-stu-id="f897b-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f897b-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="f897b-130">See also</span></span>



- [<span data-ttu-id="f897b-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f897b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

