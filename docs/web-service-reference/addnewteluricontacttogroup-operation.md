---
title: Operação AddNewTelUriContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9688ce8-2465-45bb-8bd2-94b32ed4885c
description: Encontre informações sobre como usar a operação do EWS AddNewTelUriContactToGroup.
ms.openlocfilehash: 91228ec627ad928d2f1837c135af24846f811b1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464942"
---
# <a name="addnewteluricontacttogroup-operation"></a><span data-ttu-id="b2b4a-103">Operação AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="b2b4a-103">AddNewTelUriContactToGroup operation</span></span>

<span data-ttu-id="b2b4a-104">Encontre informações sobre como usar a operação do EWS **AddNewTelUriContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="b2b4a-104">Find information about how to use the **AddNewTelUriContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="b2b4a-105">A operação **AddNewTelUriContactToGroup** adiciona um novo contato a um grupo com base no número de telefone de um contato.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-105">The **AddNewTelUriContactToGroup** operation adds a new contact to a group based on a contact's phone number.</span></span> 
  
<span data-ttu-id="b2b4a-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addnewteluricontacttogroup-operation"></a><span data-ttu-id="b2b4a-107">Usando a operação AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="b2b4a-107">Using the AddNewTelUriContactToGroup operation</span></span>

<span data-ttu-id="b2b4a-108">Uma solicitação de operação **AddNewTelUriContactToGroup** envia o URI de Tel, o URI do SIP, o número de telefone do contato e o grupo para o qual adicionar o contato.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-108">An **AddNewTelUriContactToGroup** operation request submits a contact's TEL URI, SIP URI, phone number, and the group to add the contact to.</span></span> <span data-ttu-id="b2b4a-109">Uma resposta de operação **AddNewTelUriContactToGroup** cria uma pessoa para o novo contato.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-109">An **AddNewTelUriContactToGroup** operation response creates a persona for the new contact.</span></span> <span data-ttu-id="b2b4a-110">Essa operação permite que os clientes adicionem um novo contato mesmo que o contato não tenha um nome.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-110">This operation allows clients to add a new contact even if the contact does not have a name.</span></span> 
  
### <a name="addnewteluricontacttogroup-operation-soap-headers"></a><span data-ttu-id="b2b4a-111">Cabeçalhos SOAP de operação AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="b2b4a-111">AddNewTelUriContactToGroup operation SOAP headers</span></span>

<span data-ttu-id="b2b4a-112">A operação **AddNewTelUriContactToGroup** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-112">The **AddNewTelUriContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="b2b4a-113">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="b2b4a-113">**Header name**</span></span>|<span data-ttu-id="b2b4a-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b2b4a-114">**Element**</span></span>|<span data-ttu-id="b2b4a-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b2b4a-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b2b4a-116">**Representação**</span><span class="sxs-lookup"><span data-stu-id="b2b4a-116">**Impersonation**</span></span> <br/> |[<span data-ttu-id="b2b4a-117">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="b2b4a-117">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="b2b4a-118">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-118">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="b2b4a-119">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b2b4a-120">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="b2b4a-120">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="b2b4a-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="b2b4a-121">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="b2b4a-122">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-122">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="b2b4a-123">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-123">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b2b4a-124">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="b2b4a-124">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="b2b4a-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="b2b4a-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="b2b4a-126">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-126">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="b2b4a-127">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b2b4a-128">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="b2b4a-128">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="b2b4a-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b2b4a-129">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="b2b4a-130">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-130">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="b2b4a-131">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-131">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addnewteluricontacttogroup-operation-request-example-add-a-new-contact-to-a-group"></a><span data-ttu-id="b2b4a-132">Exemplo de solicitação de operação AddNewTelUriContactToGroup: adicionar um novo contato a um grupo</span><span class="sxs-lookup"><span data-stu-id="b2b4a-132">AddNewTelUriContactToGroup operation request example: Add a new contact to a group</span></span>

<span data-ttu-id="b2b4a-133">O exemplo a seguir de uma solicitação de operação do **AddNewTelUriContactToGroup** mostra como criar um novo contato e adicionar o novo contato a um grupo de mensagens instantâneas (IM) usando os URIs Tel e SIP do contato.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-133">The following example of an **AddNewTelUriContactToGroup** operation request shows how to create a new contact and add the new contact to an instant messaging (IM) group by using the contact's TEL and SIP URIs.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b2b4a-134">Todos os identificadores de item e as chaves de alteração deste artigo foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
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
      <m:AddNewTelUriContactToGroup>
         <m:TelUriAddress>tel:5625550100</m:TelUriAddress>
         <m:ImContactSipUriAddress>sip:john@contoso.com</m:ImContactSipUriAddress>
         <m:ImTelephoneNumber>5625550100</m:ImTelephoneNumber>
         <m:GroupId Id="AAMkADEzOTm4QrAABY7+0GAAA="/>
      </m:AddNewTelUriContactToGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="b2b4a-135">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b2b4a-135">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b2b4a-136">AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="b2b4a-136">AddNewTelUriContactToGroup</span></span>](addnewteluricontacttogroup.md)
    
- [<span data-ttu-id="b2b4a-137">TelUriAddress</span><span class="sxs-lookup"><span data-stu-id="b2b4a-137">TelUriAddress</span></span>](teluriaddress.md)
    
- [<span data-ttu-id="b2b4a-138">ImContactSipUriAddress</span><span class="sxs-lookup"><span data-stu-id="b2b4a-138">ImContactSipUriAddress</span></span>](imcontactsipuriaddress.md)
    
- [<span data-ttu-id="b2b4a-139">ImTelephoneNumber</span><span class="sxs-lookup"><span data-stu-id="b2b4a-139">ImTelephoneNumber</span></span>](imtelephonenumber.md)
    
- [<span data-ttu-id="b2b4a-140">GroupId</span><span class="sxs-lookup"><span data-stu-id="b2b4a-140">GroupId</span></span>](groupid.md)
    
## <a name="successful-addnewteluricontacttogroup-operation-response"></a><span data-ttu-id="b2b4a-141">Resposta de operação AddNewTelUriContactToGroup bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="b2b4a-141">Successful AddNewTelUriContactToGroup operation response</span></span>

<span data-ttu-id="b2b4a-142">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação do **AddNewTelUriContactToGroup** para criar um contato.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-142">The following example shows a successful response to an **AddNewTelUriContactToGroup** operation request to create a contact.</span></span> <span data-ttu-id="b2b4a-143">A resposta contém o identificador persona associado para o contato, o nome de exibição da pessoa que, nesse caso, é baseado no número de telefone do contato e no identificador de item do contato, que é exibido como parte da atribuição do identificador de origem.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-143">The response contains the associated persona identifier for the contact, the display name of the persona, which in this case is based on the contact's phone number, and the contact's item identifier, which is displayed as part of the source identifier attribution.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"                           
            xmlns:xsd="http://www.w3.org/2001/XMLSchema"
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
   </s:Header>
   <s:Body>
      <AddNewTelUriContactToGroupResponse ResponseClass="Success" 
                                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="b2b4a-144">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b2b4a-144">The response SOAP body contains following elements:</span></span>
  
- [<span data-ttu-id="b2b4a-145">AddNewTelUriContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="b2b4a-145">AddNewTelUriContactToGroupResponse</span></span>](addnewteluricontacttogroupresponse.md)
    
- [<span data-ttu-id="b2b4a-146">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b2b4a-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b2b4a-147">Pessoal</span><span class="sxs-lookup"><span data-stu-id="b2b4a-147">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="b2b4a-148">Personaid</span><span class="sxs-lookup"><span data-stu-id="b2b4a-148">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="b2b4a-149">Personatype</span><span class="sxs-lookup"><span data-stu-id="b2b4a-149">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="b2b4a-150">CreationTime</span><span class="sxs-lookup"><span data-stu-id="b2b4a-150">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="b2b4a-151">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="b2b4a-151">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="b2b4a-152">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="b2b4a-152">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="b2b4a-153">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="b2b4a-153">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="b2b4a-154">FileAs</span><span class="sxs-lookup"><span data-stu-id="b2b4a-154">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="b2b4a-155">FileAsId</span><span class="sxs-lookup"><span data-stu-id="b2b4a-155">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="b2b4a-156">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="b2b4a-156">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="b2b4a-157">Atribuições (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="b2b4a-157">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="b2b4a-158">Atribuição (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="b2b4a-158">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="b2b4a-159">ID (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="b2b4a-159">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="b2b4a-160">SourceId</span><span class="sxs-lookup"><span data-stu-id="b2b4a-160">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="b2b4a-161">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="b2b4a-161">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="b2b4a-162">Iswritable</span><span class="sxs-lookup"><span data-stu-id="b2b4a-162">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="b2b4a-163">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="b2b4a-163">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="b2b4a-164">IsHidden</span><span class="sxs-lookup"><span data-stu-id="b2b4a-164">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="b2b4a-165">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="b2b4a-165">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="b2b4a-166">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="b2b4a-166">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="b2b4a-167">Valor</span><span class="sxs-lookup"><span data-stu-id="b2b4a-167">Value</span></span>](value.md)
    
- [<span data-ttu-id="b2b4a-168">Atribuições (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="b2b4a-168">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="b2b4a-169">Atribuição (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="b2b4a-169">Attribution (string)</span></span>](attribution-string.md)
    
- [<span data-ttu-id="b2b4a-170">OtherTelephones</span><span class="sxs-lookup"><span data-stu-id="b2b4a-170">OtherTelephones</span></span>](othertelephones.md)
    
- [<span data-ttu-id="b2b4a-171">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="b2b4a-171">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="b2b4a-172">Valor</span><span class="sxs-lookup"><span data-stu-id="b2b4a-172">Value</span></span>](value.md)
    
- [<span data-ttu-id="b2b4a-173">Número</span><span class="sxs-lookup"><span data-stu-id="b2b4a-173">Number</span></span>](number.md)
    
- [<span data-ttu-id="b2b4a-174">Tipo (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="b2b4a-174">Type (string)</span></span>](type-string.md)
    
- [<span data-ttu-id="b2b4a-175">Atribuições (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="b2b4a-175">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="b2b4a-176">Atribuição (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="b2b4a-176">Attribution (string)</span></span>](attribution-string.md)
    
## <a name="addnewteluricontacttogroup-operation-error-response-example"></a><span data-ttu-id="b2b4a-177">Exemplo de resposta de erro de operação AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="b2b4a-177">AddNewTelUriContactToGroup operation error response example</span></span>

<span data-ttu-id="b2b4a-178">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **AddNewTelUriContactToGroup** quando o identificador de grupo contém um valor bem-formado que não identifica um grupo na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b2b4a-178">The following example shows an error response to an **AddNewTelUriContactToGroup** operation request when the group identifier contains a well-formed value that does not identify a group in the mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddNewTelUriContactToGroupResponse ResponseClass="Error" 
                                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddNewTelUriContactToGroupResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="b2b4a-179">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b2b4a-179">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b2b4a-180">AddNewTelUriContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="b2b4a-180">AddNewTelUriContactToGroupResponse</span></span>](addnewteluricontacttogroupresponse.md)
    
- [<span data-ttu-id="b2b4a-181">MessageText</span><span class="sxs-lookup"><span data-stu-id="b2b4a-181">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b2b4a-182">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b2b4a-182">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b2b4a-183">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b2b4a-183">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="b2b4a-184">Confira também</span><span class="sxs-lookup"><span data-stu-id="b2b4a-184">See also</span></span>

- [<span data-ttu-id="b2b4a-185">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b2b4a-185">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="b2b4a-186">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b2b4a-186">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

