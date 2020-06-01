---
title: GetInboxRulesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetInboxRulesResponse
api_type:
- schema
ms.assetid: 6d6c1950-c328-489a-94bf-a250fdbd5cd9
description: O elemento GetInboxRulesResponse define uma resposta a uma solicitação de operação GetInboxRules.
ms.openlocfilehash: 0d67d7eaf6ffbeeb790249190a98f252dbdb9c87
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458282"
---
# <a name="getinboxrulesresponse"></a><span data-ttu-id="a06c5-103">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="a06c5-103">GetInboxRulesResponse</span></span>

<span data-ttu-id="a06c5-104">O elemento **GetInboxRulesResponse** define uma resposta a uma solicitação de [operação GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a06c5-104">The **GetInboxRulesResponse** element defines a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span> 
  
```XML
<GetInboxRulesResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <OutlookRuleBlobExists/>
   <InboxRules/>
</GetInboxRulesResponse>
```

 <span data-ttu-id="a06c5-105">**GetInboxRulesResponseType**</span><span class="sxs-lookup"><span data-stu-id="a06c5-105">**GetInboxRulesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a06c5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a06c5-106">Attributes and elements</span></span>

<span data-ttu-id="a06c5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a06c5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a06c5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a06c5-108">Attributes</span></span>

|<span data-ttu-id="a06c5-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="a06c5-109">**Attribute**</span></span>|<span data-ttu-id="a06c5-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a06c5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a06c5-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="a06c5-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="a06c5-112">Descreve o status de uma resposta de [operação do GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a06c5-112">Describes the status of a [GetInboxRules operation](getinboxrules-operation.md) response.</span></span> <br/><br/><span data-ttu-id="a06c5-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="a06c5-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="a06c5-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="a06c5-114">-  Success</span></span>  <br/><span data-ttu-id="a06c5-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="a06c5-115">-  Warning</span></span>  <br/><span data-ttu-id="a06c5-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="a06c5-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="a06c5-117">Atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="a06c5-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="a06c5-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="a06c5-118">**Value**</span></span>|<span data-ttu-id="a06c5-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a06c5-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a06c5-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="a06c5-120">**Success**</span></span> <br/> |<span data-ttu-id="a06c5-121">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="a06c5-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="a06c5-122">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="a06c5-122">**Warning**</span></span> <br/> | <span data-ttu-id="a06c5-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="a06c5-123">Describes a request that was not processed.</span></span> <span data-ttu-id="a06c5-124">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="a06c5-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="a06c5-125">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="a06c5-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="a06c5-126">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="a06c5-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="a06c5-127">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="a06c5-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="a06c5-128">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="a06c5-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="a06c5-129">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="a06c5-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="a06c5-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="a06c5-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="a06c5-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="a06c5-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="a06c5-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="a06c5-132">**Error**</span></span> <br/> | <span data-ttu-id="a06c5-133">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="a06c5-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="a06c5-134">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="a06c5-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="a06c5-135">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="a06c5-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="a06c5-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="a06c5-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="a06c5-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="a06c5-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="a06c5-138">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="a06c5-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="a06c5-139">– Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="a06c5-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="a06c5-140">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="a06c5-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="a06c5-141">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="a06c5-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a06c5-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a06c5-142">Child elements</span></span>

|<span data-ttu-id="a06c5-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a06c5-143">**Element**</span></span>|<span data-ttu-id="a06c5-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a06c5-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a06c5-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="a06c5-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="a06c5-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="a06c5-146">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="a06c5-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a06c5-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="a06c5-148">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="a06c5-148">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="a06c5-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a06c5-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="a06c5-150">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="a06c5-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="a06c5-151">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="a06c5-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="a06c5-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="a06c5-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="a06c5-153">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="a06c5-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="a06c5-154">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="a06c5-154">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md) <br/> |<span data-ttu-id="a06c5-155">Indica se um blob de regra do Microsoft Outlook existe na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a06c5-155">Indicates whether a Microsoft Outlook rule blob exists in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a06c5-156">InboxRules</span><span class="sxs-lookup"><span data-stu-id="a06c5-156">InboxRules</span></span>](inboxrules.md) <br/> |<span data-ttu-id="a06c5-157">Representa uma matriz das regras na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a06c5-157">Represents an array of the rules in the user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a06c5-158">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a06c5-158">Parent elements</span></span>

<span data-ttu-id="a06c5-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a06c5-159">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a06c5-160">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a06c5-160">Text value</span></span>

<span data-ttu-id="a06c5-161">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a06c5-161">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a06c5-162">Comentários</span><span class="sxs-lookup"><span data-stu-id="a06c5-162">Remarks</span></span>

<span data-ttu-id="a06c5-163">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a06c5-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a06c5-164">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a06c5-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a06c5-165">Namespace</span><span class="sxs-lookup"><span data-stu-id="a06c5-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a06c5-166">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a06c5-166">Schema name</span></span>  <br/> |<span data-ttu-id="a06c5-167">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a06c5-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a06c5-168">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a06c5-168">Validation file</span></span>  <br/> |<span data-ttu-id="a06c5-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a06c5-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a06c5-170">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a06c5-170">Can be empty</span></span>  <br/> |<span data-ttu-id="a06c5-171">False</span><span class="sxs-lookup"><span data-stu-id="a06c5-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a06c5-172">Confira também</span><span class="sxs-lookup"><span data-stu-id="a06c5-172">See also</span></span>

- [<span data-ttu-id="a06c5-173">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="a06c5-173">GetInboxRules</span></span>](getinboxrules.md)
- [<span data-ttu-id="a06c5-174">Operação GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="a06c5-174">GetInboxRules operation</span></span>](getinboxrules-operation.md)

