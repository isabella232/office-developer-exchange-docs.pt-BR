---
title: Operação AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a
description: Encontre informações sobre a operação do EWS do AddDistributionGroupToImList.
ms.openlocfilehash: e68e21b6994af5773f5cf991d55129e1db3367ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463689"
---
# <a name="adddistributiongrouptoimlist-operation"></a><span data-ttu-id="55ef8-103">Operação AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="55ef8-103">AddDistributionGroupToImList operation</span></span>

<span data-ttu-id="55ef8-104">Encontre informações sobre a operação do EWS do **AddDistributionGroupToImList** .</span><span class="sxs-lookup"><span data-stu-id="55ef8-104">Find information about the **AddDistributionGroupToImList** EWS operation.</span></span> 
  
<span data-ttu-id="55ef8-105">A operação do **AddDistributionGroupToImList** do serviços Web do Exchange (EWS) adiciona um grupo de distribuição à lista de mensagens instantâneas (IM) no repositório unificado de contatos.</span><span class="sxs-lookup"><span data-stu-id="55ef8-105">The **AddDistributionGroupToImList** Exchange Web Services (EWS) operation adds a distribution group to the instant messaging (IM) list in the Unified Contact Store.</span></span> 
  
<span data-ttu-id="55ef8-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="55ef8-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-adddistributiongrouptoimlist-operation"></a><span data-ttu-id="55ef8-107">Usando a operação AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="55ef8-107">Using the AddDistributionGroupToImList operation</span></span>

<span data-ttu-id="55ef8-108">A operação **AddDistributionGroupToImList** aceita um único argumento que identifica um grupo de distribuição para adicionar à lista de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="55ef8-108">The **AddDistributionGroupToImList** operation takes a single argument that identifies a distribution group to add to the IM list.</span></span> <span data-ttu-id="55ef8-109">Essa operação não cria um grupo de distribuição; o grupo de distribuição já deve ser criado.</span><span class="sxs-lookup"><span data-stu-id="55ef8-109">This operation does not create a distribution group; the distribution group must already be created.</span></span> 
  
<span data-ttu-id="55ef8-110">Essa operação pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="55ef8-110">This operation can use the SOAP headers that are listed in the following table.</span></span>
  
<span data-ttu-id="55ef8-111">**Tabela 1. Cabeçalhos SOAP de operação AddDistributionGroupToImList**</span><span class="sxs-lookup"><span data-stu-id="55ef8-111">**Table 1. AddDistributionGroupToImList operation SOAP headers**</span></span>

|<span data-ttu-id="55ef8-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="55ef8-112">**Header name**</span></span>|<span data-ttu-id="55ef8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="55ef8-113">**Element**</span></span>|<span data-ttu-id="55ef8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="55ef8-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="55ef8-115">**Representação**</span><span class="sxs-lookup"><span data-stu-id="55ef8-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="55ef8-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="55ef8-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="55ef8-117">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="55ef8-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="55ef8-118">Isso se aplica a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="55ef8-118">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="55ef8-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="55ef8-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="55ef8-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="55ef8-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="55ef8-121">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="55ef8-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="55ef8-122">Isso se aplica a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="55ef8-122">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="55ef8-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="55ef8-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="55ef8-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="55ef8-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="55ef8-125">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="55ef8-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="55ef8-126">Isso se aplica a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="55ef8-126">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="55ef8-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="55ef8-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="55ef8-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="55ef8-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="55ef8-129">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="55ef8-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="55ef8-130">Isso se aplica a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="55ef8-130">This is applicable to a response.</span></span>  <br/> |
   
## <a name="adddistributiongrouptoimlist-operation-request-example"></a><span data-ttu-id="55ef8-131">Exemplo de solicitação de operação AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="55ef8-131">AddDistributionGroupToImList operation request example</span></span>

<span data-ttu-id="55ef8-132">O exemplo a seguir de uma solicitação de operação do **AddDistributionGroupToImList** mostra como adicionar um grupo de distribuição à lista de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="55ef8-132">The following example of an **AddDistributionGroupToImList** operation request shows how to add a distribution group to the IM list.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:AddDistributionGroupToImList>
         <m:SmtpAddress>distributionlist1@example.com</m:SmtpAddress>
      </m:AddDistributionGroupToImList>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="55ef8-133">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="55ef8-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="55ef8-134">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="55ef8-134">AddDistributionGroupToImList</span></span>](adddistributiongrouptoimlist.md)   
- [<span data-ttu-id="55ef8-135">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="55ef8-135">SmtpAddress</span></span>](smtpaddress.md)
    
## <a name="successful-adddistributiongrouptoimlist-operation-response"></a><span data-ttu-id="55ef8-136">Resposta de operação AddDistributionGroupToImList bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="55ef8-136">Successful AddDistributionGroupToImList operation response</span></span>

<span data-ttu-id="55ef8-137">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **AddDistributionGroupToImList** .</span><span class="sxs-lookup"><span data-stu-id="55ef8-137">The following example shows a successful response to an **AddDistributionGroupToImList** operation request.</span></span> 
  
<span data-ttu-id="55ef8-138">A resposta bem-sucedida contém o nome de exibição do grupo de distribuição, a classe de repositório do Exchange para o grupo de distribuição e o identificador do EWS do novo grupo de distribuição.</span><span class="sxs-lookup"><span data-stu-id="55ef8-138">The successful response contains the distribution group display name, the Exchange store class for the distribution group, and the EWS identifier of the new distribution group.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"
            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
            xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <s:Header>
      <t:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013"/>
   </s:Header>
   <s:Body>
      <m:AddDistributionGroupToImListResponse ResponseClass="Success">
         <m:ResponseCode>NoError</m:ResponseCode>
         <m:ImGroup>
            <t:DisplayName>distributionlist1@example.com</t:DisplayName>
            <t:GroupType>IPM.DistList.MOC.DG</t:GroupType>
            <t:ExchangeStoreId Id="AAMkAGQ1MjJjAA=" 
                             ChangeKey="EgAAAA=="/>
      </m:ImGroup>
      </m:AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="55ef8-139">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="55ef8-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="55ef8-140">AddDistributionGroupToImListResponse</span><span class="sxs-lookup"><span data-stu-id="55ef8-140">AddDistributionGroupToImListResponse</span></span>](adddistributiongrouptoimlistresponse.md)
    
- [<span data-ttu-id="55ef8-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="55ef8-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="55ef8-142">Imgroup</span><span class="sxs-lookup"><span data-stu-id="55ef8-142">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="55ef8-143">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="55ef8-143">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="55ef8-144">GroupType</span><span class="sxs-lookup"><span data-stu-id="55ef8-144">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="55ef8-145">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="55ef8-145">ExchangeStoreId</span></span>](exchangestoreid.md)
    
## <a name="adddistributiongrouptoimlist-operation-errorinvalidimdistributiongroupsmtpaddress-error-response"></a><span data-ttu-id="55ef8-146">Resposta de erro ErrorInvalidImDistributionGroupSmtpAddress operação AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="55ef8-146">AddDistributionGroupToImList operation ErrorInvalidImDistributionGroupSmtpAddress error response</span></span>

<span data-ttu-id="55ef8-147">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **AddDistributionGroupToImList** .</span><span class="sxs-lookup"><span data-stu-id="55ef8-147">The following example shows an error response to an **AddDistributionGroupToImList** operation request.</span></span> <span data-ttu-id="55ef8-148">A seguinte resposta de erro ocorre quando é feita uma tentativa de adicionar um grupo de distribuição que não existe no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="55ef8-148">The following error response occurs when an attempt is made to add a distribution group that does not exist in the Exchange store.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddDistributionGroupToImListResponse ResponseClass="Error" 
                                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified IM distribution group SMTP address is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImDistributionGroupSmtpAddress</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="55ef8-149">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="55ef8-149">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="55ef8-150">AddDistributionGroupToImListResponse</span><span class="sxs-lookup"><span data-stu-id="55ef8-150">AddDistributionGroupToImListResponse</span></span>](adddistributiongrouptoimlistresponse.md)
    
- [<span data-ttu-id="55ef8-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="55ef8-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="55ef8-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="55ef8-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="55ef8-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="55ef8-153">See also</span></span>

- [<span data-ttu-id="55ef8-154">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="55ef8-154">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)   
- [<span data-ttu-id="55ef8-155">AddImGroup</span><span class="sxs-lookup"><span data-stu-id="55ef8-155">AddImGroup</span></span>](addimgroup-operation.md)   
- [<span data-ttu-id="55ef8-156">RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="55ef8-156">RemoveImGroup</span></span>](removeimgroup-operation.md)
    

