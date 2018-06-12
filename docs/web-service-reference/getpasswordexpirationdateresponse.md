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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752598"
---
# <a name="getpasswordexpirationdateresponse"></a><span data-ttu-id="e476c-103">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="e476c-103">GetPasswordExpirationDateResponse</span></span>

<span data-ttu-id="e476c-104">O elemento de **GetPasswordExpirationDateResponse** define a resposta a uma solicitação de operação [GetPasswordExpirationDate operação](getpasswordexpirationdate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e476c-104">The **GetPasswordExpirationDateResponse** element defines the response to a [GetPasswordExpirationDate operation](getpasswordexpirationdate-operation.md) operation request.</span></span> 
  
- [<span data-ttu-id="e476c-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e476c-105">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="e476c-106">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="e476c-106">GetPasswordExpirationDateResponse</span></span>](getpasswordexpirationdateresponse.md)
  
```XML
<GetPasswordExpirationDateResponse>
    <PasswordExpirationDate />
</GetPasswordExpirationDateResponse>
```

 <span data-ttu-id="e476c-107">**GetPasswordExpirationDateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e476c-107">**GetPasswordExpirationDateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e476c-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e476c-108">Attributes and elements</span></span>

<span data-ttu-id="e476c-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e476c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e476c-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="e476c-110">Attributes</span></span>

|<span data-ttu-id="e476c-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="e476c-111">**Attribute**</span></span>|<span data-ttu-id="e476c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e476c-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e476c-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="e476c-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="e476c-114">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="e476c-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="e476c-115">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="e476c-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="e476c-116">-Êxito</span><span class="sxs-lookup"><span data-stu-id="e476c-116">-  Success</span></span>  <br/><span data-ttu-id="e476c-117">-Aviso</span><span class="sxs-lookup"><span data-stu-id="e476c-117">-  Warning</span></span>  <br/><span data-ttu-id="e476c-118">-Erro</span><span class="sxs-lookup"><span data-stu-id="e476c-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="e476c-119">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e476c-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="e476c-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e476c-120">**Value**</span></span>|<span data-ttu-id="e476c-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e476c-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e476c-122">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="e476c-122">**Success**</span></span> <br/> |<span data-ttu-id="e476c-123">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="e476c-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="e476c-124">**Warning**</span><span class="sxs-lookup"><span data-stu-id="e476c-124">**Warning**</span></span> <br/> | <span data-ttu-id="e476c-125">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="e476c-125">Describes a request that was not processed.</span></span> <span data-ttu-id="e476c-126">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="e476c-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="e476c-127">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="e476c-127">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="e476c-128">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="e476c-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="e476c-129">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="e476c-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="e476c-130">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="e476c-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="e476c-131">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="e476c-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="e476c-132">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="e476c-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="e476c-133">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="e476c-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="e476c-134">**Erro**</span><span class="sxs-lookup"><span data-stu-id="e476c-134">**Error**</span></span> <br/> | <span data-ttu-id="e476c-135">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="e476c-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="e476c-136">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="e476c-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="e476c-137">-Inválido atributos e elementos.</span><span class="sxs-lookup"><span data-stu-id="e476c-137">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="e476c-138">-Atributos ou elementos que estão fora do intervalo.</span><span class="sxs-lookup"><span data-stu-id="e476c-138">-  Attributes or elements that are out of range.</span></span>  <br/><span data-ttu-id="e476c-139">-Uma marca desconhecida.</span><span class="sxs-lookup"><span data-stu-id="e476c-139">-  An unknown tag.</span></span>  <br/><span data-ttu-id="e476c-140">-Um atributo ou elemento que não é válido no contexto.</span><span class="sxs-lookup"><span data-stu-id="e476c-140">-  An attribute or element that is not valid in the context.</span></span>  <br/><span data-ttu-id="e476c-141">-Uma tentativa de acesso não autorizado por qualquer cliente.</span><span class="sxs-lookup"><span data-stu-id="e476c-141">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="e476c-142">-Uma falha no servidor em resposta a uma chamada de cliente válida.</span><span class="sxs-lookup"><span data-stu-id="e476c-142">-  A server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="e476c-143">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="e476c-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e476c-144">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e476c-144">Child elements</span></span>

|<span data-ttu-id="e476c-145">**Nome do elemento**</span><span class="sxs-lookup"><span data-stu-id="e476c-145">**Element name**</span></span>|<span data-ttu-id="e476c-146">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e476c-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e476c-147">PasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="e476c-147">PasswordExpirationDate</span></span>](passwordexpirationdate.md) <br/> |<span data-ttu-id="e476c-148">Fornece a data de expiração de senha para a conta de email especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="e476c-148">Provides the password expiration date for the email account specified in the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e476c-149">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e476c-149">Parent elements</span></span>

|<span data-ttu-id="e476c-150">**Nome do elemento**</span><span class="sxs-lookup"><span data-stu-id="e476c-150">**Element name**</span></span>|<span data-ttu-id="e476c-151">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e476c-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e476c-152">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e476c-152">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e476c-153">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="e476c-153">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e476c-154">Comentários</span><span class="sxs-lookup"><span data-stu-id="e476c-154">Remarks</span></span>

<span data-ttu-id="e476c-155">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e476c-155">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="e476c-156">Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="e476c-156">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e476c-157">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e476c-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e476c-158">Namespace</span><span class="sxs-lookup"><span data-stu-id="e476c-158">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e476c-159">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e476c-159">Schema Name</span></span>  <br/> |<span data-ttu-id="e476c-160">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e476c-160">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e476c-161">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e476c-161">Validation File</span></span>  <br/> |<span data-ttu-id="e476c-162">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e476c-162">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e476c-163">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e476c-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="e476c-164">False</span><span class="sxs-lookup"><span data-stu-id="e476c-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e476c-165">Ver também</span><span class="sxs-lookup"><span data-stu-id="e476c-165">See also</span></span>

- [<span data-ttu-id="e476c-166">Operação GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="e476c-166">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="e476c-167">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e476c-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

