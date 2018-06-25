---
title: Operação RemoveImContactFromGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a190bbec-c71b-4e6a-880b-55854c724d8c
description: Encontre informações sobre o EWS RemoveImContactFromGroup operação.
ms.openlocfilehash: 8c9af251014dbddabb439ed5bf5dc35580da6a90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825099"
---
# <a name="removeimcontactfromgroup-operation"></a><span data-ttu-id="82c77-103">Operação RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="82c77-103">RemoveImContactFromGroup operation</span></span>

<span data-ttu-id="82c77-104">Encontre informações sobre a operação de EWS **RemoveImContactFromGroup** .</span><span class="sxs-lookup"><span data-stu-id="82c77-104">Find information about the **RemoveImContactFromGroup** EWS operation.</span></span> 
  
<span data-ttu-id="82c77-105">A operação **RemoveImContactFromGroup** remove um único contato de mensagens Instantâneas de um grupo de mensagens Instantâneas.</span><span class="sxs-lookup"><span data-stu-id="82c77-105">The **RemoveImContactFromGroup** operation removes a single IM contact from an IM group.</span></span> 
  
<span data-ttu-id="82c77-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="82c77-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removeimcontactfromgroup-operation"></a><span data-ttu-id="82c77-107">Usando a operação RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="82c77-107">Using the RemoveImContactFromGroup operation</span></span>

<span data-ttu-id="82c77-108">A operação **RemoveImContactFromGroup** leva dois argumentos: um identificador de item de contato e o grupo (IM) do qual o contato é removido de mensagens de instantâneas correspondente.</span><span class="sxs-lookup"><span data-stu-id="82c77-108">The **RemoveImContactFromGroup** operation takes two arguments: a contact item identifier, and the corresponding instant messaging (IM) group from which the contact is removed.</span></span> 
  
### <a name="removeimcontactfromgroup-operation-soap-headers"></a><span data-ttu-id="82c77-109">Cabeçalhos SOAP RemoveImContactFromGroup operação</span><span class="sxs-lookup"><span data-stu-id="82c77-109">RemoveImContactFromGroup operation SOAP headers</span></span>

<span data-ttu-id="82c77-110">A operação **RemoveImContactFromGroup** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="82c77-110">The **RemoveImContactFromGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="82c77-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="82c77-111">**Header name**</span></span>|<span data-ttu-id="82c77-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="82c77-112">**Element**</span></span>|<span data-ttu-id="82c77-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="82c77-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="82c77-114">**Representação**</span><span class="sxs-lookup"><span data-stu-id="82c77-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="82c77-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="82c77-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="82c77-116">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="82c77-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="82c77-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="82c77-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="82c77-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="82c77-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="82c77-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="82c77-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="82c77-120">Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="82c77-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="82c77-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="82c77-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="82c77-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="82c77-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="82c77-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="82c77-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="82c77-124">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="82c77-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="82c77-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="82c77-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="82c77-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="82c77-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="82c77-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="82c77-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="82c77-128">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="82c77-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="82c77-129">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="82c77-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removeimcontactfromgroup-operation-request-example"></a><span data-ttu-id="82c77-130">Exemplo de solicitação de operação RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="82c77-130">RemoveImContactFromGroup operation request example</span></span>

<span data-ttu-id="82c77-131">O exemplo a seguir de uma solicitação de operação **RemoveImContactFromGroup** mostra como remover um contato de mensagens Instantâneas de um grupo de mensagens Instantâneas.</span><span class="sxs-lookup"><span data-stu-id="82c77-131">The following example of a **RemoveImContactFromGroup** operation request shows how to remove an IM contact from an IM group.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="82c77-132">Os identificadores de grupo e de contato foram diminuídos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="82c77-132">The group and contact identifiers have been shortened to preserve readability.</span></span> 
  
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
      <m:RemoveImContactFromGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTcAAAAvcAAA="
                      ChangeKey="EQAAABYAAABtF8oI7iVOQ"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkbWAAAAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:RemoveImContactFromGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="82c77-133">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="82c77-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="82c77-134">RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="82c77-134">RemoveImContactFromGroup</span></span>](removeimcontactfromgroup.md)
    
- [<span data-ttu-id="82c77-135">ID de contato</span><span class="sxs-lookup"><span data-stu-id="82c77-135">ContactId</span></span>](contactid.md)
    
- [<span data-ttu-id="82c77-136">GroupId</span><span class="sxs-lookup"><span data-stu-id="82c77-136">GroupId</span></span>](groupid.md)
    
## <a name="successful-removeimcontactfromgroup-operation-response"></a><span data-ttu-id="82c77-137">Resposta de operação RemoveImContactFromGroup bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="82c77-137">Successful RemoveImContactFromGroup operation response</span></span>

<span data-ttu-id="82c77-138">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **RemoveImContactFromGroup** .</span><span class="sxs-lookup"><span data-stu-id="82c77-138">The following example shows a successful response to a **RemoveImContactFromGroup** operation request.</span></span> 
  
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
      <RemoveImContactFromGroupResponse ResponseClass="Success" 
                                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveImContactFromGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="82c77-139">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="82c77-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="82c77-140">RemoveImContactFromGroupResponse</span><span class="sxs-lookup"><span data-stu-id="82c77-140">RemoveImContactFromGroupResponse</span></span>](removeimcontactfromgroupresponse.md)
    
- [<span data-ttu-id="82c77-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="82c77-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="removeimcontactfromgroup-operation-errorinvalidimcontactid-error-response"></a><span data-ttu-id="82c77-142">Operação RemoveImContactFromGroup ErrorInvalidImContactId resposta de erro</span><span class="sxs-lookup"><span data-stu-id="82c77-142">RemoveImContactFromGroup operation ErrorInvalidImContactId error response</span></span>

<span data-ttu-id="82c77-143">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **RemoveImContactFromGroup** .</span><span class="sxs-lookup"><span data-stu-id="82c77-143">The following example shows an error response to a **RemoveImContactFromGroup** operation request.</span></span> <span data-ttu-id="82c77-144">A seguinte resposta de erro ocorre quando é feita uma tentativa para remover um item de contato que não existe no grupo de mensagens Instantâneas.</span><span class="sxs-lookup"><span data-stu-id="82c77-144">The following error response occurs when an attempt is made to remove a contact item that does not exist in the IM group.</span></span> 
  
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
      <RemoveImContactFromGroupResponse ResponseClass="Error" 
                                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImContactFromGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="82c77-145">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="82c77-145">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="82c77-146">RemoveImContactFromGroupResponse</span><span class="sxs-lookup"><span data-stu-id="82c77-146">RemoveImContactFromGroupResponse</span></span>](removeimcontactfromgroupresponse.md)
    
- [<span data-ttu-id="82c77-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="82c77-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="82c77-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="82c77-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="82c77-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="82c77-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="82c77-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="82c77-150">See also</span></span>

- [<span data-ttu-id="82c77-151">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="82c77-151">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="82c77-152">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="82c77-152">AddDistributionGroupToImList</span></span>](adddistributiongrouptoimlist-operation.md)
    
- [<span data-ttu-id="82c77-153">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="82c77-153">AddImContactToGroup</span></span>](addimcontacttogroup-operation.md)
    
- [<span data-ttu-id="82c77-154">Operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="82c77-154">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="82c77-155">Operação AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="82c77-155">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md)
    
- [<span data-ttu-id="82c77-156">Operação GetImItemList</span><span class="sxs-lookup"><span data-stu-id="82c77-156">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="82c77-157">GetImItems</span><span class="sxs-lookup"><span data-stu-id="82c77-157">GetImItems</span></span>](getimitems-operation.md)
    
- [<span data-ttu-id="82c77-158">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="82c77-158">RemoveContactFromImList</span></span>](removecontactfromimlist-operation.md)
    
- [<span data-ttu-id="82c77-159">RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="82c77-159">RemoveDistributionGroupFromImList</span></span>](removedistributiongroupfromimlist-operation.md)
    
- [<span data-ttu-id="82c77-160">Operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="82c77-160">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="82c77-161">Operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="82c77-161">SetImGroup operation</span></span>](setimgroup-operation.md)
    
- [<span data-ttu-id="82c77-162">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="82c77-162">SetImListMigrationCompleted</span></span>](setimlistmigrationcompleted-operation.md)
    

