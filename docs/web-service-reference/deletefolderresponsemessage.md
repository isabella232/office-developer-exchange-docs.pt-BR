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
description: O elemento DeleteFolderResponseMessage contém o status e o resultado de uma única solicitação de operação de DeleteFolder.
ms.openlocfilehash: 6c593e0d6e8820452bb27a6baa569980e329ef10
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455734"
---
# <a name="deletefolderresponsemessage"></a><span data-ttu-id="62ae0-103">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="62ae0-103">DeleteFolderResponseMessage</span></span>

<span data-ttu-id="62ae0-104">O elemento **DeleteFolderResponseMessage** contém o status e o resultado de uma única solicitação de [operação de DeleteFolder](deletefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="62ae0-104">The **DeleteFolderResponseMessage** element contains the status and result of a single [DeleteFolder operation](deletefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="62ae0-105">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="62ae0-105">DeleteFolderResponse</span></span>](deletefolderresponse.md)  
- [<span data-ttu-id="62ae0-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="62ae0-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="62ae0-107">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="62ae0-107">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
  
```xml
<DeleteFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteFolderResponseMessage>
```

 <span data-ttu-id="62ae0-108">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="62ae0-108">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="62ae0-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="62ae0-109">Attributes and elements</span></span>

<span data-ttu-id="62ae0-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="62ae0-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="62ae0-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="62ae0-111">Attributes</span></span>

|<span data-ttu-id="62ae0-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="62ae0-112">**Attribute**</span></span>|<span data-ttu-id="62ae0-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="62ae0-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="62ae0-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="62ae0-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="62ae0-115">Descreve o status de uma resposta de [operação do DeleteFolder](deletefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="62ae0-115">Describes the status of a [DeleteFolder operation](deletefolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="62ae0-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="62ae0-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="62ae0-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="62ae0-117">-  Success</span></span>  <br/><span data-ttu-id="62ae0-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="62ae0-118">-  Warning</span></span>  <br/><span data-ttu-id="62ae0-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="62ae0-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="62ae0-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="62ae0-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="62ae0-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="62ae0-121">**Value**</span></span>|<span data-ttu-id="62ae0-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="62ae0-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="62ae0-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="62ae0-123">**Success**</span></span> <br/> |<span data-ttu-id="62ae0-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="62ae0-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="62ae0-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="62ae0-125">**Warning**</span></span> <br/> | <span data-ttu-id="62ae0-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="62ae0-126">Describes a request that was not processed.</span></span> <span data-ttu-id="62ae0-127">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="62ae0-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="62ae0-128">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="62ae0-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="62ae0-129">– O repositório do Exchange fica offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="62ae0-129">- The Exchange store goes offline during the batch.</span></span><br/><span data-ttu-id="62ae0-130">– O AD DS (serviços de domínio Active Directory) fica offline.</span><span class="sxs-lookup"><span data-stu-id="62ae0-130">- Active Directory Domain Services (AD DS) goes offline.</span></span><br/><span data-ttu-id="62ae0-131">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="62ae0-131">- Mailboxes are moved.</span></span><br/><span data-ttu-id="62ae0-132">– O banco de dados de mensagens (MDB) fica offline.</span><span class="sxs-lookup"><span data-stu-id="62ae0-132">- The message database (MDB) goes offline.</span></span><br/><span data-ttu-id="62ae0-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="62ae0-133">- A password is expired.</span></span><br/><span data-ttu-id="62ae0-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="62ae0-134">- A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="62ae0-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="62ae0-135">**Error**</span></span> <br/> | <span data-ttu-id="62ae0-136">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="62ae0-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="62ae0-137">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="62ae0-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="62ae0-138">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="62ae0-138">- Invalid attributes or elements</span></span><br/><span data-ttu-id="62ae0-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="62ae0-139">- Attributes or elements out of range</span></span><br/><span data-ttu-id="62ae0-140">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="62ae0-140">- Unknown tag</span></span><br/><span data-ttu-id="62ae0-141">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="62ae0-141">- Attribute or element not valid in the context</span></span><br/><span data-ttu-id="62ae0-142">– Tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="62ae0-142">- Unauthorized access attempt by any client</span></span><br/><span data-ttu-id="62ae0-143">-Falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="62ae0-143">- Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="62ae0-144">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="62ae0-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="62ae0-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="62ae0-145">Child elements</span></span>

|<span data-ttu-id="62ae0-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="62ae0-146">**Element**</span></span>|<span data-ttu-id="62ae0-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="62ae0-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62ae0-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="62ae0-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="62ae0-149">Uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="62ae0-149">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="62ae0-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="62ae0-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="62ae0-151">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="62ae0-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="62ae0-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="62ae0-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="62ae0-153">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="62ae0-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="62ae0-154">Ele contém o valor de 0.</span><span class="sxs-lookup"><span data-stu-id="62ae0-154">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="62ae0-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="62ae0-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="62ae0-156">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="62ae0-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="62ae0-157">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="62ae0-157">Parent elements</span></span>

|<span data-ttu-id="62ae0-158">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="62ae0-158">**Element**</span></span>|<span data-ttu-id="62ae0-159">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="62ae0-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62ae0-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="62ae0-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="62ae0-161">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="62ae0-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="62ae0-162">Comentários</span><span class="sxs-lookup"><span data-stu-id="62ae0-162">Remarks</span></span>

<span data-ttu-id="62ae0-163">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="62ae0-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="62ae0-164">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="62ae0-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="62ae0-165">Namespace</span><span class="sxs-lookup"><span data-stu-id="62ae0-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="62ae0-166">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="62ae0-166">Schema Name</span></span>  <br/> |<span data-ttu-id="62ae0-167">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="62ae0-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="62ae0-168">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="62ae0-168">Validation File</span></span>  <br/> |<span data-ttu-id="62ae0-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="62ae0-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="62ae0-170">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="62ae0-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="62ae0-171">False</span><span class="sxs-lookup"><span data-stu-id="62ae0-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="62ae0-172">Confira também</span><span class="sxs-lookup"><span data-stu-id="62ae0-172">See also</span></span>

- [<span data-ttu-id="62ae0-173">Operação DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="62ae0-173">DeleteFolder operation</span></span>](deletefolder-operation.md)
- [<span data-ttu-id="62ae0-174">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="62ae0-174">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="62ae0-175">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="62ae0-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="62ae0-176">Excluindo pastas</span><span class="sxs-lookup"><span data-stu-id="62ae0-176">Deleting Folders</span></span>](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

