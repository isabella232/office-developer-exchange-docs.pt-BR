---
title: Operação RemoveImContactFromGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a190bbec-c71b-4e6a-880b-55854c724d8c
description: Encontre informações sobre a operação do EWS do RemoveImContactFromGroup.
ms.openlocfilehash: 4750ef57794c3da540ac36baa8ef6ef093939ea1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466966"
---
# <a name="removeimcontactfromgroup-operation"></a><span data-ttu-id="9267f-103">Operação RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="9267f-103">RemoveImContactFromGroup operation</span></span>

<span data-ttu-id="9267f-104">Encontre informações sobre a operação do EWS do **RemoveImContactFromGroup** .</span><span class="sxs-lookup"><span data-stu-id="9267f-104">Find information about the **RemoveImContactFromGroup** EWS operation.</span></span> 
  
<span data-ttu-id="9267f-105">A operação **RemoveImContactFromGroup** remove um único contato de mensagens instantâneas de um grupo de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="9267f-105">The **RemoveImContactFromGroup** operation removes a single IM contact from an IM group.</span></span> 
  
<span data-ttu-id="9267f-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9267f-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removeimcontactfromgroup-operation"></a><span data-ttu-id="9267f-107">Usando a operação RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="9267f-107">Using the RemoveImContactFromGroup operation</span></span>

<span data-ttu-id="9267f-108">A operação **RemoveImContactFromGroup** leva dois argumentos: um identificador de item de contato e o grupo de mensagens instantâneas (IM) correspondente a partir do qual o contato foi removido.</span><span class="sxs-lookup"><span data-stu-id="9267f-108">The **RemoveImContactFromGroup** operation takes two arguments: a contact item identifier, and the corresponding instant messaging (IM) group from which the contact is removed.</span></span> 
  
### <a name="removeimcontactfromgroup-operation-soap-headers"></a><span data-ttu-id="9267f-109">Cabeçalhos SOAP de operação RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="9267f-109">RemoveImContactFromGroup operation SOAP headers</span></span>

<span data-ttu-id="9267f-110">A operação **RemoveImContactFromGroup** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="9267f-110">The **RemoveImContactFromGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="9267f-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="9267f-111">**Header name**</span></span>|<span data-ttu-id="9267f-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9267f-112">**Element**</span></span>|<span data-ttu-id="9267f-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9267f-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9267f-114">**Representação**</span><span class="sxs-lookup"><span data-stu-id="9267f-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="9267f-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="9267f-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="9267f-116">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="9267f-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="9267f-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="9267f-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="9267f-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="9267f-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="9267f-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="9267f-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="9267f-120">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9267f-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="9267f-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="9267f-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="9267f-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="9267f-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="9267f-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="9267f-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="9267f-124">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="9267f-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="9267f-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="9267f-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="9267f-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="9267f-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="9267f-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="9267f-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="9267f-128">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="9267f-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="9267f-129">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="9267f-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removeimcontactfromgroup-operation-request-example"></a><span data-ttu-id="9267f-130">Exemplo de solicitação de operação RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="9267f-130">RemoveImContactFromGroup operation request example</span></span>

<span data-ttu-id="9267f-131">O exemplo a seguir de uma solicitação de operação **RemoveImContactFromGroup** mostra como remover um contato de mensagens instantâneas de um grupo de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="9267f-131">The following example of a **RemoveImContactFromGroup** operation request shows how to remove an IM contact from an IM group.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="9267f-132">Os identificadores de grupo e de contato foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9267f-132">The group and contact identifiers have been shortened to preserve readability.</span></span> 
  
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
      <m:RemoveImContactFromGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTcAAAAvcAAA="
                      ChangeKey="EQAAABYAAABtF8oI7iVOQ"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkbWAAAAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:RemoveImContactFromGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="9267f-133">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="9267f-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="9267f-134">RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="9267f-134">RemoveImContactFromGroup</span></span>](removeimcontactfromgroup.md)
    
- [<span data-ttu-id="9267f-135">ContactID</span><span class="sxs-lookup"><span data-stu-id="9267f-135">ContactId</span></span>](contactid.md)
    
- [<span data-ttu-id="9267f-136">GroupId</span><span class="sxs-lookup"><span data-stu-id="9267f-136">GroupId</span></span>](groupid.md)
    
## <a name="successful-removeimcontactfromgroup-operation-response"></a><span data-ttu-id="9267f-137">Resposta de operação RemoveImContactFromGroup bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="9267f-137">Successful RemoveImContactFromGroup operation response</span></span>

<span data-ttu-id="9267f-138">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **RemoveImContactFromGroup** .</span><span class="sxs-lookup"><span data-stu-id="9267f-138">The following example shows a successful response to a **RemoveImContactFromGroup** operation request.</span></span> 
  
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
      <RemoveImContactFromGroupResponse ResponseClass="Success" 
                                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveImContactFromGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="9267f-139">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="9267f-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="9267f-140">RemoveImContactFromGroupResponse</span><span class="sxs-lookup"><span data-stu-id="9267f-140">RemoveImContactFromGroupResponse</span></span>](removeimcontactfromgroupresponse.md)
    
- [<span data-ttu-id="9267f-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9267f-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="removeimcontactfromgroup-operation-errorinvalidimcontactid-error-response"></a><span data-ttu-id="9267f-142">Resposta de erro ErrorInvalidImContactId operação RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="9267f-142">RemoveImContactFromGroup operation ErrorInvalidImContactId error response</span></span>

<span data-ttu-id="9267f-143">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **RemoveImContactFromGroup** .</span><span class="sxs-lookup"><span data-stu-id="9267f-143">The following example shows an error response to a **RemoveImContactFromGroup** operation request.</span></span> <span data-ttu-id="9267f-144">A seguinte resposta de erro ocorre quando é feita uma tentativa de remover um item de contato que não existe no grupo de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="9267f-144">The following error response occurs when an attempt is made to remove a contact item that does not exist in the IM group.</span></span> 
  
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
      <RemoveImContactFromGroupResponse ResponseClass="Error" 
                                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImContactFromGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="9267f-145">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="9267f-145">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="9267f-146">RemoveImContactFromGroupResponse</span><span class="sxs-lookup"><span data-stu-id="9267f-146">RemoveImContactFromGroupResponse</span></span>](removeimcontactfromgroupresponse.md)
    
- [<span data-ttu-id="9267f-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="9267f-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="9267f-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9267f-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9267f-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9267f-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="9267f-150">Também consulte</span><span class="sxs-lookup"><span data-stu-id="9267f-150">See also</span></span>

- [<span data-ttu-id="9267f-151">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9267f-151">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="9267f-152">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="9267f-152">AddDistributionGroupToImList</span></span>](adddistributiongrouptoimlist-operation.md)
    
- [<span data-ttu-id="9267f-153">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="9267f-153">AddImContactToGroup</span></span>](addimcontacttogroup-operation.md)
    
- [<span data-ttu-id="9267f-154">Operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="9267f-154">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="9267f-155">Operação AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="9267f-155">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md)
    
- [<span data-ttu-id="9267f-156">Operação GetImItemList</span><span class="sxs-lookup"><span data-stu-id="9267f-156">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="9267f-157">GetImItems</span><span class="sxs-lookup"><span data-stu-id="9267f-157">GetImItems</span></span>](getimitems-operation.md)
    
- [<span data-ttu-id="9267f-158">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="9267f-158">RemoveContactFromImList</span></span>](removecontactfromimlist-operation.md)
    
- [<span data-ttu-id="9267f-159">RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="9267f-159">RemoveDistributionGroupFromImList</span></span>](removedistributiongroupfromimlist-operation.md)
    
- [<span data-ttu-id="9267f-160">Operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="9267f-160">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="9267f-161">Operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="9267f-161">SetImGroup operation</span></span>](setimgroup-operation.md)
    
- [<span data-ttu-id="9267f-162">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="9267f-162">SetImListMigrationCompleted</span></span>](setimlistmigrationcompleted-operation.md)
    

