---
title: CreateFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolderResponse
api_type:
- schema
ms.assetid: 158adecc-491a-47d9-af73-acc2cd3f8566
description: O elemento CreateFolderResponse define uma resposta a uma solicitação CreateFolder.
ms.openlocfilehash: c51fb17f0b0f9c3dd1db8b0ff31f230fac37ce67
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458877"
---
# <a name="createfolderresponse"></a><span data-ttu-id="58d02-103">CreateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="58d02-103">CreateFolderResponse</span></span>

<span data-ttu-id="58d02-104">O elemento **CreateFolderResponse** define uma resposta a uma solicitação CreateFolder.</span><span class="sxs-lookup"><span data-stu-id="58d02-104">The **CreateFolderResponse** element defines a response to a CreateFolder request.</span></span> 
  
```xml
<CreateFolderResponse>
   <ResponseMessages/>
</CreateFolderResponse>
```

 <span data-ttu-id="58d02-105">**CreateFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="58d02-105">**CreateFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58d02-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="58d02-106">Attributes and elements</span></span>

<span data-ttu-id="58d02-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="58d02-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58d02-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="58d02-108">Attributes</span></span>

<span data-ttu-id="58d02-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58d02-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58d02-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="58d02-110">Child elements</span></span>

|<span data-ttu-id="58d02-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="58d02-111">**Element**</span></span>|<span data-ttu-id="58d02-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="58d02-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58d02-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="58d02-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="58d02-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="58d02-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="58d02-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="58d02-115">Parent elements</span></span>

<span data-ttu-id="58d02-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58d02-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="58d02-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="58d02-117">Remarks</span></span>

<span data-ttu-id="58d02-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="58d02-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="58d02-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="58d02-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58d02-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="58d02-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="58d02-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="58d02-121">Schema name</span></span>  <br/> |<span data-ttu-id="58d02-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="58d02-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="58d02-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="58d02-123">Validation file</span></span>  <br/> |<span data-ttu-id="58d02-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="58d02-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="58d02-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="58d02-125">Can be empty</span></span>  <br/> |<span data-ttu-id="58d02-126">False</span><span class="sxs-lookup"><span data-stu-id="58d02-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="58d02-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="58d02-127">See also</span></span>



[<span data-ttu-id="58d02-128">Operação CreateFolder</span><span class="sxs-lookup"><span data-stu-id="58d02-128">CreateFolder operation</span></span>](createfolder-operation.md)
  
[<span data-ttu-id="58d02-129">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="58d02-129">CreateFolder</span></span>](createfolder.md)


- [<span data-ttu-id="58d02-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="58d02-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

