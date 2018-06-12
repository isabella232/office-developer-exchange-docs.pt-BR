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
description: O elemento FindFolderResponseMessage contém o status e o resultado de uma única solicitação de operação FindFolder.
ms.openlocfilehash: 5623e5e538e617e5bd4bbc4444328ac83d7b8065
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752277"
---
# <a name="findfolderresponsemessage"></a><span data-ttu-id="30234-103">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="30234-103">FindFolderResponseMessage</span></span>

<span data-ttu-id="30234-104">O elemento **FindFolderResponseMessage** contém o status e o resultado de uma única [operação FindFolder](findfolder-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="30234-104">The **FindFolderResponseMessage** element contains the status and result of a single [FindFolder operation](findfolder-operation.md) request.</span></span> 
  
[<span data-ttu-id="30234-105">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="30234-105">FindFolderResponse</span></span>](findfolderresponse.md)
  
[<span data-ttu-id="30234-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="30234-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="30234-107">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="30234-107">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md)
  
```xml
<FindFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindFolderResponseMessage>
```

 <span data-ttu-id="30234-108">**FindFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="30234-108">**FindFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30234-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="30234-109">Attributes and elements</span></span>

<span data-ttu-id="30234-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="30234-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30234-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="30234-111">Attributes</span></span>

|<span data-ttu-id="30234-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="30234-112">**Attribute**</span></span>|<span data-ttu-id="30234-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="30234-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="30234-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="30234-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="30234-115">Descreve o status de uma resposta [FindFolder operação](findfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="30234-115">Describes the status of a [FindFolder operation](findfolder-operation.md) response.</span></span><br/><br/> <span data-ttu-id="30234-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="30234-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="30234-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="30234-117">-  Success</span></span>  <br/><span data-ttu-id="30234-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="30234-118">-  Warning</span></span>  <br/><span data-ttu-id="30234-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="30234-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="30234-120">Atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="30234-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="30234-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="30234-121">**Value**</span></span>|<span data-ttu-id="30234-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="30234-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="30234-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="30234-123">**Success**</span></span> <br/> |<span data-ttu-id="30234-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="30234-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="30234-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="30234-125">**Warning**</span></span> <br/> | <span data-ttu-id="30234-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="30234-126">Describes a request that was not processed.</span></span> <span data-ttu-id="30234-127">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="30234-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="30234-128">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="30234-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="30234-129">-O armazenamento do Exchange fica offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="30234-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="30234-130">-Active Directory Domain Services (AD DS) ficará offline.</span><span class="sxs-lookup"><span data-stu-id="30234-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="30234-131">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="30234-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="30234-132">-O banco de dados de mensagens (MDB) ficará offline.</span><span class="sxs-lookup"><span data-stu-id="30234-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="30234-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="30234-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="30234-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="30234-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="30234-135">**Erro**</span><span class="sxs-lookup"><span data-stu-id="30234-135">**Error**</span></span> <br/> | <span data-ttu-id="30234-136">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="30234-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="30234-137">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="30234-137">The following are examples of sources of errors:</span></span>  <br/><span data-ttu-id="30234-138">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="30234-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="30234-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="30234-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="30234-140">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="30234-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="30234-141">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="30234-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="30234-142">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="30234-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="30234-143">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="30234-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="30234-144">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="30234-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="30234-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="30234-145">Child elements</span></span>

|<span data-ttu-id="30234-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="30234-146">**Element**</span></span>|<span data-ttu-id="30234-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="30234-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30234-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="30234-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="30234-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="30234-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="30234-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="30234-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="30234-151">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="30234-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="30234-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="30234-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="30234-153">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="30234-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="30234-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="30234-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="30234-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="30234-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="30234-156">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="30234-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="30234-157">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="30234-157">RootFolder (FindFolderResponseMessage)</span></span>](rootfolder-findfolderresponsemessage.md) <br/> |<span data-ttu-id="30234-158">Contém os resultados de uma pesquisa de uma pasta raiz única durante uma [operação FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="30234-158">Contains the results from a search of a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="30234-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="30234-159">Parent elements</span></span>

|<span data-ttu-id="30234-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="30234-160">**Element**</span></span>|<span data-ttu-id="30234-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="30234-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30234-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="30234-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="30234-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="30234-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="30234-164">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="30234-164">Remarks</span></span>

<span data-ttu-id="30234-165">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="30234-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30234-166">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="30234-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30234-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="30234-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="30234-168">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="30234-168">Schema name</span></span>  <br/> |<span data-ttu-id="30234-169">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="30234-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="30234-170">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="30234-170">Validation file</span></span>  <br/> |<span data-ttu-id="30234-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="30234-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="30234-172">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="30234-172">Can be empty</span></span>  <br/> |<span data-ttu-id="30234-173">False</span><span class="sxs-lookup"><span data-stu-id="30234-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="30234-174">Ver também</span><span class="sxs-lookup"><span data-stu-id="30234-174">See also</span></span>

- [<span data-ttu-id="30234-175">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="30234-175">FindFolder operation</span></span>](findfolder-operation.md)
- [<span data-ttu-id="30234-176">Localizando pastas</span><span class="sxs-lookup"><span data-stu-id="30234-176">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

