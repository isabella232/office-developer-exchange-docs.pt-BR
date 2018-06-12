---
title: ResolveNamesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNamesResponseMessage
api_type:
- schema
ms.assetid: edcdaf58-ef63-412e-8c58-409213e6ab0d
description: O elemento ResolveNamesResponseMessage contém o status e o resultado de uma solicitação de operação ResolveNames.
ms.openlocfilehash: 953a1f0b19c078d969ffe175c22df02b58c5e939
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825170"
---
# <a name="resolvenamesresponsemessage"></a><span data-ttu-id="0bb85-103">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0bb85-103">ResolveNamesResponseMessage</span></span>

<span data-ttu-id="0bb85-104">O elemento **ResolveNamesResponseMessage** contém o status e o resultado de uma solicitação de [operação ResolveNames](resolvenames-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0bb85-104">The **ResolveNamesResponseMessage** element contains the status and result of a [ResolveNames operation](resolvenames-operation.md) request.</span></span> 
  
- [<span data-ttu-id="0bb85-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="0bb85-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md) 
- [<span data-ttu-id="0bb85-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0bb85-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="0bb85-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0bb85-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
```xml
<ResolveNamesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResolutionSet/>
</ResolveNamesResponseMessage>
```

 <span data-ttu-id="0bb85-108">**ResolveNamesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0bb85-108">**ResolveNamesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0bb85-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0bb85-109">Attributes and elements</span></span>

<span data-ttu-id="0bb85-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0bb85-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0bb85-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="0bb85-111">Attributes</span></span>

|<span data-ttu-id="0bb85-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="0bb85-112">**Attribute**</span></span>|<span data-ttu-id="0bb85-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0bb85-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0bb85-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="0bb85-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="0bb85-115">Descreve o status de uma resposta [ResolveNames operação](resolvenames-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0bb85-115">Describes the status of a [ResolveNames operation](resolvenames-operation.md) response.</span></span> <br/><br/><span data-ttu-id="0bb85-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="0bb85-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="0bb85-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="0bb85-117">-  Success</span></span>  <br/><span data-ttu-id="0bb85-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="0bb85-118">-  Warning</span></span>  <br/><span data-ttu-id="0bb85-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="0bb85-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="0bb85-120">Atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0bb85-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="0bb85-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="0bb85-121">**Value**</span></span>|<span data-ttu-id="0bb85-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0bb85-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0bb85-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="0bb85-123">**Success**</span></span> <br/> |<span data-ttu-id="0bb85-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="0bb85-124">Describes a request that is fulfilled.</span></span> <span data-ttu-id="0bb85-125">Esse problema ocorre quando o nome solicitado é inequívoco e a resposta conterá um único destinatário.</span><span class="sxs-lookup"><span data-stu-id="0bb85-125">This occurs when the requested name is unambiguous and the response contains a single recipient.</span></span>  <br/> |
|<span data-ttu-id="0bb85-126">**Warning**</span><span class="sxs-lookup"><span data-stu-id="0bb85-126">**Warning**</span></span> <br/> | <span data-ttu-id="0bb85-127">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="0bb85-127">Describes a request that was not processed.</span></span> <span data-ttu-id="0bb85-128">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="0bb85-128">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="0bb85-129">Exemplo das fontes de avisos veja a seguir:</span><span class="sxs-lookup"><span data-stu-id="0bb85-129">The following are example of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="0bb85-130">-O armazenamento do Exchange fica offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="0bb85-130">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="0bb85-131">-Active Directory Domain Services (AD DS) ficará offline.</span><span class="sxs-lookup"><span data-stu-id="0bb85-131">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="0bb85-132">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="0bb85-132">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="0bb85-133">-O banco de dados de caixa de correio (MDB) ficará offline.</span><span class="sxs-lookup"><span data-stu-id="0bb85-133">-  The mailbox database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="0bb85-134">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="0bb85-134">-  A password is expired.</span></span>  <br/><span data-ttu-id="0bb85-135">-Uma cota for excedida.</span><span class="sxs-lookup"><span data-stu-id="0bb85-135">-  A quota is exceeded.</span></span>  <br/><span data-ttu-id="0bb85-136">-O nome solicitado é ambíguo e a resposta conterá vários destinatários.</span><span class="sxs-lookup"><span data-stu-id="0bb85-136">-  The requested name is ambiguous and the response contains multiple recipients.</span></span>  <br/> |
|<span data-ttu-id="0bb85-137">**Erro**</span><span class="sxs-lookup"><span data-stu-id="0bb85-137">**Error**</span></span> <br/> | <span data-ttu-id="0bb85-138">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="0bb85-138">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="0bb85-139">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="0bb85-139">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="0bb85-140">-O nome solicitado não pôde ser resolvido.</span><span class="sxs-lookup"><span data-stu-id="0bb85-140">-  The requested name could not be resolved.</span></span>  <br/><span data-ttu-id="0bb85-141">-Atributos ou elementos são inválidos.</span><span class="sxs-lookup"><span data-stu-id="0bb85-141">-  Attributes or elements are invalid.</span></span>  <br/><span data-ttu-id="0bb85-142">-Atributos ou elementos estão fora do intervalo.</span><span class="sxs-lookup"><span data-stu-id="0bb85-142">-  Attributes or elements are out of range.</span></span>  <br/><span data-ttu-id="0bb85-143">-Uma marca é desconhecida.</span><span class="sxs-lookup"><span data-stu-id="0bb85-143">-  A tag is unknown.</span></span>  <br/><span data-ttu-id="0bb85-144">-Um atributo ou elemento não é válido no contexto.</span><span class="sxs-lookup"><span data-stu-id="0bb85-144">-  An attribute or element is not valid in the context.</span></span>  <br/><span data-ttu-id="0bb85-145">-Uma tentativa de acesso não autorizado por qualquer cliente ocorreu.</span><span class="sxs-lookup"><span data-stu-id="0bb85-145">-  An unauthorized access attempt by any client occurred.</span></span>  <br/><span data-ttu-id="0bb85-146">-Falha do servidor em resposta a uma chamada de cliente válida.</span><span class="sxs-lookup"><span data-stu-id="0bb85-146">-  A server-side failure occurred in response to a valid client-side call.</span></span>  <br/>  <br/><span data-ttu-id="0bb85-147">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="0bb85-147">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0bb85-148">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0bb85-148">Child elements</span></span>

|<span data-ttu-id="0bb85-149">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0bb85-149">**Element**</span></span>|<span data-ttu-id="0bb85-150">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0bb85-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bb85-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="0bb85-151">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0bb85-152">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bb85-152">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0bb85-153">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0bb85-153">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0bb85-154">Fornece informações de erro sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bb85-154">Provides error information about the request.</span></span>  <br/> |
|[<span data-ttu-id="0bb85-155">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0bb85-155">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0bb85-156">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="0bb85-156">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="0bb85-157">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="0bb85-157">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="0bb85-158">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0bb85-158">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0bb85-159">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="0bb85-159">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0bb85-160">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="0bb85-160">ResolutionSet</span></span>](resolutionset.md) <br/> |<span data-ttu-id="0bb85-161">Contém uma matriz de resoluções referentes a um nome ambíguo.</span><span class="sxs-lookup"><span data-stu-id="0bb85-161">Contains an array of resolutions for an ambiguous name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0bb85-162">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0bb85-162">Parent elements</span></span>

|<span data-ttu-id="0bb85-163">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0bb85-163">**Element**</span></span>|<span data-ttu-id="0bb85-164">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0bb85-164">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bb85-165">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0bb85-165">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0bb85-166">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bb85-166">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0bb85-167">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="0bb85-167">Remarks</span></span>

<span data-ttu-id="0bb85-168">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="0bb85-168">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0bb85-169">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0bb85-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0bb85-170">Namespace</span><span class="sxs-lookup"><span data-stu-id="0bb85-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0bb85-171">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0bb85-171">Schema name</span></span>  <br/> |<span data-ttu-id="0bb85-172">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0bb85-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0bb85-173">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0bb85-173">Validation file</span></span>  <br/> |<span data-ttu-id="0bb85-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0bb85-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0bb85-175">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0bb85-175">Can be empty</span></span>  <br/> |<span data-ttu-id="0bb85-176">False</span><span class="sxs-lookup"><span data-stu-id="0bb85-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0bb85-177">Ver também</span><span class="sxs-lookup"><span data-stu-id="0bb85-177">See also</span></span>

- [<span data-ttu-id="0bb85-178">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="0bb85-178">ResolveNames</span></span>](resolvenames.md)
- [<span data-ttu-id="0bb85-179">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="0bb85-179">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
- [<span data-ttu-id="0bb85-180">Operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="0bb85-180">ResolveNames operation</span></span>](resolvenames-operation.md)

