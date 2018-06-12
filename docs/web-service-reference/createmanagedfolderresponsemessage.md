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
description: O elemento CreateManagedFolderResponseMessage contém o status e o resultado de uma única solicitação de operação CreateManagedFolder.
ms.openlocfilehash: e561cac949ebebc647b16578c6acbcd6132eeef7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751624"
---
# <a name="createmanagedfolderresponsemessage"></a><span data-ttu-id="777c0-103">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="777c0-103">CreateManagedFolderResponseMessage</span></span>

<span data-ttu-id="777c0-104">O elemento **CreateManagedFolderResponseMessage** contém o status e o resultado de uma única [operação CreateManagedFolder](createmanagedfolder-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="777c0-104">The **CreateManagedFolderResponseMessage** element contains the status and result of a single [CreateManagedFolder operation](createmanagedfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="777c0-105">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="777c0-105">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)  
- [<span data-ttu-id="777c0-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="777c0-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="777c0-107">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="777c0-107">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
  
```xml
<CreateManagedFolderResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CreateManagedFolderResponseMessage>
```

<span data-ttu-id="777c0-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="777c0-108">**FolderInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="777c0-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="777c0-109">Attributes and elements</span></span>

<span data-ttu-id="777c0-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="777c0-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="777c0-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="777c0-111">Attributes</span></span>

|<span data-ttu-id="777c0-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="777c0-112">**Attribute**</span></span>|<span data-ttu-id="777c0-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="777c0-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="777c0-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="777c0-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="777c0-115">Descreve o status de uma resposta [CreateManagedFolder operação](createmanagedfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="777c0-115">Describes the status of a [CreateManagedFolder operation](createmanagedfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="777c0-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="777c0-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="777c0-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="777c0-117">-  Success</span></span>  <br/><span data-ttu-id="777c0-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="777c0-118">-  Warning</span></span>  <br/><span data-ttu-id="777c0-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="777c0-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="777c0-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="777c0-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="777c0-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="777c0-121">**Value**</span></span>|<span data-ttu-id="777c0-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="777c0-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="777c0-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="777c0-123">**Success**</span></span> <br/> |<span data-ttu-id="777c0-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="777c0-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="777c0-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="777c0-125">**Warning**</span></span> <br/> | <span data-ttu-id="777c0-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="777c0-126">Describes a request that was not processed.</span></span> <span data-ttu-id="777c0-127">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="777c0-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="777c0-128">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="777c0-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="777c0-129">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="777c0-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="777c0-130">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="777c0-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="777c0-131">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="777c0-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="777c0-132">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="777c0-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="777c0-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="777c0-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="777c0-134">-Uma cota for excedida.</span><span class="sxs-lookup"><span data-stu-id="777c0-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="777c0-135">**Erro**</span><span class="sxs-lookup"><span data-stu-id="777c0-135">**Error**</span></span> <br/> | <span data-ttu-id="777c0-136">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="777c0-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="777c0-137">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="777c0-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="777c0-138">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="777c0-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="777c0-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="777c0-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="777c0-140">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="777c0-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="777c0-141">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="777c0-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="777c0-142">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="777c0-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="777c0-143">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="777c0-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="777c0-144">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="777c0-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="777c0-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="777c0-145">Child elements</span></span>

|<span data-ttu-id="777c0-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="777c0-146">**Element**</span></span>|<span data-ttu-id="777c0-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="777c0-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="777c0-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="777c0-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="777c0-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="777c0-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="777c0-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="777c0-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="777c0-151">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="777c0-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="777c0-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="777c0-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="777c0-153">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="777c0-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="777c0-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="777c0-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="777c0-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="777c0-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="777c0-156">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="777c0-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="777c0-157">Pastas</span><span class="sxs-lookup"><span data-stu-id="777c0-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="777c0-158">Contém uma matriz de pastas gerenciadas criadas.</span><span class="sxs-lookup"><span data-stu-id="777c0-158">Contains an array of created managed folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="777c0-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="777c0-159">Parent elements</span></span>

|<span data-ttu-id="777c0-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="777c0-160">**Element**</span></span>|<span data-ttu-id="777c0-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="777c0-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="777c0-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="777c0-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="777c0-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="777c0-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="777c0-164">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="777c0-164">Remarks</span></span>

<span data-ttu-id="777c0-165">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="777c0-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="777c0-166">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="777c0-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="777c0-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="777c0-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="777c0-168">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="777c0-168">Schema Name</span></span>  <br/> |<span data-ttu-id="777c0-169">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="777c0-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="777c0-170">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="777c0-170">Validation File</span></span>  <br/> |<span data-ttu-id="777c0-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="777c0-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="777c0-172">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="777c0-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="777c0-173">False</span><span class="sxs-lookup"><span data-stu-id="777c0-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="777c0-174">Ver também</span><span class="sxs-lookup"><span data-stu-id="777c0-174">See also</span></span>

- [<span data-ttu-id="777c0-175">Operação CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="777c0-175">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)
- [<span data-ttu-id="777c0-176">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="777c0-176">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="777c0-177">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="777c0-177">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

