---
title: GetPasswordExpirationDateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d3fff1f-ef13-46d5-bd7f-ef535eb80c72
description: O elemento de GetPasswordExpirationDateResponse define a resposta a uma solicitação de operação de operação GetPasswordExpirationDate.
ms.openlocfilehash: 3754a53da53c12479f11c2e32cd15a08cba665fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752598"
---
# <a name="getpasswordexpirationdateresponse"></a><span data-ttu-id="48677-103">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="48677-103">GetPasswordExpirationDateResponse</span></span>

<span data-ttu-id="48677-104">O elemento de **GetPasswordExpirationDateResponse** define a resposta a uma solicitação de operação [GetPasswordExpirationDate operação](getpasswordexpirationdate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="48677-104">The **GetPasswordExpirationDateResponse** element defines the response to a [GetPasswordExpirationDate operation](getpasswordexpirationdate-operation.md) operation request.</span></span> 
  
- [<span data-ttu-id="48677-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="48677-105">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="48677-106">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="48677-106">GetPasswordExpirationDateResponse</span></span>](getpasswordexpirationdateresponse.md)
  
```XML
<GetPasswordExpirationDateResponse>
    <PasswordExpirationDate />
</GetPasswordExpirationDateResponse>
```

 <span data-ttu-id="48677-107">**GetPasswordExpirationDateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="48677-107">**GetPasswordExpirationDateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="48677-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="48677-108">Attributes and elements</span></span>

<span data-ttu-id="48677-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="48677-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="48677-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="48677-110">Attributes</span></span>

|<span data-ttu-id="48677-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="48677-111">**Attribute**</span></span>|<span data-ttu-id="48677-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="48677-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="48677-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="48677-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="48677-114">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="48677-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="48677-115">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="48677-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="48677-116">-Êxito</span><span class="sxs-lookup"><span data-stu-id="48677-116">-  Success</span></span>  <br/><span data-ttu-id="48677-117">-Aviso</span><span class="sxs-lookup"><span data-stu-id="48677-117">-  Warning</span></span>  <br/><span data-ttu-id="48677-118">-Erro</span><span class="sxs-lookup"><span data-stu-id="48677-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="48677-119">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="48677-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="48677-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="48677-120">**Value**</span></span>|<span data-ttu-id="48677-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="48677-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="48677-122">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="48677-122">**Success**</span></span> <br/> |<span data-ttu-id="48677-123">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="48677-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="48677-124">**Warning**</span><span class="sxs-lookup"><span data-stu-id="48677-124">**Warning**</span></span> <br/> | <span data-ttu-id="48677-125">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="48677-125">Describes a request that was not processed.</span></span> <span data-ttu-id="48677-126">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="48677-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="48677-127">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="48677-127">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="48677-128">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="48677-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="48677-129">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="48677-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="48677-130">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="48677-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="48677-131">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="48677-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="48677-132">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="48677-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="48677-133">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="48677-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="48677-134">**Erro**</span><span class="sxs-lookup"><span data-stu-id="48677-134">**Error**</span></span> <br/> | <span data-ttu-id="48677-135">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="48677-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="48677-136">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="48677-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="48677-137">-Inválido atributos e elementos.</span><span class="sxs-lookup"><span data-stu-id="48677-137">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="48677-138">-Atributos ou elementos que estão fora do intervalo.</span><span class="sxs-lookup"><span data-stu-id="48677-138">-  Attributes or elements that are out of range.</span></span>  <br/><span data-ttu-id="48677-139">-Uma marca desconhecida.</span><span class="sxs-lookup"><span data-stu-id="48677-139">-  An unknown tag.</span></span>  <br/><span data-ttu-id="48677-140">-Um atributo ou elemento que não é válido no contexto.</span><span class="sxs-lookup"><span data-stu-id="48677-140">-  An attribute or element that is not valid in the context.</span></span>  <br/><span data-ttu-id="48677-141">-Uma tentativa de acesso não autorizado por qualquer cliente.</span><span class="sxs-lookup"><span data-stu-id="48677-141">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="48677-142">-Uma falha no servidor em resposta a uma chamada de cliente válida.</span><span class="sxs-lookup"><span data-stu-id="48677-142">-  A server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="48677-143">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="48677-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="48677-144">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="48677-144">Child elements</span></span>

|<span data-ttu-id="48677-145">**Nome do elemento**</span><span class="sxs-lookup"><span data-stu-id="48677-145">**Element name**</span></span>|<span data-ttu-id="48677-146">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="48677-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48677-147">PasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="48677-147">PasswordExpirationDate</span></span>](passwordexpirationdate.md) <br/> |<span data-ttu-id="48677-148">Fornece a data de expiração de senha para a conta de email especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="48677-148">Provides the password expiration date for the email account specified in the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="48677-149">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="48677-149">Parent elements</span></span>

|<span data-ttu-id="48677-150">**Nome do elemento**</span><span class="sxs-lookup"><span data-stu-id="48677-150">**Element name**</span></span>|<span data-ttu-id="48677-151">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="48677-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48677-152">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="48677-152">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="48677-153">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="48677-153">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="48677-154">Comentários</span><span class="sxs-lookup"><span data-stu-id="48677-154">Remarks</span></span>

<span data-ttu-id="48677-155">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="48677-155">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="48677-156">Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="48677-156">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="48677-157">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="48677-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="48677-158">Namespace</span><span class="sxs-lookup"><span data-stu-id="48677-158">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="48677-159">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="48677-159">Schema Name</span></span>  <br/> |<span data-ttu-id="48677-160">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="48677-160">Messages schema</span></span>  <br/> |
|<span data-ttu-id="48677-161">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="48677-161">Validation File</span></span>  <br/> |<span data-ttu-id="48677-162">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="48677-162">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="48677-163">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="48677-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="48677-164">False</span><span class="sxs-lookup"><span data-stu-id="48677-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="48677-165">Ver também</span><span class="sxs-lookup"><span data-stu-id="48677-165">See also</span></span>

- [<span data-ttu-id="48677-166">Operação GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="48677-166">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="48677-167">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="48677-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

