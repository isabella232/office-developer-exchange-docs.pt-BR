---
title: Operação AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a
description: Encontre informações sobre o EWS AddDistributionGroupToImList operação.
ms.openlocfilehash: 7c562c317890a4cffb9e5844ea41c1096a8595b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751045"
---
# <a name="adddistributiongrouptoimlist-operation"></a><span data-ttu-id="b6c08-103">Operação AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="b6c08-103">AddDistributionGroupToImList operation</span></span>

<span data-ttu-id="b6c08-104">Encontre informações sobre a operação de EWS **AddDistributionGroupToImList** .</span><span class="sxs-lookup"><span data-stu-id="b6c08-104">Find information about the **AddDistributionGroupToImList** EWS operation.</span></span> 
  
<span data-ttu-id="b6c08-105">A operação de serviços Web do Exchange (EWS) **AddDistributionGroupToImList** adiciona um grupo de distribuição para a lista (IM) no repositório de contato de Unificação de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="b6c08-105">The **AddDistributionGroupToImList** Exchange Web Services (EWS) operation adds a distribution group to the instant messaging (IM) list in the Unified Contact Store.</span></span> 
  
<span data-ttu-id="b6c08-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b6c08-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-adddistributiongrouptoimlist-operation"></a><span data-ttu-id="b6c08-107">Usando a operação AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="b6c08-107">Using the AddDistributionGroupToImList operation</span></span>

<span data-ttu-id="b6c08-108">A operação **AddDistributionGroupToImList** aceita um argumento único que identifica um grupo de distribuição para adicionar à lista de mensagens Instantâneas.</span><span class="sxs-lookup"><span data-stu-id="b6c08-108">The **AddDistributionGroupToImList** operation takes a single argument that identifies a distribution group to add to the IM list.</span></span> <span data-ttu-id="b6c08-109">Esta operação não cria um grupo de distribuição; o grupo de distribuição já deve ser criado.</span><span class="sxs-lookup"><span data-stu-id="b6c08-109">This operation does not create a distribution group; the distribution group must already be created.</span></span> 
  
<span data-ttu-id="b6c08-110">Esta operação pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="b6c08-110">This operation can use the SOAP headers that are listed in the following table.</span></span>
  
<span data-ttu-id="b6c08-111">**Tabela 1. Cabeçalhos SOAP AddDistributionGroupToImList operação**</span><span class="sxs-lookup"><span data-stu-id="b6c08-111">**Table 1. AddDistributionGroupToImList operation SOAP headers**</span></span>

|<span data-ttu-id="b6c08-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="b6c08-112">**Header name**</span></span>|<span data-ttu-id="b6c08-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b6c08-113">**Element**</span></span>|<span data-ttu-id="b6c08-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b6c08-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b6c08-115">**Representação**</span><span class="sxs-lookup"><span data-stu-id="b6c08-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="b6c08-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="b6c08-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="b6c08-117">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="b6c08-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="b6c08-118">Isso é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6c08-118">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b6c08-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="b6c08-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="b6c08-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="b6c08-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="b6c08-121">Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b6c08-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="b6c08-122">Isso é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6c08-122">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b6c08-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="b6c08-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="b6c08-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="b6c08-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="b6c08-125">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="b6c08-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="b6c08-126">Isso é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6c08-126">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b6c08-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="b6c08-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="b6c08-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b6c08-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="b6c08-129">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6c08-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="b6c08-130">Isso é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="b6c08-130">This is applicable to a response.</span></span>  <br/> |
   
## <a name="adddistributiongrouptoimlist-operation-request-example"></a><span data-ttu-id="b6c08-131">Exemplo de solicitação de operação AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="b6c08-131">AddDistributionGroupToImList operation request example</span></span>

<span data-ttu-id="b6c08-132">O exemplo a seguir de uma solicitação de operação **AddDistributionGroupToImList** mostra como adicionar um grupo de distribuição à lista de mensagens Instantâneas.</span><span class="sxs-lookup"><span data-stu-id="b6c08-132">The following example of an **AddDistributionGroupToImList** operation request shows how to add a distribution group to the IM list.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="b6c08-133">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b6c08-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b6c08-134">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="b6c08-134">AddDistributionGroupToImList</span></span>](adddistributiongrouptoimlist.md)   
- [<span data-ttu-id="b6c08-135">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="b6c08-135">SmtpAddress</span></span>](smtpaddress.md)
    
## <a name="successful-adddistributiongrouptoimlist-operation-response"></a><span data-ttu-id="b6c08-136">Resposta de operação AddDistributionGroupToImList bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="b6c08-136">Successful AddDistributionGroupToImList operation response</span></span>

<span data-ttu-id="b6c08-137">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **AddDistributionGroupToImList** .</span><span class="sxs-lookup"><span data-stu-id="b6c08-137">The following example shows a successful response to an **AddDistributionGroupToImList** operation request.</span></span> 
  
<span data-ttu-id="b6c08-138">A resposta bem-sucedida contém o nome de exibição do grupo de distribuição, a classe de repositório do Exchange para o grupo de distribuição e o identificador do EWS do novo grupo de distribuição.</span><span class="sxs-lookup"><span data-stu-id="b6c08-138">The successful response contains the distribution group display name, the Exchange store class for the distribution group, and the EWS identifier of the new distribution group.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"
            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
            xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="b6c08-139">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b6c08-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b6c08-140">AddDistributionGroupToImListResponse</span><span class="sxs-lookup"><span data-stu-id="b6c08-140">AddDistributionGroupToImListResponse</span></span>](adddistributiongrouptoimlistresponse.md)
    
- [<span data-ttu-id="b6c08-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b6c08-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b6c08-142">ImGroup</span><span class="sxs-lookup"><span data-stu-id="b6c08-142">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="b6c08-143">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="b6c08-143">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="b6c08-144">GroupType</span><span class="sxs-lookup"><span data-stu-id="b6c08-144">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="b6c08-145">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="b6c08-145">ExchangeStoreId</span></span>](exchangestoreid.md)
    
## <a name="adddistributiongrouptoimlist-operation-errorinvalidimdistributiongroupsmtpaddress-error-response"></a><span data-ttu-id="b6c08-146">Operação AddDistributionGroupToImList ErrorInvalidImDistributionGroupSmtpAddress resposta de erro</span><span class="sxs-lookup"><span data-stu-id="b6c08-146">AddDistributionGroupToImList operation ErrorInvalidImDistributionGroupSmtpAddress error response</span></span>

<span data-ttu-id="b6c08-147">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **AddDistributionGroupToImList** .</span><span class="sxs-lookup"><span data-stu-id="b6c08-147">The following example shows an error response to an **AddDistributionGroupToImList** operation request.</span></span> <span data-ttu-id="b6c08-148">A seguinte resposta de erro ocorre quando é feita uma tentativa para adicionar um grupo de distribuição que não existe no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6c08-148">The following error response occurs when an attempt is made to add a distribution group that does not exist in the Exchange store.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddDistributionGroupToImListResponse ResponseClass="Error" 
                                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified IM distribution group SMTP address is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImDistributionGroupSmtpAddress</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="b6c08-149">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b6c08-149">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b6c08-150">AddDistributionGroupToImListResponse</span><span class="sxs-lookup"><span data-stu-id="b6c08-150">AddDistributionGroupToImListResponse</span></span>](adddistributiongrouptoimlistresponse.md)
    
- [<span data-ttu-id="b6c08-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="b6c08-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b6c08-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b6c08-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="b6c08-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="b6c08-153">See also</span></span>

- [<span data-ttu-id="b6c08-154">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b6c08-154">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)   
- [<span data-ttu-id="b6c08-155">AddImGroup</span><span class="sxs-lookup"><span data-stu-id="b6c08-155">AddImGroup</span></span>](addimgroup-operation.md)   
- [<span data-ttu-id="b6c08-156">RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="b6c08-156">RemoveImGroup</span></span>](removeimgroup-operation.md)
    

