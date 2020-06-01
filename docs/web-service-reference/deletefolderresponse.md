---
title: DeleteFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolderResponse
api_type:
- schema
ms.assetid: 27578bda-ef0a-4a33-bccc-2c1bc1735424
description: O elemento DeleteFolderResponse define uma resposta a uma solicitação DeleteFolder.
ms.openlocfilehash: 58b814662c769784c5fd682a9e039863a9787d8d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458485"
---
# <a name="deletefolderresponse"></a><span data-ttu-id="95bd8-103">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="95bd8-103">DeleteFolderResponse</span></span>

<span data-ttu-id="95bd8-104">O elemento **DeleteFolderResponse** define uma resposta a uma solicitação DeleteFolder.</span><span class="sxs-lookup"><span data-stu-id="95bd8-104">The **DeleteFolderResponse** element defines a response to a DeleteFolder request.</span></span> 
  
```xml
<DeleteFolderResponse>
   <ResponseMessages/>
</DeleteFolderResponse>
```

 <span data-ttu-id="95bd8-105">**DeleteFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="95bd8-105">**DeleteFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95bd8-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="95bd8-106">Attributes and elements</span></span>

<span data-ttu-id="95bd8-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="95bd8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95bd8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="95bd8-108">Attributes</span></span>

<span data-ttu-id="95bd8-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="95bd8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95bd8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="95bd8-110">Child elements</span></span>

|<span data-ttu-id="95bd8-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="95bd8-111">**Element**</span></span>|<span data-ttu-id="95bd8-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="95bd8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95bd8-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="95bd8-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="95bd8-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="95bd8-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="95bd8-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="95bd8-115">Parent elements</span></span>

<span data-ttu-id="95bd8-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="95bd8-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="95bd8-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="95bd8-117">Remarks</span></span>

<span data-ttu-id="95bd8-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="95bd8-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95bd8-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="95bd8-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95bd8-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="95bd8-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="95bd8-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="95bd8-121">Schema name</span></span>  <br/> |<span data-ttu-id="95bd8-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="95bd8-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="95bd8-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="95bd8-123">Validation file</span></span>  <br/> |<span data-ttu-id="95bd8-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="95bd8-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="95bd8-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="95bd8-125">Can be empty</span></span>  <br/> |<span data-ttu-id="95bd8-126">False</span><span class="sxs-lookup"><span data-stu-id="95bd8-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="95bd8-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="95bd8-127">See also</span></span>

- [<span data-ttu-id="95bd8-128">Operação DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="95bd8-128">DeleteFolder operation</span></span>](deletefolder-operation.md) 
- [<span data-ttu-id="95bd8-129">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="95bd8-129">DeleteFolder</span></span>](deletefolder.md)
- [<span data-ttu-id="95bd8-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="95bd8-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

