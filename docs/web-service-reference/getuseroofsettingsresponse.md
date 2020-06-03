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
description: O elemento GetUserOofSettingsResponse contém a mensagem de resposta e as configurações de ausência temporária (OOF) para um usuário.
ms.openlocfilehash: f7f28c67fd36630ffb5294ab35c0fef2f467ba22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457813"
---
# <a name="getuseroofsettingsresponse"></a><span data-ttu-id="d37d3-103">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="d37d3-103">GetUserOofSettingsResponse</span></span>

<span data-ttu-id="d37d3-104">O elemento **GetUserOofSettingsResponse** contém a mensagem de resposta e as configurações de ausência temporária (OOF) para um usuário.</span><span class="sxs-lookup"><span data-stu-id="d37d3-104">The **GetUserOofSettingsResponse** element contains the response message and the Out of Office (OOF) settings for a user.</span></span> 
  
```xml
<GetUserOofSettingsResponse>
   <ResponseMessage>...</ResponseMessage>
   <OofSettings>...</OofSettings>
   <AllowExternalOof>...</AllowExternalOof>
</GetUserOofSettingsResponse>
```

 <span data-ttu-id="d37d3-105">**GetUserOofSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="d37d3-105">**GetUserOofSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d37d3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d37d3-106">Attributes and elements</span></span>

<span data-ttu-id="d37d3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d37d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d37d3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d37d3-108">Attributes</span></span>

<span data-ttu-id="d37d3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d37d3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d37d3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d37d3-110">Child elements</span></span>

|<span data-ttu-id="d37d3-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d37d3-111">**Element**</span></span>|<span data-ttu-id="d37d3-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d37d3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d37d3-113">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d37d3-113">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="d37d3-114">Fornece informações descritivas sobre o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="d37d3-114">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="d37d3-115">OofSettings</span><span class="sxs-lookup"><span data-stu-id="d37d3-115">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="d37d3-116">Contém as configurações de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="d37d3-116">Contains the OOF settings.</span></span>  <br/> |
|[<span data-ttu-id="d37d3-117">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="d37d3-117">AllowExternalOof</span></span>](allowexternaloof.md) <br/> |<span data-ttu-id="d37d3-118">Contém um valor que identifica a quem mensagens externas OOF são enviadas.</span><span class="sxs-lookup"><span data-stu-id="d37d3-118">Contains a value that identifies to whom external OOF messages are sent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d37d3-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d37d3-119">Parent elements</span></span>

<span data-ttu-id="d37d3-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d37d3-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d37d3-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="d37d3-121">Remarks</span></span>

<span data-ttu-id="d37d3-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d37d3-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d37d3-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d37d3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d37d3-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="d37d3-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d37d3-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d37d3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d37d3-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d37d3-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d37d3-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d37d3-127">Validation File</span></span>  <br/> |<span data-ttu-id="d37d3-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d37d3-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d37d3-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d37d3-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="d37d3-130">False</span><span class="sxs-lookup"><span data-stu-id="d37d3-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d37d3-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="d37d3-131">See also</span></span>



[<span data-ttu-id="d37d3-132">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d37d3-132">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="d37d3-133">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d37d3-133">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

