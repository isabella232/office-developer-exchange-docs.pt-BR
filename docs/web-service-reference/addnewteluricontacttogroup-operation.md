---
title: Operação AddNewTelUriContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9688ce8-2465-45bb-8bd2-94b32ed4885c
description: Encontre informações sobre como usar a operação AddNewTelUriContactToGroup EWS.
ms.openlocfilehash: 34450171776b4215d9c0a39700a309e2e2d755dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751062"
---
# <a name="addnewteluricontacttogroup-operation"></a><span data-ttu-id="838a7-103">Operação AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="838a7-103">AddNewTelUriContactToGroup operation</span></span>

<span data-ttu-id="838a7-104">Encontre informações sobre como usar a operação de EWS **AddNewTelUriContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="838a7-104">Find information about how to use the **AddNewTelUriContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="838a7-105">A operação **AddNewTelUriContactToGroup** adiciona um novo contato a um grupo com base no número de telefone do contato.</span><span class="sxs-lookup"><span data-stu-id="838a7-105">The **AddNewTelUriContactToGroup** operation adds a new contact to a group based on a contact's phone number.</span></span> 
  
<span data-ttu-id="838a7-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="838a7-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addnewteluricontacttogroup-operation"></a><span data-ttu-id="838a7-107">Usando a operação AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="838a7-107">Using the AddNewTelUriContactToGroup operation</span></span>

<span data-ttu-id="838a7-108">Uma solicitação de operação **AddNewTelUriContactToGroup** envia o URI do TEL de um contato, URI do SIP, número de telefone e o grupo para adicionar o contato.</span><span class="sxs-lookup"><span data-stu-id="838a7-108">An **AddNewTelUriContactToGroup** operation request submits a contact's TEL URI, SIP URI, phone number, and the group to add the contact to.</span></span> <span data-ttu-id="838a7-109">Uma resposta de operação **AddNewTelUriContactToGroup** cria uma pessoa para o novo contato.</span><span class="sxs-lookup"><span data-stu-id="838a7-109">An **AddNewTelUriContactToGroup** operation response creates a persona for the new contact.</span></span> <span data-ttu-id="838a7-110">Essa operação permite que os clientes adicionar um novo contato, mesmo se o contato não tem um nome.</span><span class="sxs-lookup"><span data-stu-id="838a7-110">This operation allows clients to add a new contact even if the contact does not have a name.</span></span> 
  
### <a name="addnewteluricontacttogroup-operation-soap-headers"></a><span data-ttu-id="838a7-111">Cabeçalhos SOAP AddNewTelUriContactToGroup operação</span><span class="sxs-lookup"><span data-stu-id="838a7-111">AddNewTelUriContactToGroup operation SOAP headers</span></span>

<span data-ttu-id="838a7-112">A operação **AddNewTelUriContactToGroup** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="838a7-112">The **AddNewTelUriContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="838a7-113">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="838a7-113">**Header name**</span></span>|<span data-ttu-id="838a7-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="838a7-114">**Element**</span></span>|<span data-ttu-id="838a7-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="838a7-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="838a7-116">**Representação**</span><span class="sxs-lookup"><span data-stu-id="838a7-116">**Impersonation**</span></span> <br/> |[<span data-ttu-id="838a7-117">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="838a7-117">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="838a7-118">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="838a7-118">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="838a7-119">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="838a7-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="838a7-120">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="838a7-120">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="838a7-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="838a7-121">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="838a7-122">Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="838a7-122">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="838a7-123">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="838a7-123">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="838a7-124">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="838a7-124">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="838a7-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="838a7-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="838a7-126">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="838a7-126">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="838a7-127">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="838a7-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="838a7-128">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="838a7-128">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="838a7-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="838a7-129">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="838a7-130">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="838a7-130">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="838a7-131">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="838a7-131">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addnewteluricontacttogroup-operation-request-example-add-a-new-contact-to-a-group"></a><span data-ttu-id="838a7-132">Exemplo de solicitação de operação AddNewTelUriContactToGroup: adicionar um novo contato a um grupo</span><span class="sxs-lookup"><span data-stu-id="838a7-132">AddNewTelUriContactToGroup operation request example: Add a new contact to a group</span></span>

<span data-ttu-id="838a7-133">O exemplo a seguir de uma solicitação de operação **AddNewTelUriContactToGroup** mostra como criar um novo contato e adicionar o novo contato a um grupo de (IM) de mensagens instantâneo usando TEL e os URIs do SIP do contato.</span><span class="sxs-lookup"><span data-stu-id="838a7-133">The following example of an **AddNewTelUriContactToGroup** operation request shows how to create a new contact and add the new contact to an instant messaging (IM) group by using the contact's TEL and SIP URIs.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="838a7-134">Todos os identificadores de itens e teclas de alteração neste artigo foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="838a7-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
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
      <m:AddNewTelUriContactToGroup>
         <m:TelUriAddress>tel:5625550100</m:TelUriAddress>
         <m:ImContactSipUriAddress>sip:john@contoso.com</m:ImContactSipUriAddress>
         <m:ImTelephoneNumber>5625550100</m:ImTelephoneNumber>
         <m:GroupId Id="AAMkADEzOTm4QrAABY7+0GAAA="/>
      </m:AddNewTelUriContactToGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="838a7-135">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="838a7-135">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="838a7-136">AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="838a7-136">AddNewTelUriContactToGroup</span></span>](addnewteluricontacttogroup.md)
    
- [<span data-ttu-id="838a7-137">TelUriAddress</span><span class="sxs-lookup"><span data-stu-id="838a7-137">TelUriAddress</span></span>](teluriaddress.md)
    
- [<span data-ttu-id="838a7-138">ImContactSipUriAddress</span><span class="sxs-lookup"><span data-stu-id="838a7-138">ImContactSipUriAddress</span></span>](imcontactsipuriaddress.md)
    
- [<span data-ttu-id="838a7-139">ImTelephoneNumber</span><span class="sxs-lookup"><span data-stu-id="838a7-139">ImTelephoneNumber</span></span>](imtelephonenumber.md)
    
- [<span data-ttu-id="838a7-140">GroupId</span><span class="sxs-lookup"><span data-stu-id="838a7-140">GroupId</span></span>](groupid.md)
    
## <a name="successful-addnewteluricontacttogroup-operation-response"></a><span data-ttu-id="838a7-141">Resposta de operação AddNewTelUriContactToGroup bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="838a7-141">Successful AddNewTelUriContactToGroup operation response</span></span>

<span data-ttu-id="838a7-142">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **AddNewTelUriContactToGroup** para criar um contato.</span><span class="sxs-lookup"><span data-stu-id="838a7-142">The following example shows a successful response to an **AddNewTelUriContactToGroup** operation request to create a contact.</span></span> <span data-ttu-id="838a7-143">A resposta conterá o identificador de pessoa associado para o contato, o nome de exibição da pessoa, o que nesse caso é baseada no número de telefone do contato, e o identificador de item do contato, que é exibida como parte da atribuição de identificador do código-fonte.</span><span class="sxs-lookup"><span data-stu-id="838a7-143">The response contains the associated persona identifier for the contact, the display name of the persona, which in this case is based on the contact's phone number, and the contact's item identifier, which is displayed as part of the source identifier attribution.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"                           
            xmlns:xsd="http://www.w3.org/2001/XMLSchema"
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
   </s:Header>
   <s:Body>
      <AddNewTelUriContactToGroupResponse ResponseClass="Success" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <Persona>
            <t:PersonaId Id="AAQkADE686dX3s="/>
            <t:PersonaType>Person</t:PersonaType>
            <t:CreationTime>2012-10-29T23:10:13Z</t:CreationTime>
            <t:DisplayName/>
            <t:DisplayNameFirstLast>5625550100</t:DisplayNameFirstLast>
            <t:DisplayNameLastFirst>5625550100</t:DisplayNameLastFirst>
            <t:FileAs/>
            <t:FileAsId >None</t:FileAsId>
            <t:RelevanceScore >2147483647</t:RelevanceScore>
            <t:Attributions>
               <t:Attribution>
                  <t:Id>0</t:Id>
                  <t:SourceId Id="ABhHuhCAAA=" ChangeKey="EQAAABxFU"/>
                  <t:DisplayName>Lync Contacts</t:DisplayName>
                  <t:IsWritable>false</t:IsWritable>
                  <t:IsQuickContact>true</t:IsQuickContact>
                  <t:IsHidden>false</t:IsHidden>
               </t:Attribution>
            </t:Attributions>
            <t:FileAsIds>
               <t:StringAttributedValue>
                  <t:Value>None</t:Value>
                  <t:Attributions>
                     <t:Attribution>0</t:Attribution>
                  </t:Attributions>
               </t:StringAttributedValue>
            </t:FileAsIds>
            <t:OtherTelephones>
               <t:PhoneNumberAttributedValue>
                  <t:Value>
                     <t:Number>5625550100</t:Number>
                     <t:Type>Other</t:Type>
                  </t:Value>
                  <t:Attributions>
                     <t:Attribution>0</t:Attribution>
                  </t:Attributions>
               </t:PhoneNumberAttributedValue>
            </t:OtherTelephones>
         </Persona>
      </AddNewTelUriContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="838a7-144">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="838a7-144">The response SOAP body contains following elements:</span></span>
  
- [<span data-ttu-id="838a7-145">AddNewTelUriContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="838a7-145">AddNewTelUriContactToGroupResponse</span></span>](addnewteluricontacttogroupresponse.md)
    
- [<span data-ttu-id="838a7-146">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="838a7-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="838a7-147">Pessoa</span><span class="sxs-lookup"><span data-stu-id="838a7-147">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="838a7-148">PersonaId</span><span class="sxs-lookup"><span data-stu-id="838a7-148">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="838a7-149">PersonaType</span><span class="sxs-lookup"><span data-stu-id="838a7-149">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="838a7-150">CreationTime</span><span class="sxs-lookup"><span data-stu-id="838a7-150">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="838a7-151">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="838a7-151">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="838a7-152">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="838a7-152">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="838a7-153">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="838a7-153">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="838a7-154">FileAs</span><span class="sxs-lookup"><span data-stu-id="838a7-154">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="838a7-155">FileAsId</span><span class="sxs-lookup"><span data-stu-id="838a7-155">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="838a7-156">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="838a7-156">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="838a7-157">Atribuições (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="838a7-157">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="838a7-158">Atribuição (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="838a7-158">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="838a7-159">ID (String)</span><span class="sxs-lookup"><span data-stu-id="838a7-159">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="838a7-160">SourceId</span><span class="sxs-lookup"><span data-stu-id="838a7-160">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="838a7-161">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="838a7-161">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="838a7-162">IsWritable</span><span class="sxs-lookup"><span data-stu-id="838a7-162">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="838a7-163">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="838a7-163">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="838a7-164">IsHidden</span><span class="sxs-lookup"><span data-stu-id="838a7-164">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="838a7-165">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="838a7-165">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="838a7-166">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="838a7-166">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="838a7-167">Valor</span><span class="sxs-lookup"><span data-stu-id="838a7-167">Value</span></span>](value.md)
    
- [<span data-ttu-id="838a7-168">Atribuições (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="838a7-168">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="838a7-169">Atribuição (string)</span><span class="sxs-lookup"><span data-stu-id="838a7-169">Attribution (string)</span></span>](attribution-string.md)
    
- [<span data-ttu-id="838a7-170">OtherTelephones</span><span class="sxs-lookup"><span data-stu-id="838a7-170">OtherTelephones</span></span>](othertelephones.md)
    
- [<span data-ttu-id="838a7-171">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="838a7-171">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="838a7-172">Valor</span><span class="sxs-lookup"><span data-stu-id="838a7-172">Value</span></span>](value.md)
    
- [<span data-ttu-id="838a7-173">Número</span><span class="sxs-lookup"><span data-stu-id="838a7-173">Number</span></span>](number.md)
    
- [<span data-ttu-id="838a7-174">Tipo (string)</span><span class="sxs-lookup"><span data-stu-id="838a7-174">Type (string)</span></span>](type-string.md)
    
- [<span data-ttu-id="838a7-175">Atribuições (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="838a7-175">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="838a7-176">Atribuição (string)</span><span class="sxs-lookup"><span data-stu-id="838a7-176">Attribution (string)</span></span>](attribution-string.md)
    
## <a name="addnewteluricontacttogroup-operation-error-response-example"></a><span data-ttu-id="838a7-177">Exemplo de resposta de erro de operação AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="838a7-177">AddNewTelUriContactToGroup operation error response example</span></span>

<span data-ttu-id="838a7-178">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **AddNewTelUriContactToGroup** quando o identificador do grupo contém um valor válido que não identifica um grupo na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="838a7-178">The following example shows an error response to an **AddNewTelUriContactToGroup** operation request when the group identifier contains a well-formed value that does not identify a group in the mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddNewTelUriContactToGroupResponse ResponseClass="Error" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddNewTelUriContactToGroupResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="838a7-179">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="838a7-179">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="838a7-180">AddNewTelUriContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="838a7-180">AddNewTelUriContactToGroupResponse</span></span>](addnewteluricontacttogroupresponse.md)
    
- [<span data-ttu-id="838a7-181">MessageText</span><span class="sxs-lookup"><span data-stu-id="838a7-181">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="838a7-182">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="838a7-182">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="838a7-183">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="838a7-183">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="838a7-184">Confira também</span><span class="sxs-lookup"><span data-stu-id="838a7-184">See also</span></span>

- [<span data-ttu-id="838a7-185">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="838a7-185">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="838a7-186">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="838a7-186">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

