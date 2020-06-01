---
title: CreateManagedFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolderResponseMessage
api_type:
- schema
ms.assetid: a72eefc3-ef0b-4b44-a74b-e6907b5b5f68
description: O elemento CreateManagedFolderResponseMessage contém o status e o resultado de uma única solicitação de operação de CreateManagedFolder.
ms.openlocfilehash: 03ebcaeb79b2fac20882d2cea3d1e24b42dd472f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467701"
---
# <a name="createmanagedfolderresponsemessage"></a><span data-ttu-id="375ae-103">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="375ae-103">CreateManagedFolderResponseMessage</span></span>

<span data-ttu-id="375ae-104">O elemento **CreateManagedFolderResponseMessage** contém o status e o resultado de uma única solicitação de [operação de CreateManagedFolder](createmanagedfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="375ae-104">The **CreateManagedFolderResponseMessage** element contains the status and result of a single [CreateManagedFolder operation](createmanagedfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="375ae-105">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="375ae-105">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)  
- [<span data-ttu-id="375ae-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="375ae-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="375ae-107">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="375ae-107">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
  
```xml
<CreateManagedFolderResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CreateManagedFolderResponseMessage>
```

<span data-ttu-id="375ae-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="375ae-108">**FolderInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="375ae-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="375ae-109">Attributes and elements</span></span>

<span data-ttu-id="375ae-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="375ae-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="375ae-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="375ae-111">Attributes</span></span>

|<span data-ttu-id="375ae-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="375ae-112">**Attribute**</span></span>|<span data-ttu-id="375ae-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="375ae-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="375ae-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="375ae-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="375ae-115">Descreve o status de uma resposta de [operação do CreateManagedFolder](createmanagedfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="375ae-115">Describes the status of a [CreateManagedFolder operation](createmanagedfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="375ae-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="375ae-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="375ae-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="375ae-117">-  Success</span></span>  <br/><span data-ttu-id="375ae-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="375ae-118">-  Warning</span></span>  <br/><span data-ttu-id="375ae-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="375ae-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="375ae-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="375ae-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="375ae-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="375ae-121">**Value**</span></span>|<span data-ttu-id="375ae-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="375ae-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="375ae-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="375ae-123">**Success**</span></span> <br/> |<span data-ttu-id="375ae-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="375ae-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="375ae-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="375ae-125">**Warning**</span></span> <br/> | <span data-ttu-id="375ae-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="375ae-126">Describes a request that was not processed.</span></span> <span data-ttu-id="375ae-127">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="375ae-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="375ae-128">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="375ae-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="375ae-129">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="375ae-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="375ae-130">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="375ae-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="375ae-131">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="375ae-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="375ae-132">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="375ae-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="375ae-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="375ae-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="375ae-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="375ae-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="375ae-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="375ae-135">**Error**</span></span> <br/> | <span data-ttu-id="375ae-136">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="375ae-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="375ae-137">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="375ae-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="375ae-138">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="375ae-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="375ae-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="375ae-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="375ae-140">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="375ae-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="375ae-141">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="375ae-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="375ae-142">– Tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="375ae-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="375ae-143">-Falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="375ae-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="375ae-144">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="375ae-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="375ae-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="375ae-145">Child elements</span></span>

|<span data-ttu-id="375ae-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="375ae-146">**Element**</span></span>|<span data-ttu-id="375ae-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="375ae-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="375ae-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="375ae-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="375ae-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="375ae-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="375ae-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="375ae-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="375ae-151">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="375ae-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="375ae-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="375ae-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="375ae-153">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="375ae-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="375ae-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="375ae-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="375ae-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="375ae-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="375ae-156">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="375ae-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="375ae-157">Pastas</span><span class="sxs-lookup"><span data-stu-id="375ae-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="375ae-158">Contém uma matriz de pastas gerenciadas criadas.</span><span class="sxs-lookup"><span data-stu-id="375ae-158">Contains an array of created managed folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="375ae-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="375ae-159">Parent elements</span></span>

|<span data-ttu-id="375ae-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="375ae-160">**Element**</span></span>|<span data-ttu-id="375ae-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="375ae-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="375ae-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="375ae-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="375ae-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="375ae-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="375ae-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="375ae-164">Remarks</span></span>

<span data-ttu-id="375ae-165">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="375ae-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="375ae-166">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="375ae-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="375ae-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="375ae-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="375ae-168">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="375ae-168">Schema Name</span></span>  <br/> |<span data-ttu-id="375ae-169">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="375ae-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="375ae-170">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="375ae-170">Validation File</span></span>  <br/> |<span data-ttu-id="375ae-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="375ae-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="375ae-172">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="375ae-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="375ae-173">False</span><span class="sxs-lookup"><span data-stu-id="375ae-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="375ae-174">Confira também</span><span class="sxs-lookup"><span data-stu-id="375ae-174">See also</span></span>

- [<span data-ttu-id="375ae-175">Operação CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="375ae-175">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)
- [<span data-ttu-id="375ae-176">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="375ae-176">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="375ae-177">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="375ae-177">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

