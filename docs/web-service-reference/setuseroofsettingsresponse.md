---
title: SetUserOofSettingsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetUserOofSettingsResponse
api_type:
- schema
ms.assetid: 8aa4025b-38df-4d63-a6a5-c3b932bec26e
description: O elemento SetUserOofSettingsResponse contém o resultado de uma tentativa de mensagem SetUserOofSettingsRequest.
ms.openlocfilehash: ab2eaaad1b7b094baad724ec56f4c26280f1f15f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825471"
---
# <a name="setuseroofsettingsresponse"></a><span data-ttu-id="47d4a-103">SetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="47d4a-103">SetUserOofSettingsResponse</span></span>

<span data-ttu-id="47d4a-104">O elemento **SetUserOofSettingsResponse** contém o resultado de uma tentativa de mensagem [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="47d4a-104">The **SetUserOofSettingsResponse** element contains the result of a [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) message attempt.</span></span> 
  
```xml
<SetUserOofSettingsResponse>
   <ResponseMessage>...</ResponseMessage>
<SetUserOofSettingsResponse>
```

 <span data-ttu-id="47d4a-105">**SetUserOofSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="47d4a-105">**SetUserOofSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="47d4a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="47d4a-106">Attributes and elements</span></span>

<span data-ttu-id="47d4a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="47d4a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47d4a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="47d4a-108">Attributes</span></span>

<span data-ttu-id="47d4a-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="47d4a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47d4a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="47d4a-110">Child elements</span></span>

|<span data-ttu-id="47d4a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="47d4a-111">**Element**</span></span>|<span data-ttu-id="47d4a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47d4a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47d4a-113">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="47d4a-113">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="47d4a-114">Fornece informações descritivas sobre o status de resposta.</span><span class="sxs-lookup"><span data-stu-id="47d4a-114">Provides descriptive information about the response status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="47d4a-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="47d4a-115">Parent elements</span></span>

<span data-ttu-id="47d4a-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="47d4a-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="47d4a-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="47d4a-117">Remarks</span></span>

<span data-ttu-id="47d4a-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="47d4a-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="47d4a-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="47d4a-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47d4a-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="47d4a-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="47d4a-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="47d4a-121">Schema Name</span></span>  <br/> |<span data-ttu-id="47d4a-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="47d4a-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="47d4a-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="47d4a-123">Validation File</span></span>  <br/> |<span data-ttu-id="47d4a-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="47d4a-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="47d4a-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="47d4a-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="47d4a-126">False</span><span class="sxs-lookup"><span data-stu-id="47d4a-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="47d4a-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="47d4a-127">See also</span></span>



[<span data-ttu-id="47d4a-128">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="47d4a-128">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

