---
title: Operação AddImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 376acc42-2684-4596-aca1-82a4a10865c9
description: Encontre informações sobre o EWS AddImContactToGroup operação.
ms.openlocfilehash: 669d798b6cabc1cab1fc057a3e18c565467440f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751046"
---
# <a name="addimcontacttogroup-operation"></a><span data-ttu-id="68e92-103">Operação AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="68e92-103">AddImContactToGroup operation</span></span>

<span data-ttu-id="68e92-104">Encontre informações sobre a operação de EWS **AddImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="68e92-104">Find information about the **AddImContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="68e92-105">A operação de serviços Web do Exchange (EWS) **AddImContactToGroup** adiciona um contato existente de mensagens instantâneas (IM) a um grupo.</span><span class="sxs-lookup"><span data-stu-id="68e92-105">The **AddImContactToGroup** Exchange Web Services (EWS) operation adds an existing instant messaging (IM) contact to a group.</span></span> 
  
<span data-ttu-id="68e92-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="68e92-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addimcontacttogroup-operation"></a><span data-ttu-id="68e92-107">Usando a operação AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="68e92-107">Using the AddImContactToGroup operation</span></span>

<span data-ttu-id="68e92-108">A operação **AddImContactToGroup** só pode aceitar contatos de mensagens Instantâneas.</span><span class="sxs-lookup"><span data-stu-id="68e92-108">The **AddImContactToGroup** operation can only accept IM contacts.</span></span> <span data-ttu-id="68e92-109">Se você deseja adicionar um novo contato de mensagens Instantâneas para o repositório unificado de contatos, use a operação de [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="68e92-109">If you want to add a new IM contact to the Unified Contact Store, use the [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) operation.</span></span> 
  
<span data-ttu-id="68e92-110">A operação **AddImContactToGroup** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="68e92-110">The **AddImContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="68e92-111">**Tabela 1. Cabeçalhos SOAP AddImContactToGroup operação**</span><span class="sxs-lookup"><span data-stu-id="68e92-111">**Table 1. AddImContactToGroup operation SOAP headers**</span></span>

|<span data-ttu-id="68e92-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="68e92-112">**Header name**</span></span>|<span data-ttu-id="68e92-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="68e92-113">**Element**</span></span>|<span data-ttu-id="68e92-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="68e92-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="68e92-115">**Representação**</span><span class="sxs-lookup"><span data-stu-id="68e92-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="68e92-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="68e92-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="68e92-117">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="68e92-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="68e92-118">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="68e92-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="68e92-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="68e92-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="68e92-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="68e92-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="68e92-121">Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="68e92-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="68e92-122">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="68e92-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="68e92-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="68e92-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="68e92-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="68e92-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="68e92-125">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="68e92-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="68e92-126">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="68e92-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="68e92-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="68e92-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="68e92-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="68e92-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="68e92-129">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="68e92-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="68e92-130">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="68e92-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addimcontacttogroup-operation-request-example-add-an-existing-im-contact-to-an-im-group"></a><span data-ttu-id="68e92-131">Exemplo de solicitação de operação AddImContactToGroup: adicionar um IM existente entre em contato com a um grupo de mensagens Instantâneas</span><span class="sxs-lookup"><span data-stu-id="68e92-131">AddImContactToGroup operation request example: Add an existing IM contact to an IM group</span></span>

<span data-ttu-id="68e92-132">O exemplo a seguir de uma solicitação de operação **AddImContactToGroup** mostra como adicionar um contato de mensagens Instantâneas existente, um grupo de mensagens Instantâneas.</span><span class="sxs-lookup"><span data-stu-id="68e92-132">The following example of an **AddImContactToGroup** operation request shows how to add an existing IM contact an IM group.</span></span> 
  
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
      <m:AddImContactToGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTc4Y2AA="
                      ChangeKey="EQAAABYAAABtF8oI7i"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkzzAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:AddImContactToGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="68e92-133">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="68e92-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="68e92-134">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="68e92-134">AddImContactToGroup</span></span>](addimcontacttogroup.md)
    
- [<span data-ttu-id="68e92-135">ID de contato</span><span class="sxs-lookup"><span data-stu-id="68e92-135">ContactId</span></span>](contactid.md)
    
- [<span data-ttu-id="68e92-136">GroupId</span><span class="sxs-lookup"><span data-stu-id="68e92-136">GroupId</span></span>](groupid.md)
    
## <a name="successful-addimcontacttogroup-operation-response"></a><span data-ttu-id="68e92-137">Resposta de operação AddImContactToGroup bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="68e92-137">Successful AddImContactToGroup operation response</span></span>

<span data-ttu-id="68e92-138">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **AddImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="68e92-138">The following example shows a successful response to an **AddImContactToGroup** operation request.</span></span> 
  
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
      <AddImContactToGroupResponse ResponseClass="Success" 
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </AddImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="68e92-139">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="68e92-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="68e92-140">AddImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="68e92-140">AddImContactToGroupResponse</span></span>](addimcontacttogroupresponse.md)
    
- [<span data-ttu-id="68e92-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="68e92-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="addimcontacttogroup-operation-errorinvalidimcontactid-error-response"></a><span data-ttu-id="68e92-142">Operação AddImContactToGroup ErrorInvalidImContactId resposta de erro</span><span class="sxs-lookup"><span data-stu-id="68e92-142">AddImContactToGroup operation ErrorInvalidImContactId error response</span></span>

<span data-ttu-id="68e92-143">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **AddImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="68e92-143">The following example shows an error response to an **AddImContactToGroup** operation request.</span></span> <span data-ttu-id="68e92-144">A seguinte resposta de erro ocorre quando é feita uma tentativa para adicionar um contato que não seja um contato de mensagens Instantâneas.</span><span class="sxs-lookup"><span data-stu-id="68e92-144">The following error response occurs when an attempt is made to add a contact that is not an IM contact.</span></span> 
  
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
      <AddImContactToGroupResponse ResponseClass="Error" 
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         </AddImContactToGroupResponse>
      </s:Body>
</s:Envelope>
```

<span data-ttu-id="68e92-145">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="68e92-145">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="68e92-146">AddImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="68e92-146">AddImContactToGroupResponse</span></span>](addimcontacttogroupresponse.md)
    
- [<span data-ttu-id="68e92-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="68e92-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="68e92-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="68e92-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="68e92-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="68e92-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="68e92-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="68e92-150">See also</span></span>

- [<span data-ttu-id="68e92-151">Operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="68e92-151">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="68e92-152">Operação AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="68e92-152">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md)
    
- [<span data-ttu-id="68e92-153">Operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="68e92-153">SetImGroup operation</span></span>](setimgroup-operation.md)
    
- [<span data-ttu-id="68e92-154">Operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="68e92-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="68e92-155">Operação GetImItemList</span><span class="sxs-lookup"><span data-stu-id="68e92-155">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="68e92-156">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="68e92-156">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

