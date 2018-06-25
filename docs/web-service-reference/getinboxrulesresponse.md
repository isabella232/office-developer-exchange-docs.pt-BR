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
description: O elemento de GetInboxRulesResponse define uma resposta a uma solicitação de operação GetInboxRules.
ms.openlocfilehash: d84064ab777fe13ded7727381842ddd1ee9d047d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752541"
---
# <a name="getinboxrulesresponse"></a><span data-ttu-id="7d92c-103">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="7d92c-103">GetInboxRulesResponse</span></span>

<span data-ttu-id="7d92c-104">O elemento de **GetInboxRulesResponse** define uma resposta a uma solicitação de [operação GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7d92c-104">The **GetInboxRulesResponse** element defines a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span> 
  
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

 <span data-ttu-id="7d92c-105">**GetInboxRulesResponseType**</span><span class="sxs-lookup"><span data-stu-id="7d92c-105">**GetInboxRulesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d92c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7d92c-106">Attributes and elements</span></span>

<span data-ttu-id="7d92c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7d92c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d92c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7d92c-108">Attributes</span></span>

|<span data-ttu-id="7d92c-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="7d92c-109">**Attribute**</span></span>|<span data-ttu-id="7d92c-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7d92c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7d92c-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="7d92c-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="7d92c-112">Descreve o status de uma resposta de [operação GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7d92c-112">Describes the status of a [GetInboxRules operation](getinboxrules-operation.md) response.</span></span> <br/><br/><span data-ttu-id="7d92c-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="7d92c-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="7d92c-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="7d92c-114">-  Success</span></span>  <br/><span data-ttu-id="7d92c-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="7d92c-115">-  Warning</span></span>  <br/><span data-ttu-id="7d92c-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="7d92c-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="7d92c-117">Atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="7d92c-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="7d92c-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="7d92c-118">**Value**</span></span>|<span data-ttu-id="7d92c-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7d92c-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7d92c-120">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="7d92c-120">**Success**</span></span> <br/> |<span data-ttu-id="7d92c-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="7d92c-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="7d92c-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="7d92c-122">**Warning**</span></span> <br/> | <span data-ttu-id="7d92c-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="7d92c-123">Describes a request that was not processed.</span></span> <span data-ttu-id="7d92c-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="7d92c-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="7d92c-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="7d92c-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="7d92c-126">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="7d92c-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="7d92c-127">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="7d92c-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="7d92c-128">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="7d92c-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="7d92c-129">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="7d92c-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="7d92c-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="7d92c-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="7d92c-131">-Uma cota for excedida.</span><span class="sxs-lookup"><span data-stu-id="7d92c-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="7d92c-132">**Erro**</span><span class="sxs-lookup"><span data-stu-id="7d92c-132">**Error**</span></span> <br/> | <span data-ttu-id="7d92c-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="7d92c-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="7d92c-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="7d92c-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="7d92c-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="7d92c-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="7d92c-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="7d92c-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="7d92c-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="7d92c-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="7d92c-138">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="7d92c-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="7d92c-139">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="7d92c-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="7d92c-140">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="7d92c-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="7d92c-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="7d92c-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7d92c-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7d92c-142">Child elements</span></span>

|<span data-ttu-id="7d92c-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7d92c-143">**Element**</span></span>|<span data-ttu-id="7d92c-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7d92c-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d92c-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="7d92c-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7d92c-146">Fornece a descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d92c-146">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7d92c-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7d92c-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7d92c-148">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d92c-148">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="7d92c-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7d92c-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7d92c-150">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="7d92c-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="7d92c-151">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="7d92c-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="7d92c-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="7d92c-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7d92c-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="7d92c-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="7d92c-154">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="7d92c-154">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md) <br/> |<span data-ttu-id="7d92c-155">Indica se um blob de regra do Microsoft Outlook existe na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="7d92c-155">Indicates whether a Microsoft Outlook rule blob exists in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="7d92c-156">InboxRules</span><span class="sxs-lookup"><span data-stu-id="7d92c-156">InboxRules</span></span>](inboxrules.md) <br/> |<span data-ttu-id="7d92c-157">Representa uma matriz das regras na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="7d92c-157">Represents an array of the rules in the user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7d92c-158">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7d92c-158">Parent elements</span></span>

<span data-ttu-id="7d92c-159">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7d92c-159">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="7d92c-160">Text value</span><span class="sxs-lookup"><span data-stu-id="7d92c-160">Text value</span></span>

<span data-ttu-id="7d92c-161">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7d92c-161">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7d92c-162">Comentários</span><span class="sxs-lookup"><span data-stu-id="7d92c-162">Remarks</span></span>

<span data-ttu-id="7d92c-163">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7d92c-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d92c-164">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7d92c-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d92c-165">Namespace</span><span class="sxs-lookup"><span data-stu-id="7d92c-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7d92c-166">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7d92c-166">Schema name</span></span>  <br/> |<span data-ttu-id="7d92c-167">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="7d92c-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7d92c-168">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7d92c-168">Validation file</span></span>  <br/> |<span data-ttu-id="7d92c-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7d92c-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7d92c-170">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="7d92c-170">Can be empty</span></span>  <br/> |<span data-ttu-id="7d92c-171">False</span><span class="sxs-lookup"><span data-stu-id="7d92c-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d92c-172">Ver também</span><span class="sxs-lookup"><span data-stu-id="7d92c-172">See also</span></span>

- [<span data-ttu-id="7d92c-173">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="7d92c-173">GetInboxRules</span></span>](getinboxrules.md)
- [<span data-ttu-id="7d92c-174">Operação GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="7d92c-174">GetInboxRules operation</span></span>](getinboxrules-operation.md)

