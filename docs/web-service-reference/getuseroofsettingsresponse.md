---
title: GetUserOofSettingsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserOofSettingsResponse
api_type:
- schema
ms.assetid: 011cb38b-da3c-4b1b-8836-a6b212b511f6
description: O elemento GetUserOofSettingsResponse contém a mensagem de resposta e as configurações de fora do escritório (OOF) para um usuário.
ms.openlocfilehash: dc63b6d54471973ce5961a5a5ad6a23f6521fc0e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823693"
---
# <a name="getuseroofsettingsresponse"></a><span data-ttu-id="9f411-103">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="9f411-103">GetUserOofSettingsResponse</span></span>

<span data-ttu-id="9f411-104">O elemento **GetUserOofSettingsResponse** contém a mensagem de resposta e as configurações de fora do escritório (OOF) para um usuário.</span><span class="sxs-lookup"><span data-stu-id="9f411-104">The **GetUserOofSettingsResponse** element contains the response message and the Out of Office (OOF) settings for a user.</span></span> 
  
```xml
<GetUserOofSettingsResponse>
   <ResponseMessage>...</ResponseMessage>
   <OofSettings>...</OofSettings>
   <AllowExternalOof>...</AllowExternalOof>
</GetUserOofSettingsResponse>
```

 <span data-ttu-id="9f411-105">**GetUserOofSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="9f411-105">**GetUserOofSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f411-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9f411-106">Attributes and elements</span></span>

<span data-ttu-id="9f411-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9f411-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f411-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9f411-108">Attributes</span></span>

<span data-ttu-id="9f411-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9f411-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f411-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9f411-110">Child elements</span></span>

|<span data-ttu-id="9f411-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9f411-111">**Element**</span></span>|<span data-ttu-id="9f411-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9f411-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f411-113">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9f411-113">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="9f411-114">Fornece informações descritivas sobre o status de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f411-114">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="9f411-115">OofSettings</span><span class="sxs-lookup"><span data-stu-id="9f411-115">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="9f411-116">Contém as configurações de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="9f411-116">Contains the OOF settings.</span></span>  <br/> |
|[<span data-ttu-id="9f411-117">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="9f411-117">AllowExternalOof</span></span>](allowexternaloof.md) <br/> |<span data-ttu-id="9f411-118">Contém um valor que identifica a quem as mensagens de ausência temporária externas são enviadas.</span><span class="sxs-lookup"><span data-stu-id="9f411-118">Contains a value that identifies to whom external OOF messages are sent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f411-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9f411-119">Parent elements</span></span>

<span data-ttu-id="9f411-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9f411-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9f411-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="9f411-121">Remarks</span></span>

<span data-ttu-id="9f411-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="9f411-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f411-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9f411-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f411-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="9f411-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9f411-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9f411-125">Schema Name</span></span>  <br/> |<span data-ttu-id="9f411-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9f411-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9f411-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9f411-127">Validation File</span></span>  <br/> |<span data-ttu-id="9f411-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9f411-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9f411-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9f411-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="9f411-130">False</span><span class="sxs-lookup"><span data-stu-id="9f411-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f411-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="9f411-131">See also</span></span>



[<span data-ttu-id="9f411-132">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="9f411-132">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="9f411-133">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="9f411-133">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

