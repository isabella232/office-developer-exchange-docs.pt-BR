---
title: Operação AddImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 376acc42-2684-4596-aca1-82a4a10865c9
description: Encontre informações sobre a operação do EWS do AddImContactToGroup.
ms.openlocfilehash: a69ee0b355e78e1249383cab612a75bcda8d9e8a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458408"
---
# <a name="addimcontacttogroup-operation"></a><span data-ttu-id="50ad4-103">Operação AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="50ad4-103">AddImContactToGroup operation</span></span>

<span data-ttu-id="50ad4-104">Encontre informações sobre a operação do EWS do **AddImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="50ad4-104">Find information about the **AddImContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="50ad4-105">A operação do **AddImContactToGroup** do serviços Web do Exchange (EWS) adiciona um contato de mensagens instantâneas (IM) existente a um grupo.</span><span class="sxs-lookup"><span data-stu-id="50ad4-105">The **AddImContactToGroup** Exchange Web Services (EWS) operation adds an existing instant messaging (IM) contact to a group.</span></span> 
  
<span data-ttu-id="50ad4-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="50ad4-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addimcontacttogroup-operation"></a><span data-ttu-id="50ad4-107">Usando a operação AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="50ad4-107">Using the AddImContactToGroup operation</span></span>

<span data-ttu-id="50ad4-108">A operação **AddImContactToGroup** pode aceitar somente contatos de im.</span><span class="sxs-lookup"><span data-stu-id="50ad4-108">The **AddImContactToGroup** operation can only accept IM contacts.</span></span> <span data-ttu-id="50ad4-109">Se quiser adicionar um novo contato de mensagens instantâneas ao repositório unificado de contatos, use a operação [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="50ad4-109">If you want to add a new IM contact to the Unified Contact Store, use the [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) operation.</span></span> 
  
<span data-ttu-id="50ad4-110">A operação **AddImContactToGroup** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="50ad4-110">The **AddImContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="50ad4-111">**Tabela 1. Cabeçalhos SOAP de operação AddImContactToGroup**</span><span class="sxs-lookup"><span data-stu-id="50ad4-111">**Table 1. AddImContactToGroup operation SOAP headers**</span></span>

|<span data-ttu-id="50ad4-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="50ad4-112">**Header name**</span></span>|<span data-ttu-id="50ad4-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="50ad4-113">**Element**</span></span>|<span data-ttu-id="50ad4-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="50ad4-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="50ad4-115">**Representação**</span><span class="sxs-lookup"><span data-stu-id="50ad4-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="50ad4-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="50ad4-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="50ad4-117">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="50ad4-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="50ad4-118">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="50ad4-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="50ad4-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="50ad4-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="50ad4-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="50ad4-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="50ad4-121">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="50ad4-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="50ad4-122">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="50ad4-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="50ad4-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="50ad4-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="50ad4-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="50ad4-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="50ad4-125">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="50ad4-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="50ad4-126">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="50ad4-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="50ad4-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="50ad4-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="50ad4-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="50ad4-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="50ad4-129">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="50ad4-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="50ad4-130">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="50ad4-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addimcontacttogroup-operation-request-example-add-an-existing-im-contact-to-an-im-group"></a><span data-ttu-id="50ad4-131">Exemplo de solicitação de operação AddImContactToGroup: adicionar um contato de IM existente a um grupo de mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="50ad4-131">AddImContactToGroup operation request example: Add an existing IM contact to an IM group</span></span>

<span data-ttu-id="50ad4-132">O exemplo a seguir de uma solicitação de operação do **AddImContactToGroup** mostra como adicionar um contato de im existente um grupo de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="50ad4-132">The following example of an **AddImContactToGroup** operation request shows how to add an existing IM contact an IM group.</span></span> 
  
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
      <m:AddImContactToGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTc4Y2AA="
                      ChangeKey="EQAAABYAAABtF8oI7i"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkzzAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:AddImContactToGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="50ad4-133">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="50ad4-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="50ad4-134">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="50ad4-134">AddImContactToGroup</span></span>](addimcontacttogroup.md)
    
- [<span data-ttu-id="50ad4-135">ContactID</span><span class="sxs-lookup"><span data-stu-id="50ad4-135">ContactId</span></span>](contactid.md)
    
- [<span data-ttu-id="50ad4-136">GroupId</span><span class="sxs-lookup"><span data-stu-id="50ad4-136">GroupId</span></span>](groupid.md)
    
## <a name="successful-addimcontacttogroup-operation-response"></a><span data-ttu-id="50ad4-137">Resposta de operação AddImContactToGroup bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="50ad4-137">Successful AddImContactToGroup operation response</span></span>

<span data-ttu-id="50ad4-138">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **AddImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="50ad4-138">The following example shows a successful response to an **AddImContactToGroup** operation request.</span></span> 
  
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
      <AddImContactToGroupResponse ResponseClass="Success" 
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </AddImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="50ad4-139">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="50ad4-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="50ad4-140">AddImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="50ad4-140">AddImContactToGroupResponse</span></span>](addimcontacttogroupresponse.md)
    
- [<span data-ttu-id="50ad4-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="50ad4-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="addimcontacttogroup-operation-errorinvalidimcontactid-error-response"></a><span data-ttu-id="50ad4-142">Resposta de erro ErrorInvalidImContactId operação AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="50ad4-142">AddImContactToGroup operation ErrorInvalidImContactId error response</span></span>

<span data-ttu-id="50ad4-143">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **AddImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="50ad4-143">The following example shows an error response to an **AddImContactToGroup** operation request.</span></span> <span data-ttu-id="50ad4-144">A seguinte resposta de erro ocorre quando é feita uma tentativa de adicionar um contato que não é um contato de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="50ad4-144">The following error response occurs when an attempt is made to add a contact that is not an IM contact.</span></span> 
  
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
      <AddImContactToGroupResponse ResponseClass="Error" 
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         </AddImContactToGroupResponse>
      </s:Body>
</s:Envelope>
```

<span data-ttu-id="50ad4-145">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="50ad4-145">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="50ad4-146">AddImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="50ad4-146">AddImContactToGroupResponse</span></span>](addimcontacttogroupresponse.md)
    
- [<span data-ttu-id="50ad4-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="50ad4-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="50ad4-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="50ad4-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="50ad4-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="50ad4-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="50ad4-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="50ad4-150">See also</span></span>

- [<span data-ttu-id="50ad4-151">Operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="50ad4-151">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="50ad4-152">Operação AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="50ad4-152">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md)
    
- [<span data-ttu-id="50ad4-153">Operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="50ad4-153">SetImGroup operation</span></span>](setimgroup-operation.md)
    
- [<span data-ttu-id="50ad4-154">Operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="50ad4-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="50ad4-155">Operação GetImItemList</span><span class="sxs-lookup"><span data-stu-id="50ad4-155">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="50ad4-156">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="50ad4-156">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

