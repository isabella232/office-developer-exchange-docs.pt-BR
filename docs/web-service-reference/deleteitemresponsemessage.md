---
title: DeleteItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemResponseMessage
api_type:
- schema
ms.assetid: c3d34c4d-8d83-4612-aa9e-66f9cc7314df
description: O elemento DeleteItemResponseMessage contém o status e o resultado de uma única solicitação de operação DeleteItem.
ms.openlocfilehash: 1f0cc3d49bfa5fba6da32cf65df6b6718ccfbded
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751765"
---
# <a name="deleteitemresponsemessage"></a><span data-ttu-id="0d07b-103">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0d07b-103">DeleteItemResponseMessage</span></span>

<span data-ttu-id="0d07b-104">O elemento **DeleteItemResponseMessage** contém o status e o resultado de uma única [operação DeleteItem](deleteitem-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d07b-104">The **DeleteItemResponseMessage** element contains the status and result of a single [DeleteItem operation](deleteitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="0d07b-105">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="0d07b-105">DeleteItemResponse</span></span>](deleteitemresponse.md) 
- [<span data-ttu-id="0d07b-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0d07b-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="0d07b-107">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0d07b-107">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
  
```xml
<DeleteItemResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteItemResponseMessage>
```

 <span data-ttu-id="0d07b-108">**DeleteItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0d07b-108">**DeleteItemResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d07b-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0d07b-109">Attributes and elements</span></span>

<span data-ttu-id="0d07b-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0d07b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d07b-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="0d07b-111">Attributes</span></span>

|<span data-ttu-id="0d07b-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="0d07b-112">**Attribute**</span></span>|<span data-ttu-id="0d07b-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0d07b-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0d07b-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="0d07b-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="0d07b-115">Descreve o status de uma resposta de [operação DeleteItem](deleteitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0d07b-115">Describes the status of a [DeleteItem operation](deleteitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="0d07b-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="0d07b-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="0d07b-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="0d07b-117">- Success</span></span>  <br/><span data-ttu-id="0d07b-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="0d07b-118">-  Warning</span></span>  <br/><span data-ttu-id="0d07b-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="0d07b-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="0d07b-120">Atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0d07b-120">ResponseClass attribute</span></span>

|<span data-ttu-id="0d07b-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="0d07b-121">**Value**</span></span>|<span data-ttu-id="0d07b-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0d07b-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0d07b-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="0d07b-123">**Success**</span></span> <br/> |<span data-ttu-id="0d07b-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="0d07b-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="0d07b-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="0d07b-125">**Warning**</span></span> <br/> | <span data-ttu-id="0d07b-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="0d07b-126">Describes a request that was not processed.</span></span> <span data-ttu-id="0d07b-127">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="0d07b-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="0d07b-128">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="0d07b-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="0d07b-129">-O armazenamento do Exchange fica offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="0d07b-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="0d07b-130">-Active Directory Domain Services (AD DS) ficará offline.</span><span class="sxs-lookup"><span data-stu-id="0d07b-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="0d07b-131">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="0d07b-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="0d07b-132">-O banco de dados de mensagens (MDB) ficará offline.</span><span class="sxs-lookup"><span data-stu-id="0d07b-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="0d07b-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="0d07b-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="0d07b-134">-Uma cota for excedida.</span><span class="sxs-lookup"><span data-stu-id="0d07b-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="0d07b-135">**Erro**</span><span class="sxs-lookup"><span data-stu-id="0d07b-135">**Error**</span></span> <br/> | <span data-ttu-id="0d07b-136">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="0d07b-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="0d07b-137">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="0d07b-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="0d07b-138">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0d07b-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="0d07b-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="0d07b-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="0d07b-140">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="0d07b-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="0d07b-141">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="0d07b-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="0d07b-142">-Um cliente tentar definir o nível de log de erro acima do nível máximo permitido pelo administrador</span><span class="sxs-lookup"><span data-stu-id="0d07b-142">-  A client attempt to set the error logging level above the maximum level that is permitted by the administrator</span></span>  <br/><span data-ttu-id="0d07b-143">-Um cliente tentar definir o nível de severidade falha abaixo do nível de padrão que é especificado pelo administrador</span><span class="sxs-lookup"><span data-stu-id="0d07b-143">-  A client attempt to set the severity failure level below the default level that is specified by the administrator</span></span>  <br/><span data-ttu-id="0d07b-144">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="0d07b-144">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="0d07b-145">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="0d07b-145">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="0d07b-146">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="0d07b-146">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0d07b-147">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0d07b-147">Child elements</span></span>

|<span data-ttu-id="0d07b-148">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0d07b-148">**Element**</span></span>|<span data-ttu-id="0d07b-149">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0d07b-149">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d07b-150">MessageText</span><span class="sxs-lookup"><span data-stu-id="0d07b-150">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0d07b-151">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d07b-151">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0d07b-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0d07b-152">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0d07b-153">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d07b-153">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="0d07b-154">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0d07b-154">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0d07b-155">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="0d07b-155">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="0d07b-156">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="0d07b-156">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="0d07b-157">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0d07b-157">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0d07b-158">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="0d07b-158">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0d07b-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0d07b-159">Parent elements</span></span>

|<span data-ttu-id="0d07b-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0d07b-160">**Element**</span></span>|<span data-ttu-id="0d07b-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0d07b-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d07b-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0d07b-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0d07b-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d07b-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0d07b-164">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="0d07b-164">Remarks</span></span>

<span data-ttu-id="0d07b-165">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="0d07b-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="0d07b-166">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="0d07b-166">Version differences</span></span>

<span data-ttu-id="0d07b-167">Nas versões do Exchange, começando com compilação 15.00.0986.00, o elemento **DeleteItemResponseMessage** é do tipo **DeleteItemResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="0d07b-167">In versions of Exchange starting with build 15.00.0986.00, the **DeleteItemResponseMessage** element is of type **DeleteItemResponseMessageType**.</span></span> <span data-ttu-id="0d07b-168">Nas versões anteriores, o elemento é do tipo **ResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="0d07b-168">In previous versions, the element is of type **ResponseMessageType**.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d07b-169">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0d07b-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d07b-170">Namespace</span><span class="sxs-lookup"><span data-stu-id="0d07b-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0d07b-171">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0d07b-171">Schema Name</span></span>  <br/> |<span data-ttu-id="0d07b-172">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0d07b-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0d07b-173">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0d07b-173">Validation File</span></span>  <br/> |<span data-ttu-id="0d07b-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0d07b-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0d07b-175">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0d07b-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="0d07b-176">False</span><span class="sxs-lookup"><span data-stu-id="0d07b-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0d07b-177">Ver também</span><span class="sxs-lookup"><span data-stu-id="0d07b-177">See also</span></span>

- [<span data-ttu-id="0d07b-178">Operação DeleteItem</span><span class="sxs-lookup"><span data-stu-id="0d07b-178">DeleteItem operation</span></span>](deleteitem-operation.md)
- [<span data-ttu-id="0d07b-179">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="0d07b-179">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="0d07b-180">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0d07b-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="0d07b-181">Excluindo itens (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="0d07b-181">Deleting Items (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/9bfc39e6-d944-4eb6-8aee-cbaf1e37c67d%28Office.15%29.aspx)

