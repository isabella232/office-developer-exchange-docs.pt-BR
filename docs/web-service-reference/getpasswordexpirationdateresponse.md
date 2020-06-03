---
title: GetPasswordExpirationDateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d3fff1f-ef13-46d5-bd7f-ef535eb80c72
description: O elemento GetPasswordExpirationDateResponse define a resposta para uma solicitação de operação de operação GetPasswordExpirationDate.
ms.openlocfilehash: c925b2b37879ba0f8f25b2dd73737ed2f3202555
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530201"
---
# <a name="getpasswordexpirationdateresponse"></a><span data-ttu-id="0df1a-103">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="0df1a-103">GetPasswordExpirationDateResponse</span></span>

<span data-ttu-id="0df1a-104">O elemento **GetPasswordExpirationDateResponse** define a resposta para uma solicitação de operação de [operação GetPasswordExpirationDate](getpasswordexpirationdate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0df1a-104">The **GetPasswordExpirationDateResponse** element defines the response to a [GetPasswordExpirationDate operation](getpasswordexpirationdate-operation.md) operation request.</span></span> 
  
- [<span data-ttu-id="0df1a-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0df1a-105">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="0df1a-106">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="0df1a-106">GetPasswordExpirationDateResponse</span></span>](getpasswordexpirationdateresponse.md)
  
```XML
<GetPasswordExpirationDateResponse>
    <PasswordExpirationDate />
</GetPasswordExpirationDateResponse>
```

 <span data-ttu-id="0df1a-107">**GetPasswordExpirationDateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0df1a-107">**GetPasswordExpirationDateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0df1a-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0df1a-108">Attributes and elements</span></span>

<span data-ttu-id="0df1a-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0df1a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0df1a-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="0df1a-110">Attributes</span></span>

|<span data-ttu-id="0df1a-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="0df1a-111">**Attribute**</span></span>|<span data-ttu-id="0df1a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0df1a-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0df1a-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="0df1a-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="0df1a-114">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="0df1a-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="0df1a-115">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="0df1a-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="0df1a-116">-Êxito</span><span class="sxs-lookup"><span data-stu-id="0df1a-116">-  Success</span></span>  <br/><span data-ttu-id="0df1a-117">-Aviso</span><span class="sxs-lookup"><span data-stu-id="0df1a-117">-  Warning</span></span>  <br/><span data-ttu-id="0df1a-118">-Erro</span><span class="sxs-lookup"><span data-stu-id="0df1a-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="0df1a-119">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0df1a-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="0df1a-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="0df1a-120">**Value**</span></span>|<span data-ttu-id="0df1a-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0df1a-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0df1a-122">**Success**</span><span class="sxs-lookup"><span data-stu-id="0df1a-122">**Success**</span></span> <br/> |<span data-ttu-id="0df1a-123">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="0df1a-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="0df1a-124">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="0df1a-124">**Warning**</span></span> <br/> | <span data-ttu-id="0df1a-125">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="0df1a-125">Describes a request that was not processed.</span></span> <span data-ttu-id="0df1a-126">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="0df1a-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="0df1a-127">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="0df1a-127">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="0df1a-128">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="0df1a-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="0df1a-129">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="0df1a-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="0df1a-130">-As caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="0df1a-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="0df1a-131">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="0df1a-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="0df1a-132">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="0df1a-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="0df1a-133">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="0df1a-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="0df1a-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="0df1a-134">**Error**</span></span> <br/> | <span data-ttu-id="0df1a-135">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="0df1a-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="0df1a-136">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="0df1a-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="0df1a-137">-Atributos ou elementos inválidos.</span><span class="sxs-lookup"><span data-stu-id="0df1a-137">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="0df1a-138">-Atributos ou elementos que estão fora do intervalo.</span><span class="sxs-lookup"><span data-stu-id="0df1a-138">-  Attributes or elements that are out of range.</span></span>  <br/><span data-ttu-id="0df1a-139">-Uma marca desconhecida.</span><span class="sxs-lookup"><span data-stu-id="0df1a-139">-  An unknown tag.</span></span>  <br/><span data-ttu-id="0df1a-140">-Um atributo ou elemento que não é válido no contexto.</span><span class="sxs-lookup"><span data-stu-id="0df1a-140">-  An attribute or element that is not valid in the context.</span></span>  <br/><span data-ttu-id="0df1a-141">– Uma tentativa de acesso não autorizado por qualquer cliente.</span><span class="sxs-lookup"><span data-stu-id="0df1a-141">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="0df1a-142">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente.</span><span class="sxs-lookup"><span data-stu-id="0df1a-142">-  A server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="0df1a-143">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="0df1a-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0df1a-144">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0df1a-144">Child elements</span></span>

|<span data-ttu-id="0df1a-145">**Nome do elemento**</span><span class="sxs-lookup"><span data-stu-id="0df1a-145">**Element name**</span></span>|<span data-ttu-id="0df1a-146">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0df1a-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0df1a-147">PasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="0df1a-147">PasswordExpirationDate</span></span>](passwordexpirationdate.md) <br/> |<span data-ttu-id="0df1a-148">Fornece a data de expiração da senha para a conta de email especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="0df1a-148">Provides the password expiration date for the email account specified in the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0df1a-149">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0df1a-149">Parent elements</span></span>

|<span data-ttu-id="0df1a-150">**Nome do elemento**</span><span class="sxs-lookup"><span data-stu-id="0df1a-150">**Element name**</span></span>|<span data-ttu-id="0df1a-151">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0df1a-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0df1a-152">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0df1a-152">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0df1a-153">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="0df1a-153">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0df1a-154">Comentários</span><span class="sxs-lookup"><span data-stu-id="0df1a-154">Remarks</span></span>

<span data-ttu-id="0df1a-155">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0df1a-155">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="0df1a-156">Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="0df1a-156">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0df1a-157">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0df1a-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0df1a-158">Namespace</span><span class="sxs-lookup"><span data-stu-id="0df1a-158">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0df1a-159">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0df1a-159">Schema Name</span></span>  <br/> |<span data-ttu-id="0df1a-160">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0df1a-160">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0df1a-161">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0df1a-161">Validation File</span></span>  <br/> |<span data-ttu-id="0df1a-162">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0df1a-162">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0df1a-163">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0df1a-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="0df1a-164">False</span><span class="sxs-lookup"><span data-stu-id="0df1a-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0df1a-165">Confira também</span><span class="sxs-lookup"><span data-stu-id="0df1a-165">See also</span></span>

- [<span data-ttu-id="0df1a-166">Operação GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="0df1a-166">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="0df1a-167">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0df1a-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

