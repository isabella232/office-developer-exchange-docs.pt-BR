---
title: CreateFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolderResponseMessage
api_type:
- schema
ms.assetid: 1301dd15-b008-4fd9-8c89-b15a20b186e2
description: O elemento CreateFolderResponseMessage contém o status e o resultado de uma única solicitação de operação CreateFolder.
ms.openlocfilehash: 386dd2aa4e114d8382d5c83a3d6da70b1ccbbada
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457526"
---
# <a name="createfolderresponsemessage"></a><span data-ttu-id="dc76a-103">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dc76a-103">CreateFolderResponseMessage</span></span>

<span data-ttu-id="dc76a-104">O elemento **CreateFolderResponseMessage** contém o status e o resultado de uma única solicitação de [operação CreateFolder](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dc76a-104">The **CreateFolderResponseMessage** element contains the status and result of a single [CreateFolder operation](createfolder-operation.md) request.</span></span> 
  
```xml
<CreateFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CreateFolderResponseMessage>
```

<span data-ttu-id="dc76a-105">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="dc76a-105">**FolderInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="dc76a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="dc76a-106">Attributes and elements</span></span>

<span data-ttu-id="dc76a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dc76a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc76a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="dc76a-108">Attributes</span></span>

|<span data-ttu-id="dc76a-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="dc76a-109">**Attribute**</span></span>|<span data-ttu-id="dc76a-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dc76a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dc76a-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="dc76a-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="dc76a-112">Descreve o status de uma resposta de [operação CreateFolder](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dc76a-112">Describes the status of a [CreateFolder operation](createfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="dc76a-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="dc76a-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="dc76a-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="dc76a-114">-  Success</span></span>  <br/><span data-ttu-id="dc76a-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="dc76a-115">-  Warning</span></span>  <br/><span data-ttu-id="dc76a-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="dc76a-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="dc76a-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="dc76a-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="dc76a-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="dc76a-118">**Value**</span></span>|<span data-ttu-id="dc76a-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dc76a-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dc76a-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="dc76a-120">**Success**</span></span> <br/> |<span data-ttu-id="dc76a-121">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="dc76a-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="dc76a-122">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="dc76a-122">**Warning**</span></span> <br/> | <span data-ttu-id="dc76a-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="dc76a-123">Describes a request that was not processed.</span></span> <span data-ttu-id="dc76a-124">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="dc76a-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="dc76a-125">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="dc76a-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="dc76a-126">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="dc76a-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="dc76a-127">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="dc76a-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="dc76a-128">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="dc76a-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="dc76a-129">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="dc76a-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="dc76a-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="dc76a-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="dc76a-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="dc76a-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="dc76a-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="dc76a-132">**Error**</span></span> <br/> | <span data-ttu-id="dc76a-133">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="dc76a-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="dc76a-134">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="dc76a-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="dc76a-135">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="dc76a-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="dc76a-136">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="dc76a-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="dc76a-137">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="dc76a-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="dc76a-138">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="dc76a-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="dc76a-139">– Tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="dc76a-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="dc76a-140">-Falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="dc76a-140">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="dc76a-141">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="dc76a-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="dc76a-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dc76a-142">Child elements</span></span>

|<span data-ttu-id="dc76a-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dc76a-143">**Element**</span></span>|<span data-ttu-id="dc76a-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dc76a-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc76a-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="dc76a-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="dc76a-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc76a-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="dc76a-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="dc76a-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="dc76a-148">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="dc76a-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="dc76a-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="dc76a-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="dc76a-150">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="dc76a-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="dc76a-151">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="dc76a-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="dc76a-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="dc76a-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="dc76a-153">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="dc76a-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="dc76a-154">Pastas</span><span class="sxs-lookup"><span data-stu-id="dc76a-154">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="dc76a-155">Contém uma matriz de pastas criadas.</span><span class="sxs-lookup"><span data-stu-id="dc76a-155">Contains an array of created folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dc76a-156">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dc76a-156">Parent elements</span></span>

|<span data-ttu-id="dc76a-157">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dc76a-157">**Element**</span></span>|<span data-ttu-id="dc76a-158">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dc76a-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc76a-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dc76a-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="dc76a-160">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="dc76a-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dc76a-161">Comentários</span><span class="sxs-lookup"><span data-stu-id="dc76a-161">Remarks</span></span>

<span data-ttu-id="dc76a-162">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange Server com a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="dc76a-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc76a-163">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="dc76a-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc76a-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="dc76a-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dc76a-165">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dc76a-165">Schema Name</span></span>  <br/> |<span data-ttu-id="dc76a-166">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="dc76a-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dc76a-167">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dc76a-167">Validation File</span></span>  <br/> |<span data-ttu-id="dc76a-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dc76a-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dc76a-169">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="dc76a-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="dc76a-170">False</span><span class="sxs-lookup"><span data-stu-id="dc76a-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc76a-171">Confira também</span><span class="sxs-lookup"><span data-stu-id="dc76a-171">See also</span></span>

- [<span data-ttu-id="dc76a-172">Operação CreateFolder</span><span class="sxs-lookup"><span data-stu-id="dc76a-172">CreateFolder operation</span></span>](createfolder-operation.md)
- [<span data-ttu-id="dc76a-173">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="dc76a-173">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="dc76a-174">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="dc76a-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

