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
ms.openlocfilehash: 12f32008dbbc603fca7adf26057f1f1904d3cfb2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455594"
---
# <a name="resolvenamesresponsemessage"></a><span data-ttu-id="e8aea-103">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e8aea-103">ResolveNamesResponseMessage</span></span>

<span data-ttu-id="e8aea-104">O elemento **ResolveNamesResponseMessage** contém o status e o resultado de uma solicitação de [operação ResolveNames](resolvenames-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e8aea-104">The **ResolveNamesResponseMessage** element contains the status and result of a [ResolveNames operation](resolvenames-operation.md) request.</span></span> 
  
- [<span data-ttu-id="e8aea-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="e8aea-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md) 
- [<span data-ttu-id="e8aea-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e8aea-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="e8aea-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e8aea-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
```xml
<ResolveNamesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResolutionSet/>
</ResolveNamesResponseMessage>
```

 <span data-ttu-id="e8aea-108">**ResolveNamesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e8aea-108">**ResolveNamesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8aea-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e8aea-109">Attributes and elements</span></span>

<span data-ttu-id="e8aea-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e8aea-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8aea-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="e8aea-111">Attributes</span></span>

|<span data-ttu-id="e8aea-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="e8aea-112">**Attribute**</span></span>|<span data-ttu-id="e8aea-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e8aea-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e8aea-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="e8aea-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="e8aea-115">Descreve o status de uma resposta de [operação ResolveNames](resolvenames-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e8aea-115">Describes the status of a [ResolveNames operation](resolvenames-operation.md) response.</span></span> <br/><br/><span data-ttu-id="e8aea-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="e8aea-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="e8aea-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="e8aea-117">-  Success</span></span>  <br/><span data-ttu-id="e8aea-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="e8aea-118">-  Warning</span></span>  <br/><span data-ttu-id="e8aea-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="e8aea-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="e8aea-120">Atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e8aea-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="e8aea-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e8aea-121">**Value**</span></span>|<span data-ttu-id="e8aea-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e8aea-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e8aea-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="e8aea-123">**Success**</span></span> <br/> |<span data-ttu-id="e8aea-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="e8aea-124">Describes a request that is fulfilled.</span></span> <span data-ttu-id="e8aea-125">Isso ocorre quando o nome solicitado é inambíguo e a resposta contém um único destinatário.</span><span class="sxs-lookup"><span data-stu-id="e8aea-125">This occurs when the requested name is unambiguous and the response contains a single recipient.</span></span>  <br/> |
|<span data-ttu-id="e8aea-126">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="e8aea-126">**Warning**</span></span> <br/> | <span data-ttu-id="e8aea-127">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="e8aea-127">Describes a request that was not processed.</span></span> <span data-ttu-id="e8aea-128">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="e8aea-128">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="e8aea-129">Veja a seguir um exemplo de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="e8aea-129">The following are example of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="e8aea-130">– O repositório do Exchange fica offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="e8aea-130">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="e8aea-131">– O AD DS (serviços de domínio Active Directory) fica offline.</span><span class="sxs-lookup"><span data-stu-id="e8aea-131">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="e8aea-132">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="e8aea-132">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="e8aea-133">– O banco de dados de caixa de correio (MDB) fica offline.</span><span class="sxs-lookup"><span data-stu-id="e8aea-133">-  The mailbox database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="e8aea-134">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="e8aea-134">-  A password is expired.</span></span>  <br/><span data-ttu-id="e8aea-135">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="e8aea-135">-  A quota is exceeded.</span></span>  <br/><span data-ttu-id="e8aea-136">-O nome solicitado é ambíguo e a resposta contém vários destinatários.</span><span class="sxs-lookup"><span data-stu-id="e8aea-136">-  The requested name is ambiguous and the response contains multiple recipients.</span></span>  <br/> |
|<span data-ttu-id="e8aea-137">**Error**</span><span class="sxs-lookup"><span data-stu-id="e8aea-137">**Error**</span></span> <br/> | <span data-ttu-id="e8aea-138">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="e8aea-138">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="e8aea-139">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="e8aea-139">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="e8aea-140">-O nome solicitado não pôde ser resolvido.</span><span class="sxs-lookup"><span data-stu-id="e8aea-140">-  The requested name could not be resolved.</span></span>  <br/><span data-ttu-id="e8aea-141">-Os atributos ou elementos são inválidos.</span><span class="sxs-lookup"><span data-stu-id="e8aea-141">-  Attributes or elements are invalid.</span></span>  <br/><span data-ttu-id="e8aea-142">-Os atributos ou elementos estão fora do intervalo.</span><span class="sxs-lookup"><span data-stu-id="e8aea-142">-  Attributes or elements are out of range.</span></span>  <br/><span data-ttu-id="e8aea-143">-Uma marca é desconhecida.</span><span class="sxs-lookup"><span data-stu-id="e8aea-143">-  A tag is unknown.</span></span>  <br/><span data-ttu-id="e8aea-144">-Um atributo ou elemento não é válido no contexto.</span><span class="sxs-lookup"><span data-stu-id="e8aea-144">-  An attribute or element is not valid in the context.</span></span>  <br/><span data-ttu-id="e8aea-145">-Uma tentativa de acesso não autorizado por qualquer cliente ocorreu.</span><span class="sxs-lookup"><span data-stu-id="e8aea-145">-  An unauthorized access attempt by any client occurred.</span></span>  <br/><span data-ttu-id="e8aea-146">-Uma falha do servidor ocorreu em resposta a uma chamada válida do lado do cliente.</span><span class="sxs-lookup"><span data-stu-id="e8aea-146">-  A server-side failure occurred in response to a valid client-side call.</span></span>  <br/>  <br/><span data-ttu-id="e8aea-147">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="e8aea-147">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e8aea-148">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e8aea-148">Child elements</span></span>

|<span data-ttu-id="e8aea-149">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e8aea-149">**Element**</span></span>|<span data-ttu-id="e8aea-150">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e8aea-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8aea-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="e8aea-151">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e8aea-152">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8aea-152">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e8aea-153">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e8aea-153">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e8aea-154">Fornece informações de erro sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8aea-154">Provides error information about the request.</span></span>  <br/> |
|[<span data-ttu-id="e8aea-155">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e8aea-155">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e8aea-156">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="e8aea-156">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="e8aea-157">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="e8aea-157">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="e8aea-158">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e8aea-158">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e8aea-159">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="e8aea-159">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e8aea-160">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="e8aea-160">ResolutionSet</span></span>](resolutionset.md) <br/> |<span data-ttu-id="e8aea-161">Contém uma matriz de resoluções para um nome ambíguo.</span><span class="sxs-lookup"><span data-stu-id="e8aea-161">Contains an array of resolutions for an ambiguous name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e8aea-162">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e8aea-162">Parent elements</span></span>

|<span data-ttu-id="e8aea-163">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e8aea-163">**Element**</span></span>|<span data-ttu-id="e8aea-164">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e8aea-164">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8aea-165">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e8aea-165">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e8aea-166">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8aea-166">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e8aea-167">Comentários</span><span class="sxs-lookup"><span data-stu-id="e8aea-167">Remarks</span></span>

<span data-ttu-id="e8aea-168">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="e8aea-168">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8aea-169">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e8aea-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8aea-170">Namespace</span><span class="sxs-lookup"><span data-stu-id="e8aea-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e8aea-171">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e8aea-171">Schema name</span></span>  <br/> |<span data-ttu-id="e8aea-172">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e8aea-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e8aea-173">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e8aea-173">Validation file</span></span>  <br/> |<span data-ttu-id="e8aea-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e8aea-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e8aea-175">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e8aea-175">Can be empty</span></span>  <br/> |<span data-ttu-id="e8aea-176">False</span><span class="sxs-lookup"><span data-stu-id="e8aea-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8aea-177">Confira também</span><span class="sxs-lookup"><span data-stu-id="e8aea-177">See also</span></span>

- [<span data-ttu-id="e8aea-178">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="e8aea-178">ResolveNames</span></span>](resolvenames.md)
- [<span data-ttu-id="e8aea-179">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="e8aea-179">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
- [<span data-ttu-id="e8aea-180">Operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="e8aea-180">ResolveNames operation</span></span>](resolvenames-operation.md)

