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
description: O elemento DeleteItemResponseMessage contém o status e o resultado de uma única solicitação de operação de DeleteItem.
ms.openlocfilehash: 78e3efc6a9e9e6629d7efe7f2dc294e0a731005a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526925"
---
# <a name="deleteitemresponsemessage"></a><span data-ttu-id="dbfa3-103">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dbfa3-103">DeleteItemResponseMessage</span></span>

<span data-ttu-id="dbfa3-104">O elemento **DeleteItemResponseMessage** contém o status e o resultado de uma única solicitação de [operação de DeleteItem](deleteitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dbfa3-104">The **DeleteItemResponseMessage** element contains the status and result of a single [DeleteItem operation](deleteitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="dbfa3-105">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="dbfa3-105">DeleteItemResponse</span></span>](deleteitemresponse.md) 
- [<span data-ttu-id="dbfa3-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dbfa3-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="dbfa3-107">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dbfa3-107">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
  
```xml
<DeleteItemResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteItemResponseMessage>
```

 <span data-ttu-id="dbfa3-108">**DeleteItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="dbfa3-108">**DeleteItemResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dbfa3-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="dbfa3-109">Attributes and elements</span></span>

<span data-ttu-id="dbfa3-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dbfa3-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="dbfa3-111">Attributes</span></span>

|<span data-ttu-id="dbfa3-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="dbfa3-112">**Attribute**</span></span>|<span data-ttu-id="dbfa3-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dbfa3-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dbfa3-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="dbfa3-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="dbfa3-115">Descreve o status de uma resposta de [operação do DeleteItem](deleteitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dbfa3-115">Describes the status of a [DeleteItem operation](deleteitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="dbfa3-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="dbfa3-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="dbfa3-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="dbfa3-117">- Success</span></span>  <br/><span data-ttu-id="dbfa3-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="dbfa3-118">-  Warning</span></span>  <br/><span data-ttu-id="dbfa3-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="dbfa3-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="dbfa3-120">Atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="dbfa3-120">ResponseClass attribute</span></span>

|<span data-ttu-id="dbfa3-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="dbfa3-121">**Value**</span></span>|<span data-ttu-id="dbfa3-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dbfa3-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dbfa3-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="dbfa3-123">**Success**</span></span> <br/> |<span data-ttu-id="dbfa3-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="dbfa3-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="dbfa3-125">**Warning**</span></span> <br/> | <span data-ttu-id="dbfa3-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-126">Describes a request that was not processed.</span></span> <span data-ttu-id="dbfa3-127">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="dbfa3-128">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="dbfa3-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="dbfa3-129">– O repositório do Exchange fica offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="dbfa3-130">– O AD DS (serviços de domínio Active Directory) fica offline.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="dbfa3-131">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="dbfa3-132">– O banco de dados de mensagens (MDB) fica offline.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="dbfa3-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="dbfa3-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="dbfa3-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="dbfa3-135">**Error**</span></span> <br/> | <span data-ttu-id="dbfa3-136">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="dbfa3-137">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="dbfa3-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="dbfa3-138">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="dbfa3-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="dbfa3-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="dbfa3-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="dbfa3-140">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="dbfa3-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="dbfa3-141">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="dbfa3-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="dbfa3-142">– Um cliente tenta definir o nível de log de erros acima do nível máximo permitido pelo administrador</span><span class="sxs-lookup"><span data-stu-id="dbfa3-142">-  A client attempt to set the error logging level above the maximum level that is permitted by the administrator</span></span>  <br/><span data-ttu-id="dbfa3-143">– Um cliente tenta definir o nível de falha de gravidade abaixo do nível padrão especificado pelo administrador</span><span class="sxs-lookup"><span data-stu-id="dbfa3-143">-  A client attempt to set the severity failure level below the default level that is specified by the administrator</span></span>  <br/><span data-ttu-id="dbfa3-144">– Tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="dbfa3-144">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="dbfa3-145">-Falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="dbfa3-145">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="dbfa3-146">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="dbfa3-146">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="dbfa3-147">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dbfa3-147">Child elements</span></span>

|<span data-ttu-id="dbfa3-148">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dbfa3-148">**Element**</span></span>|<span data-ttu-id="dbfa3-149">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dbfa3-149">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbfa3-150">MessageText</span><span class="sxs-lookup"><span data-stu-id="dbfa3-150">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="dbfa3-151">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-151">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="dbfa3-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="dbfa3-152">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="dbfa3-153">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-153">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="dbfa3-154">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="dbfa3-154">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="dbfa3-155">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-155">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="dbfa3-156">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-156">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="dbfa3-157">MessageXml</span><span class="sxs-lookup"><span data-stu-id="dbfa3-157">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="dbfa3-158">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-158">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dbfa3-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dbfa3-159">Parent elements</span></span>

|<span data-ttu-id="dbfa3-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dbfa3-160">**Element**</span></span>|<span data-ttu-id="dbfa3-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dbfa3-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbfa3-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dbfa3-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="dbfa3-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dbfa3-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="dbfa3-164">Remarks</span></span>

<span data-ttu-id="dbfa3-165">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="dbfa3-166">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="dbfa3-166">Version differences</span></span>

<span data-ttu-id="dbfa3-167">Nas versões do Exchange que começam com a compilação 15.00.0986.00, o elemento **DeleteItemResponseMessage** é do tipo **DeleteItemResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-167">In versions of Exchange starting with build 15.00.0986.00, the **DeleteItemResponseMessage** element is of type **DeleteItemResponseMessageType**.</span></span> <span data-ttu-id="dbfa3-168">Nas versões anteriores, o elemento é do tipo **ResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-168">In previous versions, the element is of type **ResponseMessageType**.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dbfa3-169">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="dbfa3-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dbfa3-170">Namespace</span><span class="sxs-lookup"><span data-stu-id="dbfa3-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dbfa3-171">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dbfa3-171">Schema Name</span></span>  <br/> |<span data-ttu-id="dbfa3-172">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="dbfa3-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dbfa3-173">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dbfa3-173">Validation File</span></span>  <br/> |<span data-ttu-id="dbfa3-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dbfa3-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dbfa3-175">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="dbfa3-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="dbfa3-176">False</span><span class="sxs-lookup"><span data-stu-id="dbfa3-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dbfa3-177">Confira também</span><span class="sxs-lookup"><span data-stu-id="dbfa3-177">See also</span></span>

- [<span data-ttu-id="dbfa3-178">Operação DeleteItem</span><span class="sxs-lookup"><span data-stu-id="dbfa3-178">DeleteItem operation</span></span>](deleteitem-operation.md)
- [<span data-ttu-id="dbfa3-179">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="dbfa3-179">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="dbfa3-180">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="dbfa3-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="dbfa3-181">Excluindo itens (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="dbfa3-181">Deleting Items (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/9bfc39e6-d944-4eb6-8aee-cbaf1e37c67d%28Office.15%29.aspx)

