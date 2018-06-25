---
title: FindMessageTrackingReportResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindMessageTrackingReportResponse
api_type:
- schema
ms.assetid: ed4265dc-0e79-4b34-8bf4-88a94875629d
description: O elemento FindMessageTrackingReportResponse contém o status e o resultado de uma única solicitação de operação FindMessageTrackingReport.
ms.openlocfilehash: fa381f500eac9a46b11aea8c813f1ffc625a3bc3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752298"
---
# <a name="findmessagetrackingreportresponse"></a><span data-ttu-id="845d2-103">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="845d2-103">FindMessageTrackingReportResponse</span></span>

<span data-ttu-id="845d2-104">O elemento **FindMessageTrackingReportResponse** contém o status e o resultado de uma única solicitação de [operação FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="845d2-104">The **FindMessageTrackingReportResponse** element contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span> 
  
```xml
<FindMessageTrackingReportResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Diagnostics/>
   <MessageTrackingSearchResults/>
   <Errors/>
   <Properties/>
</FindMessageTrackingReportResponse>
```

 <span data-ttu-id="845d2-105">**FindMessageTrackingReportResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="845d2-105">**FindMessageTrackingReportResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="845d2-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="845d2-106">Attributes and elements</span></span>

<span data-ttu-id="845d2-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="845d2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="845d2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="845d2-108">Attributes</span></span>

|<span data-ttu-id="845d2-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="845d2-109">**Attribute**</span></span>|<span data-ttu-id="845d2-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="845d2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="845d2-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="845d2-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="845d2-112">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="845d2-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="845d2-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="845d2-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="845d2-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="845d2-114">-  Success</span></span>  <br/><span data-ttu-id="845d2-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="845d2-115">-  Warning</span></span>  <br/><span data-ttu-id="845d2-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="845d2-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="845d2-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="845d2-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="845d2-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="845d2-118">**Value**</span></span>|<span data-ttu-id="845d2-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="845d2-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="845d2-120">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="845d2-120">**Success**</span></span> <br/> |<span data-ttu-id="845d2-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="845d2-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="845d2-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="845d2-122">**Warning**</span></span> <br/> | <span data-ttu-id="845d2-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="845d2-123">Describes a request that was not processed.</span></span> <span data-ttu-id="845d2-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="845d2-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="845d2-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="845d2-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="845d2-126">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="845d2-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="845d2-127">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="845d2-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="845d2-128">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="845d2-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="845d2-129">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="845d2-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="845d2-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="845d2-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="845d2-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="845d2-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="845d2-132">**Erro**</span><span class="sxs-lookup"><span data-stu-id="845d2-132">**Error**</span></span> <br/> | <span data-ttu-id="845d2-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="845d2-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="845d2-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="845d2-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="845d2-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="845d2-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="845d2-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="845d2-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="845d2-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="845d2-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="845d2-138">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="845d2-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="845d2-139">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="845d2-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="845d2-140">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="845d2-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="845d2-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="845d2-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="845d2-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="845d2-142">Child elements</span></span>

|<span data-ttu-id="845d2-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="845d2-143">**Element**</span></span>|<span data-ttu-id="845d2-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="845d2-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="845d2-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="845d2-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="845d2-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="845d2-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="845d2-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="845d2-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="845d2-148">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="845d2-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="845d2-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="845d2-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="845d2-150">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="845d2-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="845d2-151">Esse elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="845d2-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="845d2-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="845d2-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="845d2-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="845d2-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="845d2-154">Diagnósticos</span><span class="sxs-lookup"><span data-stu-id="845d2-154">Diagnostics</span></span>](diagnostics.md) <br/> |<span data-ttu-id="845d2-155">Contém informações que serão usadas para produzir vários relatórios de estatísticos para o recurso de rastreamento em um data center.</span><span class="sxs-lookup"><span data-stu-id="845d2-155">Contains information that will be used to produce various statistical reports for the tracking feature in a DataCenter.</span></span>  <br/> |
|[<span data-ttu-id="845d2-156">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="845d2-156">MessageTrackingSearchResults</span></span>](messagetrackingsearchresults.md) <br/> |<span data-ttu-id="845d2-157">Contém matriz de mensagens que correspondam aos requisitos de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="845d2-157">Contains and array of messages that match the search requirements.</span></span>  <br/> |
|[<span data-ttu-id="845d2-158">ExecutedSearchScope</span><span class="sxs-lookup"><span data-stu-id="845d2-158">ExecutedSearchScope</span></span>](executedsearchscope.md) <br/> |<span data-ttu-id="845d2-159">Contém o escopo da pesquisa que foi executada para obter os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="845d2-159">Contains the scope of the search that was performed to get the search results.</span></span>  <br/> |
|[<span data-ttu-id="845d2-160">Erros</span><span class="sxs-lookup"><span data-stu-id="845d2-160">Errors</span></span>](errors-ex15websvcsotherref.md) <br/> |<span data-ttu-id="845d2-161">Contém um recipiente de propriedades para armazenar os erros são retornados pelo serviço Web.</span><span class="sxs-lookup"><span data-stu-id="845d2-161">Contains a property bag to store errors that are returned through the Web service.</span></span>  <br/> |
|[<span data-ttu-id="845d2-162">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="845d2-162">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="845d2-163">Contém uma lista de uma ou mais propriedades de controle.</span><span class="sxs-lookup"><span data-stu-id="845d2-163">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="845d2-164">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="845d2-164">Parent elements</span></span>

<span data-ttu-id="845d2-165">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="845d2-165">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="845d2-166">Text value</span><span class="sxs-lookup"><span data-stu-id="845d2-166">Text value</span></span>

<span data-ttu-id="845d2-167">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="845d2-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="845d2-168">Comentários</span><span class="sxs-lookup"><span data-stu-id="845d2-168">Remarks</span></span>

<span data-ttu-id="845d2-169">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="845d2-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="845d2-170">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="845d2-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="845d2-171">Namespace</span><span class="sxs-lookup"><span data-stu-id="845d2-171">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="845d2-172">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="845d2-172">Schema Name</span></span>  <br/> |<span data-ttu-id="845d2-173">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="845d2-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="845d2-174">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="845d2-174">Validation File</span></span>  <br/> |<span data-ttu-id="845d2-175">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="845d2-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="845d2-176">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="845d2-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="845d2-177">False</span><span class="sxs-lookup"><span data-stu-id="845d2-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="845d2-178">Ver também</span><span class="sxs-lookup"><span data-stu-id="845d2-178">See also</span></span>

- [<span data-ttu-id="845d2-179">Operação FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="845d2-179">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="845d2-180">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="845d2-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

