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
description: O elemento AllowExternalOof contém um valor que identifica a quem as mensagens de ausência temporária externas são enviadas.
ms.openlocfilehash: 1c87a51676bf6e44b2e650a4e973d0ab89a52e31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751084"
---
# <a name="allowexternaloof"></a><span data-ttu-id="aa4d5-103">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="aa4d5-103">AllowExternalOof</span></span>

<span data-ttu-id="aa4d5-104">O elemento **AllowExternalOof** contém um valor que identifica a quem as mensagens de ausência temporária externas são enviadas.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-104">The **AllowExternalOof** element contains a value that identifies to whom external Out of Office (OOF) messages are sent.</span></span> 
  
- [<span data-ttu-id="aa4d5-105">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="aa4d5-105">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
  
- [<span data-ttu-id="aa4d5-106">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="aa4d5-106">AllowExternalOof</span></span>](allowexternaloof.md)
  
```xml
<AllowExternalOof>None or Known or All</AllowExternalOof>
```

 <span data-ttu-id="aa4d5-107">**ExternalAudience**</span><span class="sxs-lookup"><span data-stu-id="aa4d5-107">**ExternalAudience**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa4d5-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="aa4d5-108">Attributes and elements</span></span>

<span data-ttu-id="aa4d5-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa4d5-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="aa4d5-110">Attributes</span></span>

<span data-ttu-id="aa4d5-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa4d5-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="aa4d5-112">Child elements</span></span>

<span data-ttu-id="aa4d5-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aa4d5-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="aa4d5-114">Parent elements</span></span>

|<span data-ttu-id="aa4d5-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aa4d5-115">**Element**</span></span>|<span data-ttu-id="aa4d5-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aa4d5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa4d5-117">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="aa4d5-117">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="aa4d5-118">Contém os resultados de resposta e as configurações de ausência temporária para um usuário.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-118">Contains the response results and the OOF settings for a user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aa4d5-119">Text value</span><span class="sxs-lookup"><span data-stu-id="aa4d5-119">Text value</span></span>

<span data-ttu-id="aa4d5-120">Um valor de texto é necessário para esse elemento.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-120">A text value is required for this element.</span></span> <span data-ttu-id="aa4d5-121">A tabela a seguir lista os valores possíveis para esse elemento.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-121">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="aa4d5-122">**Valor**</span><span class="sxs-lookup"><span data-stu-id="aa4d5-122">**Value**</span></span>|<span data-ttu-id="aa4d5-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aa4d5-123">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aa4d5-124">**None**</span><span class="sxs-lookup"><span data-stu-id="aa4d5-124">**None**</span></span> <br/> |<span data-ttu-id="aa4d5-125">Remetentes de email fora da organização do usuário da caixa de correio que enviar mensagens para o usuário não receberá uma resposta de mensagem de ausência temporária externa.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-125">E-mail senders outside the mailbox user's organization who send messages to the user will not receive an external OOF message response.</span></span>  <br/> |
|<span data-ttu-id="aa4d5-126">**Conhecidos**</span><span class="sxs-lookup"><span data-stu-id="aa4d5-126">**Known**</span></span> <br/> |<span data-ttu-id="aa4d5-127">Remetentes de email fora da organização do usuário da caixa de correio que enviar mensagens para o usuário receberá uma resposta de mensagem de ausência temporária externa apenas se o remetente está no Exchange do usuário armazenam a lista de contatos.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-127">E-mail senders outside the mailbox user's organization who send messages to the user will only receive an external OOF message response if the sender is in the user's Exchange store contact list.</span></span>  <br/> |
|<span data-ttu-id="aa4d5-128">**All**</span><span class="sxs-lookup"><span data-stu-id="aa4d5-128">**All**</span></span> <br/> |<span data-ttu-id="aa4d5-129">Remetentes de email fora da organização do usuário da caixa de correio que enviar mensagens para o usuário receberá uma resposta de mensagem de ausência temporária externa.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-129">E-mail senders outside the mailbox user's organization who send messages to the user will receive an external OOF message response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aa4d5-130">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="aa4d5-130">Remarks</span></span>

<span data-ttu-id="aa4d5-131">Esse elemento compartilha o mesmo tipo de elemento [ExternalAudience](externalaudience.md) .</span><span class="sxs-lookup"><span data-stu-id="aa4d5-131">This element shares the same type as the [ExternalAudience](externalaudience.md) element.</span></span> 
  
<span data-ttu-id="aa4d5-132">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa4d5-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="aa4d5-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa4d5-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="aa4d5-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aa4d5-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="aa4d5-135">Schema Name</span></span>  <br/> |<span data-ttu-id="aa4d5-136">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="aa4d5-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aa4d5-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="aa4d5-137">Validation File</span></span>  <br/> |<span data-ttu-id="aa4d5-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="aa4d5-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aa4d5-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="aa4d5-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa4d5-140">False</span><span class="sxs-lookup"><span data-stu-id="aa4d5-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa4d5-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="aa4d5-141">See also</span></span>

- [<span data-ttu-id="aa4d5-142">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="aa4d5-142">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md) 
- [<span data-ttu-id="aa4d5-143">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="aa4d5-143">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

