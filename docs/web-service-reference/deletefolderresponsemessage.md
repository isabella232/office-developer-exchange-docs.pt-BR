---
title: DeleteFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolderResponseMessage
api_type:
- schema
ms.assetid: de4c63ff-80b2-40c2-bc06-ef0c23beacd4
description: O elemento DeleteFolderResponseMessage contém o status e o resultado de uma única solicitação de operação DeleteFolder.
ms.openlocfilehash: 5601fe2e48ad002e0fab60d812e7d70c7398f3ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751748"
---
# <a name="deletefolderresponsemessage"></a><span data-ttu-id="d2151-103">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d2151-103">DeleteFolderResponseMessage</span></span>

<span data-ttu-id="d2151-104">O elemento **DeleteFolderResponseMessage** contém o status e o resultado de uma única [operação DeleteFolder](deletefolder-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2151-104">The **DeleteFolderResponseMessage** element contains the status and result of a single [DeleteFolder operation](deletefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="d2151-105">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="d2151-105">DeleteFolderResponse</span></span>](deletefolderresponse.md)  
- [<span data-ttu-id="d2151-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d2151-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="d2151-107">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d2151-107">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
  
```xml
<DeleteFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteFolderResponseMessage>
```

 <span data-ttu-id="d2151-108">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d2151-108">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2151-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d2151-109">Attributes and elements</span></span>

<span data-ttu-id="d2151-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d2151-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2151-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="d2151-111">Attributes</span></span>

|<span data-ttu-id="d2151-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="d2151-112">**Attribute**</span></span>|<span data-ttu-id="d2151-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d2151-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d2151-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d2151-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d2151-115">Descreve o status de uma resposta [DeleteFolder operação](deletefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d2151-115">Describes the status of a [DeleteFolder operation](deletefolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="d2151-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="d2151-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="d2151-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="d2151-117">-  Success</span></span>  <br/><span data-ttu-id="d2151-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="d2151-118">-  Warning</span></span>  <br/><span data-ttu-id="d2151-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="d2151-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d2151-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="d2151-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="d2151-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="d2151-121">**Value**</span></span>|<span data-ttu-id="d2151-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d2151-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d2151-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="d2151-123">**Success**</span></span> <br/> |<span data-ttu-id="d2151-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="d2151-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d2151-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="d2151-125">**Warning**</span></span> <br/> | <span data-ttu-id="d2151-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="d2151-126">Describes a request that was not processed.</span></span> <span data-ttu-id="d2151-127">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="d2151-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="d2151-128">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="d2151-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="d2151-129">-O armazenamento do Exchange fica offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="d2151-129">- The Exchange store goes offline during the batch.</span></span><br/><span data-ttu-id="d2151-130">-Active Directory Domain Services (AD DS) ficará offline.</span><span class="sxs-lookup"><span data-stu-id="d2151-130">- Active Directory Domain Services (AD DS) goes offline.</span></span><br/><span data-ttu-id="d2151-131">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="d2151-131">- Mailboxes are moved.</span></span><br/><span data-ttu-id="d2151-132">-O banco de dados de mensagens (MDB) ficará offline.</span><span class="sxs-lookup"><span data-stu-id="d2151-132">- The message database (MDB) goes offline.</span></span><br/><span data-ttu-id="d2151-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="d2151-133">- A password is expired.</span></span><br/><span data-ttu-id="d2151-134">-Uma cota for excedida.</span><span class="sxs-lookup"><span data-stu-id="d2151-134">- A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="d2151-135">**Erro**</span><span class="sxs-lookup"><span data-stu-id="d2151-135">**Error**</span></span> <br/> | <span data-ttu-id="d2151-136">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="d2151-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="d2151-137">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="d2151-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="d2151-138">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d2151-138">- Invalid attributes or elements</span></span><br/><span data-ttu-id="d2151-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="d2151-139">- Attributes or elements out of range</span></span><br/><span data-ttu-id="d2151-140">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="d2151-140">- Unknown tag</span></span><br/><span data-ttu-id="d2151-141">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="d2151-141">- Attribute or element not valid in the context</span></span><br/><span data-ttu-id="d2151-142">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="d2151-142">- Unauthorized access attempt by any client</span></span><br/><span data-ttu-id="d2151-143">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="d2151-143">- Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="d2151-144">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="d2151-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d2151-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d2151-145">Child elements</span></span>

|<span data-ttu-id="d2151-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d2151-146">**Element**</span></span>|<span data-ttu-id="d2151-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d2151-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2151-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="d2151-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d2151-149">Uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2151-149">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d2151-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d2151-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d2151-151">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2151-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d2151-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d2151-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d2151-153">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="d2151-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="d2151-154">Ele contém o valor de 0.</span><span class="sxs-lookup"><span data-stu-id="d2151-154">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d2151-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d2151-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d2151-156">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="d2151-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d2151-157">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d2151-157">Parent elements</span></span>

|<span data-ttu-id="d2151-158">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d2151-158">**Element**</span></span>|<span data-ttu-id="d2151-159">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d2151-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2151-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d2151-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d2151-161">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2151-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d2151-162">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="d2151-162">Remarks</span></span>

<span data-ttu-id="d2151-163">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d2151-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2151-164">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d2151-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2151-165">Namespace</span><span class="sxs-lookup"><span data-stu-id="d2151-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d2151-166">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d2151-166">Schema Name</span></span>  <br/> |<span data-ttu-id="d2151-167">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d2151-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d2151-168">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d2151-168">Validation File</span></span>  <br/> |<span data-ttu-id="d2151-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d2151-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d2151-170">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d2151-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="d2151-171">False</span><span class="sxs-lookup"><span data-stu-id="d2151-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2151-172">Ver também</span><span class="sxs-lookup"><span data-stu-id="d2151-172">See also</span></span>

- [<span data-ttu-id="d2151-173">Operação DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="d2151-173">DeleteFolder operation</span></span>](deletefolder-operation.md)
- [<span data-ttu-id="d2151-174">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="d2151-174">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="d2151-175">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d2151-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="d2151-176">Excluindo pastas</span><span class="sxs-lookup"><span data-stu-id="d2151-176">Deleting Folders</span></span>](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)
