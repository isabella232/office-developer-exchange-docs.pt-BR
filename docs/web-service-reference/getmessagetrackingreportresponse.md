---
title: GetMessageTrackingReportResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMessageTrackingReportResponse
api_type:
- schema
ms.assetid: 41177894-2008-44a6-86f8-bc34c0a48e36
description: O elemento GetMessageTrackingReportResponse contém a resposta para a operação GetMessageTrackingReport.
ms.openlocfilehash: bdb8b97e57f92a32cbdc498d09297920366b58bd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752562"
---
# <a name="getmessagetrackingreportresponse"></a><span data-ttu-id="2da24-103">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="2da24-103">GetMessageTrackingReportResponse</span></span>

<span data-ttu-id="2da24-104">O elemento **GetMessageTrackingReportResponse** contém a resposta para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="2da24-104">The **GetMessageTrackingReportResponse** element contains the response for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>
  
```xml
<GetMessageTrackingReportResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MessageTrackingReport/>
   <Diagnostics/>
   <Errors/>
   <Properties/>
</GetMessageTrackingReportResponse>
```

 <span data-ttu-id="2da24-105">**GetMessageTrackingReportResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="2da24-105">**GetMessageTrackingReportResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2da24-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2da24-106">Attributes and elements</span></span>

<span data-ttu-id="2da24-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2da24-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2da24-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2da24-108">Attributes</span></span>

|<span data-ttu-id="2da24-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="2da24-109">**Attribute**</span></span>|<span data-ttu-id="2da24-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2da24-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2da24-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="2da24-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="2da24-112">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="2da24-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="2da24-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="2da24-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="2da24-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="2da24-114">-  Success</span></span>  <br/><span data-ttu-id="2da24-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="2da24-115">-  Warning</span></span>  <br/><span data-ttu-id="2da24-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="2da24-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="2da24-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="2da24-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="2da24-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="2da24-118">**Value**</span></span>|<span data-ttu-id="2da24-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2da24-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2da24-120">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="2da24-120">**Success**</span></span> <br/> |<span data-ttu-id="2da24-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="2da24-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="2da24-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="2da24-122">**Warning**</span></span> <br/> | <span data-ttu-id="2da24-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="2da24-123">Describes a request that was not processed.</span></span> <span data-ttu-id="2da24-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="2da24-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="2da24-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="2da24-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="2da24-126">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="2da24-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="2da24-127">-Ativo serve de domínio Directory (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="2da24-127">-  Active Directory Domain Serves (AD DS) is offline.</span></span>  <br/><span data-ttu-id="2da24-128">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="2da24-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="2da24-129">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="2da24-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="2da24-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="2da24-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="2da24-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="2da24-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="2da24-132">**Erro**</span><span class="sxs-lookup"><span data-stu-id="2da24-132">**Error**</span></span> <br/> | <span data-ttu-id="2da24-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="2da24-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="2da24-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="2da24-134">The following are examples of sources of errors:</span></span>  <br/>  <span data-ttu-id="2da24-135">Elementos ou atributos inválidos</span><span class="sxs-lookup"><span data-stu-id="2da24-135">Invalid attributes or elements</span></span>  <br/><br/><span data-ttu-id="2da24-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="2da24-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="2da24-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="2da24-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="2da24-138">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="2da24-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="2da24-139">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="2da24-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="2da24-140">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="2da24-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="2da24-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="2da24-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2da24-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2da24-142">Child elements</span></span>

|<span data-ttu-id="2da24-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2da24-143">**Element**</span></span>|<span data-ttu-id="2da24-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2da24-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2da24-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="2da24-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="2da24-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="2da24-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="2da24-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2da24-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="2da24-148">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2da24-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="2da24-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="2da24-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="2da24-150">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="2da24-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="2da24-151">Esse elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="2da24-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="2da24-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="2da24-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="2da24-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="2da24-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="2da24-154">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="2da24-154">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="2da24-155">Contém uma única mensagem retornada em uma [operação de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="2da24-155">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="2da24-156">Diagnósticos</span><span class="sxs-lookup"><span data-stu-id="2da24-156">Diagnostics</span></span>](diagnostics.md) <br/> |<span data-ttu-id="2da24-157">Fornece informações de tempo e de desempenho que são usadas para relatórios em um data center.</span><span class="sxs-lookup"><span data-stu-id="2da24-157">Provides timing and performance information that is used for reporting in a DataCenter.</span></span>  <br/> |
|[<span data-ttu-id="2da24-158">Erros</span><span class="sxs-lookup"><span data-stu-id="2da24-158">Errors</span></span>](errors-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2da24-159">Contém um recipiente de propriedades para armazenar os erros são retornados pelo serviço Web.</span><span class="sxs-lookup"><span data-stu-id="2da24-159">Contains a property bag to store errors that are returned through the Web service.</span></span>  <br/> |
|[<span data-ttu-id="2da24-160">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="2da24-160">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="2da24-161">Contém uma lista de uma ou mais propriedades de controle.</span><span class="sxs-lookup"><span data-stu-id="2da24-161">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2da24-162">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2da24-162">Parent elements</span></span>

<span data-ttu-id="2da24-163">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2da24-163">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="2da24-164">Text value</span><span class="sxs-lookup"><span data-stu-id="2da24-164">Text value</span></span>

<span data-ttu-id="2da24-165">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2da24-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2da24-166">Comentários</span><span class="sxs-lookup"><span data-stu-id="2da24-166">Remarks</span></span>

<span data-ttu-id="2da24-167">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2da24-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2da24-168">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2da24-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2da24-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="2da24-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2da24-170">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2da24-170">Schema Name</span></span>  <br/> |<span data-ttu-id="2da24-171">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="2da24-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2da24-172">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2da24-172">Validation File</span></span>  <br/> |<span data-ttu-id="2da24-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2da24-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2da24-174">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2da24-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="2da24-175">False</span><span class="sxs-lookup"><span data-stu-id="2da24-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2da24-176">Ver também</span><span class="sxs-lookup"><span data-stu-id="2da24-176">See also</span></span>

- [<span data-ttu-id="2da24-177">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="2da24-177">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="2da24-178">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2da24-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

