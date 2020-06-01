---
title: ExportItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExportItemsResponseMessage
api_type:
- schema
ms.assetid: 830fb008-3c45-4988-9041-91a3da3fe689
description: O elemento ExportItemsResponseMessage contém o status e os resultados de uma solicitação para exportar um único item de caixa de correio.
ms.openlocfilehash: 3265836ce6d9d6ef97a4e598bbb3f50e7c5047c6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468943"
---
# <a name="exportitemsresponsemessage"></a><span data-ttu-id="96b77-103">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="96b77-103">ExportItemsResponseMessage</span></span>

<span data-ttu-id="96b77-104">O elemento **ExportItemsResponseMessage** contém o status e os resultados de uma solicitação para exportar um único item de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="96b77-104">The **ExportItemsResponseMessage** element contains the status and results of a request to export a single mailbox item.</span></span> 
  
- [<span data-ttu-id="96b77-105">ExportItemsResponse</span><span class="sxs-lookup"><span data-stu-id="96b77-105">ExportItemsResponse</span></span>](exportitemsresponse.md)  
- [<span data-ttu-id="96b77-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="96b77-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="96b77-107">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="96b77-107">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md)
  
```XML
<ExportItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ItemId/>
   <Data/>
</ExportItemsResponseMessage>
```

<span data-ttu-id="96b77-108">**ExportItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="96b77-108">**ExportItemsResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="96b77-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="96b77-109">Attributes and elements</span></span>

<span data-ttu-id="96b77-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="96b77-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96b77-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="96b77-111">Attributes</span></span>

|<span data-ttu-id="96b77-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="96b77-112">**Attribute**</span></span>|<span data-ttu-id="96b77-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96b77-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="96b77-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="96b77-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="96b77-115">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="96b77-115">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="96b77-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="96b77-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="96b77-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="96b77-117">-  Success</span></span>  <br/><span data-ttu-id="96b77-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="96b77-118">-  Warning</span></span>  <br/><span data-ttu-id="96b77-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="96b77-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="96b77-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="96b77-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="96b77-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="96b77-121">**Value**</span></span>|<span data-ttu-id="96b77-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96b77-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="96b77-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="96b77-123">**Success**</span></span> <br/> |<span data-ttu-id="96b77-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="96b77-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="96b77-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="96b77-125">**Warning**</span></span> <br/> | <span data-ttu-id="96b77-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="96b77-126">Describes a request that was not processed.</span></span> <span data-ttu-id="96b77-127">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="96b77-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="96b77-128">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="96b77-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="96b77-129">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="96b77-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="96b77-130">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="96b77-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="96b77-131">-As caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="96b77-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="96b77-132">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="96b77-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="96b77-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="96b77-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="96b77-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="96b77-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="96b77-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="96b77-135">**Error**</span></span> <br/> | <span data-ttu-id="96b77-136">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="96b77-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="96b77-137">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="96b77-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="96b77-138">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="96b77-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="96b77-139">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="96b77-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="96b77-140">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="96b77-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="96b77-141">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="96b77-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="96b77-142">– Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="96b77-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="96b77-143">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="96b77-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="96b77-144">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="96b77-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="96b77-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="96b77-145">Child elements</span></span>

|<span data-ttu-id="96b77-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="96b77-146">**Element**</span></span>|<span data-ttu-id="96b77-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96b77-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96b77-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="96b77-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="96b77-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="96b77-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="96b77-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="96b77-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="96b77-151">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="96b77-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="96b77-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="96b77-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="96b77-153">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="96b77-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="96b77-154">Este elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="96b77-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="96b77-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="96b77-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="96b77-156">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="96b77-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="96b77-157">ItemId</span><span class="sxs-lookup"><span data-stu-id="96b77-157">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="96b77-158">Contém o identificador de item de um item exportado.</span><span class="sxs-lookup"><span data-stu-id="96b77-158">Contains the item identifier of an exported item.</span></span>  <br/> |
|[<span data-ttu-id="96b77-159">Dados (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="96b77-159">Data (base64Binary)</span></span>](data-base64binary.md) <br/> |<span data-ttu-id="96b77-160">Contém o conteúdo de um item exportado.</span><span class="sxs-lookup"><span data-stu-id="96b77-160">Contains the contents of an exported item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="96b77-161">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="96b77-161">Parent elements</span></span>

|<span data-ttu-id="96b77-162">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="96b77-162">**Element**</span></span>|<span data-ttu-id="96b77-163">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96b77-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96b77-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="96b77-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="96b77-165">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="96b77-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="96b77-166">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="96b77-166">Text value</span></span>

<span data-ttu-id="96b77-167">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="96b77-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="96b77-168">Comentários</span><span class="sxs-lookup"><span data-stu-id="96b77-168">Remarks</span></span>

<span data-ttu-id="96b77-169">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="96b77-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96b77-170">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="96b77-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96b77-171">Namespace</span><span class="sxs-lookup"><span data-stu-id="96b77-171">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="96b77-172">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="96b77-172">Schema Name</span></span>  <br/> |<span data-ttu-id="96b77-173">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="96b77-173">Message schema</span></span>  <br/> |
|<span data-ttu-id="96b77-174">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="96b77-174">Validation File</span></span>  <br/> |<span data-ttu-id="96b77-175">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="96b77-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="96b77-176">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="96b77-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="96b77-177">False</span><span class="sxs-lookup"><span data-stu-id="96b77-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96b77-178">Confira também</span><span class="sxs-lookup"><span data-stu-id="96b77-178">See also</span></span>

- [<span data-ttu-id="96b77-179">Operação ExportItems</span><span class="sxs-lookup"><span data-stu-id="96b77-179">ExportItems operation</span></span>](exportitems-operation.md) 
- [<span data-ttu-id="96b77-180">Operação UploadItems</span><span class="sxs-lookup"><span data-stu-id="96b77-180">UploadItems operation</span></span>](uploaditems-operation.md)

