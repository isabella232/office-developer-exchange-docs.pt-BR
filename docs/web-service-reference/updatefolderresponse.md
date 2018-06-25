---
title: UpdateFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolderResponse
api_type:
- schema
ms.assetid: 31f47739-dc9c-46ba-9e3f-cce25dc85e6e
description: O elemento de UpdateFolderResponse define a resposta a uma solicitação de UpdateFolder.
ms.openlocfilehash: be85d8567f02760423aaee51799a5ef8e13a1729
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837888"
---
# <a name="updatefolderresponse"></a><span data-ttu-id="1330a-103">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="1330a-103">UpdateFolderResponse</span></span>

<span data-ttu-id="1330a-104">O elemento de **UpdateFolderResponse** define a resposta a uma solicitação de UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="1330a-104">The **UpdateFolderResponse** element defines the response to an UpdateFolder request.</span></span> 
  
```xml
<UpdateFolderResponse>
   <ResponseMessages/>
</UpdateFolderResponse>
```

 <span data-ttu-id="1330a-105">**UpdateFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="1330a-105">**UpdateFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1330a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1330a-106">Attributes and elements</span></span>

<span data-ttu-id="1330a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1330a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1330a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1330a-108">Attributes</span></span>

<span data-ttu-id="1330a-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1330a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1330a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1330a-110">Child elements</span></span>

|<span data-ttu-id="1330a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1330a-111">**Element**</span></span>|<span data-ttu-id="1330a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1330a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1330a-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1330a-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="1330a-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1330a-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1330a-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1330a-115">Parent elements</span></span>

<span data-ttu-id="1330a-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1330a-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1330a-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="1330a-117">Remarks</span></span>

<span data-ttu-id="1330a-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="1330a-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1330a-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1330a-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1330a-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="1330a-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1330a-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1330a-121">Schema name</span></span>  <br/> |<span data-ttu-id="1330a-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="1330a-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1330a-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1330a-123">Validation file</span></span>  <br/> |<span data-ttu-id="1330a-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1330a-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1330a-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="1330a-125">Can be empty</span></span>  <br/> |<span data-ttu-id="1330a-126">False</span><span class="sxs-lookup"><span data-stu-id="1330a-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1330a-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="1330a-127">See also</span></span>



[<span data-ttu-id="1330a-128">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="1330a-128">UpdateFolder operation</span></span>](updatefolder-operation.md)
  
[<span data-ttu-id="1330a-129">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="1330a-129">UpdateFolder</span></span>](updatefolder.md)


- [<span data-ttu-id="1330a-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1330a-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

