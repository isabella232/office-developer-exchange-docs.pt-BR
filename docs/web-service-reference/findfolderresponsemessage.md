---
title: FindFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolderResponseMessage
api_type:
- schema
ms.assetid: 538d64fe-51ae-41d2-bfab-91698678aa1b
description: O elemento FindFolderResponseMessage contém o status e o resultado de uma única solicitação de operação de FindFolder.
ms.openlocfilehash: 318a09e371043252d43a5197211e9623f34229fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462560"
---
# <a name="findfolderresponsemessage"></a><span data-ttu-id="6f17a-103">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6f17a-103">FindFolderResponseMessage</span></span>

<span data-ttu-id="6f17a-104">O elemento **FindFolderResponseMessage** contém o status e o resultado de uma única solicitação de [operação de FindFolder](findfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6f17a-104">The **FindFolderResponseMessage** element contains the status and result of a single [FindFolder operation](findfolder-operation.md) request.</span></span> 
  
[<span data-ttu-id="6f17a-105">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="6f17a-105">FindFolderResponse</span></span>](findfolderresponse.md)
  
[<span data-ttu-id="6f17a-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6f17a-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="6f17a-107">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6f17a-107">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md)
  
```xml
<FindFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindFolderResponseMessage>
```

 <span data-ttu-id="6f17a-108">**FindFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6f17a-108">**FindFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6f17a-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6f17a-109">Attributes and elements</span></span>

<span data-ttu-id="6f17a-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6f17a-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f17a-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="6f17a-111">Attributes</span></span>

|<span data-ttu-id="6f17a-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="6f17a-112">**Attribute**</span></span>|<span data-ttu-id="6f17a-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6f17a-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6f17a-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="6f17a-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="6f17a-115">Descreve o status de uma resposta de [operação do FindFolder](findfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6f17a-115">Describes the status of a [FindFolder operation](findfolder-operation.md) response.</span></span><br/><br/> <span data-ttu-id="6f17a-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="6f17a-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="6f17a-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="6f17a-117">-  Success</span></span>  <br/><span data-ttu-id="6f17a-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="6f17a-118">-  Warning</span></span>  <br/><span data-ttu-id="6f17a-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="6f17a-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="6f17a-120">Atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="6f17a-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="6f17a-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="6f17a-121">**Value**</span></span>|<span data-ttu-id="6f17a-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6f17a-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6f17a-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="6f17a-123">**Success**</span></span> <br/> |<span data-ttu-id="6f17a-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="6f17a-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="6f17a-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="6f17a-125">**Warning**</span></span> <br/> | <span data-ttu-id="6f17a-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="6f17a-126">Describes a request that was not processed.</span></span> <span data-ttu-id="6f17a-127">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="6f17a-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="6f17a-128">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="6f17a-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="6f17a-129">– O repositório do Exchange fica offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="6f17a-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="6f17a-130">– O AD DS (serviços de domínio Active Directory) fica offline.</span><span class="sxs-lookup"><span data-stu-id="6f17a-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="6f17a-131">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="6f17a-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="6f17a-132">– O banco de dados de mensagens (MDB) fica offline.</span><span class="sxs-lookup"><span data-stu-id="6f17a-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="6f17a-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="6f17a-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="6f17a-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="6f17a-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="6f17a-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="6f17a-135">**Error**</span></span> <br/> | <span data-ttu-id="6f17a-136">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="6f17a-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="6f17a-137">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="6f17a-137">The following are examples of sources of errors:</span></span>  <br/><span data-ttu-id="6f17a-138">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="6f17a-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="6f17a-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="6f17a-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="6f17a-140">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="6f17a-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="6f17a-141">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="6f17a-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="6f17a-142">– Tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="6f17a-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="6f17a-143">-Falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="6f17a-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="6f17a-144">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="6f17a-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6f17a-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6f17a-145">Child elements</span></span>

|<span data-ttu-id="6f17a-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6f17a-146">**Element**</span></span>|<span data-ttu-id="6f17a-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6f17a-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f17a-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="6f17a-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="6f17a-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f17a-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="6f17a-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6f17a-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="6f17a-151">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="6f17a-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="6f17a-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="6f17a-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="6f17a-153">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="6f17a-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="6f17a-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="6f17a-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="6f17a-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="6f17a-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="6f17a-156">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="6f17a-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="6f17a-157">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="6f17a-157">RootFolder (FindFolderResponseMessage)</span></span>](rootfolder-findfolderresponsemessage.md) <br/> |<span data-ttu-id="6f17a-158">Contém os resultados de uma pesquisa de uma única pasta raiz durante uma [operação FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6f17a-158">Contains the results from a search of a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6f17a-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6f17a-159">Parent elements</span></span>

|<span data-ttu-id="6f17a-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6f17a-160">**Element**</span></span>|<span data-ttu-id="6f17a-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6f17a-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f17a-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6f17a-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="6f17a-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6f17a-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6f17a-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="6f17a-164">Remarks</span></span>

<span data-ttu-id="6f17a-165">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="6f17a-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6f17a-166">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6f17a-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f17a-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="6f17a-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6f17a-168">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6f17a-168">Schema name</span></span>  <br/> |<span data-ttu-id="6f17a-169">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6f17a-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6f17a-170">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6f17a-170">Validation file</span></span>  <br/> |<span data-ttu-id="6f17a-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6f17a-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6f17a-172">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="6f17a-172">Can be empty</span></span>  <br/> |<span data-ttu-id="6f17a-173">False</span><span class="sxs-lookup"><span data-stu-id="6f17a-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6f17a-174">Confira também</span><span class="sxs-lookup"><span data-stu-id="6f17a-174">See also</span></span>

- [<span data-ttu-id="6f17a-175">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="6f17a-175">FindFolder operation</span></span>](findfolder-operation.md)
- [<span data-ttu-id="6f17a-176">Localizando pastas</span><span class="sxs-lookup"><span data-stu-id="6f17a-176">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

