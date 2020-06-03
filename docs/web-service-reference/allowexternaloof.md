---
title: AllowExternalOof
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllowExternalOof
api_type:
- schema
ms.assetid: e5387172-5b92-4bb1-8394-180e9c7ff771
description: O elemento AllowExternalOof contém um valor que identifica para quem as mensagens externas fora do escritório (OOF) são enviadas.
ms.openlocfilehash: e4934bc4bc86e1f9f764279a13ecaeca073d9e5d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464809"
---
# <a name="allowexternaloof"></a><span data-ttu-id="c4a8d-103">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="c4a8d-103">AllowExternalOof</span></span>

<span data-ttu-id="c4a8d-104">O elemento **AllowExternalOof** contém um valor que identifica para quem as mensagens externas fora do escritório (OOF) são enviadas.</span><span class="sxs-lookup"><span data-stu-id="c4a8d-104">The **AllowExternalOof** element contains a value that identifies to whom external Out of Office (OOF) messages are sent.</span></span> 
  
- [<span data-ttu-id="c4a8d-105">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="c4a8d-105">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
  
- [<span data-ttu-id="c4a8d-106">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="c4a8d-106">AllowExternalOof</span></span>](allowexternaloof.md)
  
```xml
<AllowExternalOof>None or Known or All</AllowExternalOof>
```

 <span data-ttu-id="c4a8d-107">**ExternalAudience**</span><span class="sxs-lookup"><span data-stu-id="c4a8d-107">**ExternalAudience**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c4a8d-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c4a8d-108">Attributes and elements</span></span>

<span data-ttu-id="c4a8d-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c4a8d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4a8d-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="c4a8d-110">Attributes</span></span>

<span data-ttu-id="c4a8d-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c4a8d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c4a8d-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c4a8d-112">Child elements</span></span>

<span data-ttu-id="c4a8d-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c4a8d-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c4a8d-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c4a8d-114">Parent elements</span></span>

|<span data-ttu-id="c4a8d-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c4a8d-115">**Element**</span></span>|<span data-ttu-id="c4a8d-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c4a8d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4a8d-117">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="c4a8d-117">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="c4a8d-118">Contém os resultados da resposta e as configurações de ausência temporária de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c4a8d-118">Contains the response results and the OOF settings for a user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c4a8d-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c4a8d-119">Text value</span></span>

<span data-ttu-id="c4a8d-120">Um valor de texto é necessário para este elemento.</span><span class="sxs-lookup"><span data-stu-id="c4a8d-120">A text value is required for this element.</span></span> <span data-ttu-id="c4a8d-121">A tabela a seguir lista os valores possíveis para este elemento.</span><span class="sxs-lookup"><span data-stu-id="c4a8d-121">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="c4a8d-122">**Valor**</span><span class="sxs-lookup"><span data-stu-id="c4a8d-122">**Value**</span></span>|<span data-ttu-id="c4a8d-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c4a8d-123">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c4a8d-124">**Nenhum**</span><span class="sxs-lookup"><span data-stu-id="c4a8d-124">**None**</span></span> <br/> |<span data-ttu-id="c4a8d-125">Remetentes de email fora da organização do usuário da caixa de correio que enviam mensagens ao usuário não receberão uma resposta de mensagem OOF externa.</span><span class="sxs-lookup"><span data-stu-id="c4a8d-125">E-mail senders outside the mailbox user's organization who send messages to the user will not receive an external OOF message response.</span></span>  <br/> |
|<span data-ttu-id="c4a8d-126">**Desconhecido**</span><span class="sxs-lookup"><span data-stu-id="c4a8d-126">**Known**</span></span> <br/> |<span data-ttu-id="c4a8d-127">Remetentes de email fora da organização do usuário da caixa de correio que enviam mensagens para o usuário receberão apenas uma resposta de mensagem OOF externa se o remetente estiver na lista de contatos do repositório do Exchange do usuário.</span><span class="sxs-lookup"><span data-stu-id="c4a8d-127">E-mail senders outside the mailbox user's organization who send messages to the user will only receive an external OOF message response if the sender is in the user's Exchange store contact list.</span></span>  <br/> |
|<span data-ttu-id="c4a8d-128">**All**</span><span class="sxs-lookup"><span data-stu-id="c4a8d-128">**All**</span></span> <br/> |<span data-ttu-id="c4a8d-129">Remetentes de email fora da organização do usuário da caixa de correio que enviam mensagens ao usuário receberão uma resposta de mensagem OOF externa.</span><span class="sxs-lookup"><span data-stu-id="c4a8d-129">E-mail senders outside the mailbox user's organization who send messages to the user will receive an external OOF message response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c4a8d-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="c4a8d-130">Remarks</span></span>

<span data-ttu-id="c4a8d-131">Este elemento compartilha o mesmo tipo que o elemento [ExternalAudience](externalaudience.md) .</span><span class="sxs-lookup"><span data-stu-id="c4a8d-131">This element shares the same type as the [ExternalAudience](externalaudience.md) element.</span></span> 
  
<span data-ttu-id="c4a8d-132">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c4a8d-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c4a8d-133">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c4a8d-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4a8d-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="c4a8d-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c4a8d-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c4a8d-135">Schema Name</span></span>  <br/> |<span data-ttu-id="c4a8d-136">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c4a8d-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c4a8d-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c4a8d-137">Validation File</span></span>  <br/> |<span data-ttu-id="c4a8d-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c4a8d-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c4a8d-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c4a8d-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="c4a8d-140">False</span><span class="sxs-lookup"><span data-stu-id="c4a8d-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c4a8d-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="c4a8d-141">See also</span></span>

- [<span data-ttu-id="c4a8d-142">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="c4a8d-142">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md) 
- [<span data-ttu-id="c4a8d-143">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="c4a8d-143">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

