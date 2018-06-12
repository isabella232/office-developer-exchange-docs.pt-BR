---
title: CreateManagedFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolderResponse
api_type:
- schema
ms.assetid: 99062401-d356-4ce7-a5d0-c8c7aab99912
description: O elemento de CreateManagedFolderResponse define uma resposta a uma solicitação de CreateManagedFolder.
ms.openlocfilehash: fc486a197b7b0a0ed7310dda88d4bf8735f99876
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751620"
---
# <a name="createmanagedfolderresponse"></a><span data-ttu-id="99636-103">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="99636-103">CreateManagedFolderResponse</span></span>

<span data-ttu-id="99636-104">O elemento de **CreateManagedFolderResponse** define uma resposta a uma solicitação de CreateManagedFolder.</span><span class="sxs-lookup"><span data-stu-id="99636-104">The **CreateManagedFolderResponse** element defines a response to a CreateManagedFolder request.</span></span> 
  
```xml
<CreateManagedFolderResponse>
   <ResponseMessages/>
</CreateManagedFolderResponse>
```

 <span data-ttu-id="99636-105">**CreateManagedFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="99636-105">**CreateManagedFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="99636-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="99636-106">Attributes and elements</span></span>

<span data-ttu-id="99636-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="99636-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99636-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="99636-108">Attributes</span></span>

<span data-ttu-id="99636-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="99636-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="99636-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="99636-110">Child elements</span></span>

|<span data-ttu-id="99636-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="99636-111">**Element**</span></span>|<span data-ttu-id="99636-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="99636-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99636-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="99636-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="99636-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="99636-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="99636-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="99636-115">Parent elements</span></span>

<span data-ttu-id="99636-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="99636-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="99636-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="99636-117">Remarks</span></span>

<span data-ttu-id="99636-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="99636-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99636-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="99636-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99636-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="99636-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="99636-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="99636-121">Schema name</span></span>  <br/> |<span data-ttu-id="99636-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="99636-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="99636-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="99636-123">Validation file</span></span>  <br/> |<span data-ttu-id="99636-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="99636-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="99636-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="99636-125">Can be empty</span></span>  <br/> |<span data-ttu-id="99636-126">False</span><span class="sxs-lookup"><span data-stu-id="99636-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="99636-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="99636-127">See also</span></span>



[<span data-ttu-id="99636-128">Operação CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="99636-128">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)
  
[<span data-ttu-id="99636-129">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="99636-129">CreateManagedFolder</span></span>](createmanagedfolder.md)


- [<span data-ttu-id="99636-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="99636-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

