---
title: Operação RemoveDistributionGroupFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 252bddf2-98b6-4824-b548-2fba2bda5384
description: Encontre informações sobre a operação do EWS do RemoveDistributionGroupFromImList.
ms.openlocfilehash: 66220f0cab99f404e17136bbb7836ca13d569b53
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459599"
---
# <a name="removedistributiongroupfromimlist-operation"></a><span data-ttu-id="95d40-103">Operação RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="95d40-103">RemoveDistributionGroupFromImList operation</span></span>

<span data-ttu-id="95d40-104">Encontre informações sobre a operação do EWS do **RemoveDistributionGroupFromImList** .</span><span class="sxs-lookup"><span data-stu-id="95d40-104">Find information about the **RemoveDistributionGroupFromImList** EWS operation.</span></span> 
  
<span data-ttu-id="95d40-105">A operação **RemoveDistributionGroupFromImList** remove um grupo de distribuição da lista de IM (mensagens instantâneas) do Lync quando o Lync usa o Exchange para o repositório de contatos.</span><span class="sxs-lookup"><span data-stu-id="95d40-105">The **RemoveDistributionGroupFromImList** operation removes a distribution group from the Lync instant messaging (IM) list when Lync uses Exchange for the contact store.</span></span> 
  
<span data-ttu-id="95d40-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="95d40-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removedistributiongroupfromimlist-operation"></a><span data-ttu-id="95d40-107">Usando a operação RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="95d40-107">Using the RemoveDistributionGroupFromImList operation</span></span>

<span data-ttu-id="95d40-108">A operação **RemoveDistributionGroupFromImList** aceita um único argumento que identifica um grupo de distribuição a ser removido da lista de mensagens instantâneas do Lync armazenada em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="95d40-108">The **RemoveDistributionGroupFromImList** operation accepts a single argument that identifies a distribution group to remove from the Lync IM list stored on an Exchange server.</span></span> 
  
### <a name="removedistributiongroupfromimlist-operation-soap-headers"></a><span data-ttu-id="95d40-109">Cabeçalhos SOAP de operação RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="95d40-109">RemoveDistributionGroupFromImList operation SOAP headers</span></span>

<span data-ttu-id="95d40-110">A operação **RemoveDistributionGroupFromImList** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="95d40-110">The **RemoveDistributionGroupFromImList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="95d40-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="95d40-111">**Header name**</span></span>|<span data-ttu-id="95d40-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="95d40-112">**Element**</span></span>|<span data-ttu-id="95d40-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="95d40-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="95d40-114">**Representação**</span><span class="sxs-lookup"><span data-stu-id="95d40-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="95d40-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="95d40-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="95d40-116">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="95d40-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="95d40-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="95d40-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="95d40-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="95d40-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="95d40-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="95d40-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="95d40-120">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="95d40-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="95d40-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="95d40-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="95d40-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="95d40-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="95d40-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="95d40-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="95d40-124">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="95d40-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="95d40-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="95d40-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="95d40-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="95d40-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="95d40-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="95d40-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="95d40-128">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="95d40-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="95d40-129">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="95d40-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removedistributiongroupfromimlist-operation-request-example-remove-a-distribution-group-from-an-im-list"></a><span data-ttu-id="95d40-130">Exemplo de solicitação de operação RemoveDistributionGroupFromImList: remover um grupo de distribuição de uma lista de mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="95d40-130">RemoveDistributionGroupFromImList operation request example: Remove a distribution group from an IM list</span></span>

<span data-ttu-id="95d40-131">O exemplo a seguir de uma solicitação de operação **RemoveDistributionGroupFromImList** mostra como remover um grupo de distribuição de um grupo de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="95d40-131">The following example of a **RemoveDistributionGroupFromImList** operation request shows how to remove a distribution group from an IM group.</span></span> <span data-ttu-id="95d40-132">A operação **RemoveDistributionGroupFromImList** aceita o identificador de grupo exclusivo para identificar o grupo de distribuição a ser removido da lista de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="95d40-132">The **RemoveDistributionGroupFromImList** operation accepts the unique group identifier to identify the distribution group to remove from the IM list.</span></span> <span data-ttu-id="95d40-133">O elemento [ExchangeStoreId](exchangestoreid.md) que é retornado na resposta para a [operação GetImItemList](getimitemlist-operation.md) e a [operação AddDistributionGroupToImList](adddistributiongrouptoimlist-operation.md) identifica os grupos de distribuição que podem ser removidos da lista de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="95d40-133">The [ExchangeStoreId](exchangestoreid.md) element that is returned in the response for the [GetImItemList operation](getimitemlist-operation.md) and the [AddDistributionGroupToImList operation](adddistributiongrouptoimlist-operation.md) identifies distribution groups that can be removed from the IM list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="95d40-134">Todos os identificadores de item e as chaves de alteração deste artigo foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="95d40-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:RemoveDistributionGroupFromImList>
         <m:GroupId Id="AAMkADEzO4QrAABmEh5oAAA="/>
      </m:RemoveDistributionGroupFromImList>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="95d40-135">Os seguintes elementos são usados na solicitação de corpo SOAP:</span><span class="sxs-lookup"><span data-stu-id="95d40-135">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="95d40-136">RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="95d40-136">RemoveDistributionGroupFromImList</span></span>](removedistributiongroupfromimlist.md)
    
- [<span data-ttu-id="95d40-137">GroupId</span><span class="sxs-lookup"><span data-stu-id="95d40-137">GroupId</span></span>](groupid.md)
    
## <a name="successful-removedistributiongroupfromimlist-operation-response"></a><span data-ttu-id="95d40-138">Resposta de operação RemoveDistributionGroupFromImList bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="95d40-138">Successful RemoveDistributionGroupFromImList operation response</span></span>

<span data-ttu-id="95d40-139">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **RemoveDistributionGroupFromImList** para um grupo de distribuição de um grupo de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="95d40-139">The following example shows a successful response to a **RemoveDistributionGroupFromImList** operation request to a remove a distribution group from an IM group.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveDistributionGroupFromImListResponse ResponseClass="Success" 
                                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveDistributionGroupFromImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="95d40-140">Os seguintes elementos são usados no corpo SOAP de resposta:</span><span class="sxs-lookup"><span data-stu-id="95d40-140">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="95d40-141">RemoveDistributionGroupFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="95d40-141">RemoveDistributionGroupFromImListResponse</span></span>](removedistributiongroupfromimlistresponse.md)
    
- [<span data-ttu-id="95d40-142">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="95d40-142">ResponseCode</span></span>](responsecode.md)
    
## <a name="removedistributiongroupfromimlist-operation-error-response-example"></a><span data-ttu-id="95d40-143">Exemplo de resposta de erro de operação RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="95d40-143">RemoveDistributionGroupFromImList operation error response example</span></span>

<span data-ttu-id="95d40-144">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **RemoveDistributionGroupFromImList** .</span><span class="sxs-lookup"><span data-stu-id="95d40-144">The following example shows an error response to a **RemoveDistributionGroupFromImList** operation request.</span></span> <span data-ttu-id="95d40-145">Esta é uma resposta a uma solicitação para remover um grupo de distribuição que já foi removido da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="95d40-145">This is a response to a request to remove a distribution group that has already been removed from the mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveDistributionGroupFromImListResponse ResponseClass="Error" 
                                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveDistributionGroupFromImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="95d40-146">Os seguintes elementos são usados no corpo SOAP de resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="95d40-146">The following elements are used in the error response SOAP body:</span></span>
  
- [<span data-ttu-id="95d40-147">RemoveDistributionGroupFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="95d40-147">RemoveDistributionGroupFromImListResponse</span></span>](removedistributiongroupfromimlistresponse.md)
    
- [<span data-ttu-id="95d40-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="95d40-148">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="95d40-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="95d40-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="95d40-150">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="95d40-150">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="95d40-151">Também consulte</span><span class="sxs-lookup"><span data-stu-id="95d40-151">See also</span></span>

- [<span data-ttu-id="95d40-152">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="95d40-152">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="95d40-153">Operação GetImItemList</span><span class="sxs-lookup"><span data-stu-id="95d40-153">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="95d40-154">Operação AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="95d40-154">AddDistributionGroupToImList operation</span></span>](adddistributiongrouptoimlist-operation.md)
    
- [<span data-ttu-id="95d40-155">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="95d40-155">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx#What)
    

