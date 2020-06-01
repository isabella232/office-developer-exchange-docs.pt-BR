---
title: CopyFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolderResponseMessage
api_type:
- schema
ms.assetid: c82092a9-50ff-4ae1-b819-ebabbf89262b
description: O elemento CopyFolderResponseMessage contém o status e o resultado de uma única solicitação de operação de CopyFolder.
ms.openlocfilehash: 796ec57116e4b4943ca370e45cf0abefe7782c08
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458506"
---
# <a name="copyfolderresponsemessage"></a><span data-ttu-id="f9e89-103">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f9e89-103">CopyFolderResponseMessage</span></span>

<span data-ttu-id="f9e89-104">O elemento **CopyFolderResponseMessage** contém o status e o resultado de uma única solicitação de [operação de CopyFolder](copyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f9e89-104">The **CopyFolderResponseMessage** element contains the status and result of a single [CopyFolder operation](copyfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="f9e89-105">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="f9e89-105">CopyFolderResponse</span></span>](copyfolderresponse.md) 
- [<span data-ttu-id="f9e89-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f9e89-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="f9e89-107">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f9e89-107">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
  
```xml
<CopyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CopyFolderResponseMessage>
```

 <span data-ttu-id="f9e89-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f9e89-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f9e89-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f9e89-109">Attributes and elements</span></span>

<span data-ttu-id="f9e89-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f9e89-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9e89-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="f9e89-111">Attributes</span></span>

|<span data-ttu-id="f9e89-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="f9e89-112">**Attribute**</span></span>|<span data-ttu-id="f9e89-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f9e89-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f9e89-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="f9e89-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f9e89-115">Descreve o status de uma resposta de [operação do CopyFolder](copyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f9e89-115">Describes the status of a [CopyFolder operation](copyfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="f9e89-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="f9e89-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="f9e89-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="f9e89-117">- Success</span></span>  <br/><span data-ttu-id="f9e89-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="f9e89-118">-  Warning</span></span>  <br/><span data-ttu-id="f9e89-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="f9e89-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f9e89-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="f9e89-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="f9e89-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="f9e89-121">**Value**</span></span>|<span data-ttu-id="f9e89-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f9e89-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f9e89-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="f9e89-123">**Success**</span></span> <br/> |<span data-ttu-id="f9e89-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="f9e89-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f9e89-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="f9e89-125">**Warning**</span></span> <br/> | <span data-ttu-id="f9e89-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="f9e89-126">Describes a request that was not processed.</span></span> <span data-ttu-id="f9e89-127">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="f9e89-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="f9e89-128">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="f9e89-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="f9e89-129">– O repositório do Exchange fica offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="f9e89-129">- The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="f9e89-130">– O AD DS (serviços de domínio Active Directory) fica offline.</span><span class="sxs-lookup"><span data-stu-id="f9e89-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="f9e89-131">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="f9e89-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="f9e89-132">– O banco de dados de mensagens (MDB) fica offline.</span><span class="sxs-lookup"><span data-stu-id="f9e89-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="f9e89-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="f9e89-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="f9e89-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="f9e89-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="f9e89-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="f9e89-135">**Error**</span></span> <br/> | <span data-ttu-id="f9e89-136">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="f9e89-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="f9e89-137">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="f9e89-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="f9e89-138">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="f9e89-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="f9e89-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="f9e89-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="f9e89-140">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="f9e89-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="f9e89-141">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="f9e89-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="f9e89-142">– Acesso não autorizado tentado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="f9e89-142">-  Unauthorized access attempted by any client</span></span>  <br/><span data-ttu-id="f9e89-143">-Falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="f9e89-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="f9e89-144">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="f9e89-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f9e89-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f9e89-145">Child elements</span></span>

|<span data-ttu-id="f9e89-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f9e89-146">**Element**</span></span>|<span data-ttu-id="f9e89-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f9e89-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9e89-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="f9e89-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f9e89-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9e89-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f9e89-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f9e89-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f9e89-151">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="f9e89-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f9e89-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f9e89-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f9e89-153">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="f9e89-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="f9e89-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="f9e89-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f9e89-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f9e89-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f9e89-156">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="f9e89-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f9e89-157">Pastas</span><span class="sxs-lookup"><span data-stu-id="f9e89-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f9e89-158">Contém uma matriz de pastas copiadas.</span><span class="sxs-lookup"><span data-stu-id="f9e89-158">Contains an array of copied folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f9e89-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f9e89-159">Parent elements</span></span>

|<span data-ttu-id="f9e89-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f9e89-160">**Element**</span></span>|<span data-ttu-id="f9e89-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f9e89-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9e89-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f9e89-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f9e89-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f9e89-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f9e89-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="f9e89-164">Remarks</span></span>

<span data-ttu-id="f9e89-165">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f9e89-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f9e89-166">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f9e89-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9e89-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="f9e89-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f9e89-168">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f9e89-168">Schema name</span></span>  <br/> |<span data-ttu-id="f9e89-169">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f9e89-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f9e89-170">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f9e89-170">Validation file</span></span>  <br/> |<span data-ttu-id="f9e89-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f9e89-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f9e89-172">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f9e89-172">Can be empty</span></span>  <br/> |<span data-ttu-id="f9e89-173">False</span><span class="sxs-lookup"><span data-stu-id="f9e89-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f9e89-174">Confira também</span><span class="sxs-lookup"><span data-stu-id="f9e89-174">See also</span></span>

- [<span data-ttu-id="f9e89-175">Operação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="f9e89-175">CopyFolder operation</span></span>](copyfolder-operation.md)
- [<span data-ttu-id="f9e89-176">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="f9e89-176">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="f9e89-177">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f9e89-177">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

