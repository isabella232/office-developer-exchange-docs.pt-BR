---
title: Operação AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cb5525f-faa3-48f1-9551-df55ffc26f46
description: Encontre informações sobre o EWS AddNewImContactToGroup operação.
ms.openlocfilehash: f75b89dbb6e948431d56acb9baa93fe4d4a1d939
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751061"
---
# <a name="addnewimcontacttogroup-operation"></a><span data-ttu-id="8f1da-103">Operação AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="8f1da-103">AddNewImContactToGroup operation</span></span>

<span data-ttu-id="8f1da-104">Encontre informações sobre a operação de EWS **AddNewImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="8f1da-104">Find information about the **AddNewImContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="8f1da-105">A operação **AddNewImContactToGroup** adiciona um novo contato a um grupo (IM) de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="8f1da-105">The **AddNewImContactToGroup** operation adds a new contact to an instant messaging (IM) group.</span></span> 
  
<span data-ttu-id="8f1da-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8f1da-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addnewimcontacttogroup-operation"></a><span data-ttu-id="8f1da-107">Usando a operação AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="8f1da-107">Using the AddNewImContactToGroup operation</span></span>

<span data-ttu-id="8f1da-108">A operação de **AddNewImContactToGroup** aceita os seguintes três argumentos para adicionar um novo contato a um grupo de mensagens Instantâneas:</span><span class="sxs-lookup"><span data-stu-id="8f1da-108">The **AddNewImContactToGroup** operation takes the following three arguments to add a new contact to an IM group:</span></span> 
  
- <span data-ttu-id="8f1da-109">Propriedade **ImAddress** - identifica o endereço de mensagens Instantâneas do contato.</span><span class="sxs-lookup"><span data-stu-id="8f1da-109">**ImAddress** property - Identifies the contact's IM address.</span></span> <span data-ttu-id="8f1da-110">Essa propriedade é obrigatória.</span><span class="sxs-lookup"><span data-stu-id="8f1da-110">This property is required.</span></span> 
    
- <span data-ttu-id="8f1da-111">Propriedade **DisplayName** - identifica o nome para exibição do contato.</span><span class="sxs-lookup"><span data-stu-id="8f1da-111">**DisplayName** property - Identifies the contact's display name.</span></span> 
    
- <span data-ttu-id="8f1da-112">Propriedade **GroupId** - identifica o que o contato é adicionado ao grupo.</span><span class="sxs-lookup"><span data-stu-id="8f1da-112">**GroupId** property - Identifies the group that the contact is added to.</span></span> 
    
<span data-ttu-id="8f1da-113">Essa operação retorna a pessoa do contato que foi adicionado ao grupo.</span><span class="sxs-lookup"><span data-stu-id="8f1da-113">This operation returns the persona of the contact that was added to the group.</span></span>
  
### <a name="addnewimcontacttogroup-operation-soap-headers"></a><span data-ttu-id="8f1da-114">Cabeçalhos SOAP AddNewImContactToGroup operação</span><span class="sxs-lookup"><span data-stu-id="8f1da-114">AddNewImContactToGroup operation SOAP headers</span></span>

<span data-ttu-id="8f1da-115">A operação **AddNewImContactToGroup** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="8f1da-115">The **AddNewImContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="8f1da-116">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="8f1da-116">**Header name**</span></span>|<span data-ttu-id="8f1da-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8f1da-117">**Element**</span></span>|<span data-ttu-id="8f1da-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8f1da-118">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8f1da-119">**Representação**</span><span class="sxs-lookup"><span data-stu-id="8f1da-119">**Impersonation**</span></span> <br/> |[<span data-ttu-id="8f1da-120">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="8f1da-120">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="8f1da-121">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="8f1da-121">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="8f1da-122">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f1da-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="8f1da-123">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="8f1da-123">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="8f1da-124">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="8f1da-124">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="8f1da-125">Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8f1da-125">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="8f1da-126">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f1da-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="8f1da-127">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="8f1da-127">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="8f1da-128">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="8f1da-128">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="8f1da-129">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="8f1da-129">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="8f1da-130">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f1da-130">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="8f1da-131">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="8f1da-131">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="8f1da-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="8f1da-132">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="8f1da-133">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f1da-133">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="8f1da-134">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="8f1da-134">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addnewimcontacttogroup-operation-request-example-add-a-new-im-contact-to-a-group"></a><span data-ttu-id="8f1da-135">Exemplo de solicitação de operação AddNewImContactToGroup: adicionar um novo contato de mensagem Instantânea a um grupo</span><span class="sxs-lookup"><span data-stu-id="8f1da-135">AddNewImContactToGroup operation request example: Add a new IM contact to a group</span></span>

<span data-ttu-id="8f1da-136">O exemplo a seguir de uma solicitação de operação **AddNewImContactToGroup** mostra como adicionar um novo contato a um grupo existente de mensagens Instantâneas.</span><span class="sxs-lookup"><span data-stu-id="8f1da-136">The following example of an **AddNewImContactToGroup** operation request shows how to add a new contact to an existing IM group.</span></span> <span data-ttu-id="8f1da-137">O valor da propriedade **GroupId** para que esse exemplo foi retornado de resultados da [operação AddImGroup](addimgroup-operation.md).</span><span class="sxs-lookup"><span data-stu-id="8f1da-137">The **GroupId** property value for this example was returned from results of the [AddImGroup operation](addimgroup-operation.md).</span></span> <span data-ttu-id="8f1da-138">A propriedade **ExchangeStoreId** contém o valor da propriedade **GroupId** .</span><span class="sxs-lookup"><span data-stu-id="8f1da-138">The **ExchangeStoreId** property contains the **GroupId** property value.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:AddNewImContactToGroup>
         <m:ImAddress>tsmith@contoso.com</m:ImAddress>
         <m:DisplayName>Tony Smith</m:DisplayName>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:AddNewImContactToGroup>
   </soap:Body>
</soap:Envelope>
```

> [!NOTE]
> <span data-ttu-id="8f1da-139">O valor de **GroupId** foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8f1da-139">The **GroupId** value has been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="8f1da-140">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="8f1da-140">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="8f1da-141">AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="8f1da-141">AddNewImContactToGroup</span></span>](addnewimcontacttogroup.md)
    
- [<span data-ttu-id="8f1da-142">ImAddress (String)</span><span class="sxs-lookup"><span data-stu-id="8f1da-142">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="8f1da-143">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="8f1da-143">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="8f1da-144">GroupId</span><span class="sxs-lookup"><span data-stu-id="8f1da-144">GroupId</span></span>](groupid.md)
    
## <a name="successful-addnewimcontacttogroup-operation-response"></a><span data-ttu-id="8f1da-145">Resposta de operação AddNewImContactToGroup bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="8f1da-145">Successful AddNewImContactToGroup operation response</span></span>

<span data-ttu-id="8f1da-146">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **AddNewImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="8f1da-146">The following example shows a successful response to an **AddNewImContactToGroup** operation request.</span></span> <span data-ttu-id="8f1da-147">A resposta conterá a pessoa do contato recém-criado.</span><span class="sxs-lookup"><span data-stu-id="8f1da-147">The response contains the persona of the newly created contact.</span></span> <span data-ttu-id="8f1da-148">O contato é adicionado à pasta Contatos Rápidos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="8f1da-148">The contact is added to the Quick Contacts folder in Exchange.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="8f1da-149">Identificadores foram diminuídos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8f1da-149">Identifiers have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="349" 
                         MinorBuildNumber="0" 
                         Version="Exchange2013" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <AddNewImContactToGroupResponse ResponseClass="Success" 
                                    xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Persona>
        <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MTYzNGNkZmRkYQAQAJ3EkhEEXN5KufGbSYJanZk=" 
                   xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
        <PersonaType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
        <CreationTime xmlns="http://schemas.microsoft.com/exchange/services/2006/types">2012-01-05T23:06:58Z</CreationTime>
        <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayName>
        <DisplayNameFirstLast xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayNameFirstLast>
        <DisplayNameLastFirst xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayNameLastFirst>
        <FileAsId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
        <EmailAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Tony Smith</Name>
          <Address>tsmith@contoso.com</Address>
          <RoutingType>SMTP</RoutingType>
        </EmailAddress>
        <EmailAddresses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <EmailAddress>
            <Name>Tony Smith</Name>
            <Address>tsmith@contoso.com</Address>
            <RoutingType>SMTP</RoutingType>
          </EmailAddress>
        </EmailAddresses>
        <ImAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">tsmith@contoso.com</ImAddress>
        <RelevanceScore xmlns="http://schemas.microsoft.com/exchange/services/2006/types">2147483647</RelevanceScore>
        <Attributions xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Attribution>
            <Id>0</Id>
            <SourceId Id="BtF8oI7iVOQatt/bhQoTbWAAAAAAvcAAA=" 
                      ChangeKey="EQAAABYAAABtF8oIQoTbWAAAAAAyg" />
            <DisplayName>Outlook</DisplayName>
            <IsWritable>true</IsWritable>
            <IsQuickContact>true</IsQuickContact>
            <IsHidden>false</IsHidden>
            <FolderId Id="AAMkAGQ1MjJjMTBkLTc4YhQoTbWAAAAAAvZAAA=" 
                      ChangeKey="AQAAAA==" />
          </Attribution>
        </Attributions>
        <DisplayNames xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>Tony Smith</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </DisplayNames>
        <FileAsIds xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>None</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </FileAsIds>
        <Emails1 xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <EmailAddressAttributedValue>
            <Value>
              <Name>Tony Smith</Name>
              <Address>tsmith@contoso.com</Address>
              <RoutingType>SMTP</RoutingType>
            </Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </EmailAddressAttributedValue>
        </Emails1>
        <ImAddresses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>tsmith@contoso.com</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </ImAddresses>
      </Persona>
    </AddNewImContactToGroupResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="8f1da-150">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="8f1da-150">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="8f1da-151">AddNewImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="8f1da-151">AddNewImContactToGroupResponse</span></span>](addnewimcontacttogroupresponse.md)
    
- [<span data-ttu-id="8f1da-152">Pessoa</span><span class="sxs-lookup"><span data-stu-id="8f1da-152">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="8f1da-153">PersonaId</span><span class="sxs-lookup"><span data-stu-id="8f1da-153">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="8f1da-154">PersonaType</span><span class="sxs-lookup"><span data-stu-id="8f1da-154">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="8f1da-155">CreationTime</span><span class="sxs-lookup"><span data-stu-id="8f1da-155">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="8f1da-156">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="8f1da-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="8f1da-157">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="8f1da-157">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="8f1da-158">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="8f1da-158">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="8f1da-159">FileAsId</span><span class="sxs-lookup"><span data-stu-id="8f1da-159">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="8f1da-160">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="8f1da-160">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="8f1da-161">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="8f1da-161">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="8f1da-162">Endereço (string)</span><span class="sxs-lookup"><span data-stu-id="8f1da-162">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="8f1da-163">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="8f1da-163">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="8f1da-164">ImAddress (String)</span><span class="sxs-lookup"><span data-stu-id="8f1da-164">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="8f1da-165">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="8f1da-165">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="8f1da-166">Atribuições (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="8f1da-166">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="8f1da-167">Atribuição (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="8f1da-167">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="8f1da-168">ID (String)</span><span class="sxs-lookup"><span data-stu-id="8f1da-168">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="8f1da-169">SourceId</span><span class="sxs-lookup"><span data-stu-id="8f1da-169">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="8f1da-170">IsWritable</span><span class="sxs-lookup"><span data-stu-id="8f1da-170">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="8f1da-171">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="8f1da-171">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="8f1da-172">IsHidden</span><span class="sxs-lookup"><span data-stu-id="8f1da-172">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="8f1da-173">FolderId</span><span class="sxs-lookup"><span data-stu-id="8f1da-173">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="8f1da-174">DisplayNames</span><span class="sxs-lookup"><span data-stu-id="8f1da-174">DisplayNames</span></span>](displaynames.md)
    
- [<span data-ttu-id="8f1da-175">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="8f1da-175">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="8f1da-176">Valor (ArrayOfStringValueType)</span><span class="sxs-lookup"><span data-stu-id="8f1da-176">Value (ArrayOfStringValueType)</span></span>](value-arrayofstringvaluetype.md)
    
- [<span data-ttu-id="8f1da-177">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="8f1da-177">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="8f1da-178">Emails1</span><span class="sxs-lookup"><span data-stu-id="8f1da-178">Emails1</span></span>](emails1.md)
    
- [<span data-ttu-id="8f1da-179">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="8f1da-179">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
    
- [<span data-ttu-id="8f1da-180">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="8f1da-180">ImAddresses</span></span>](imaddresses.md)
    
## <a name="addnewimcontacttogroup-operation-error-response"></a><span data-ttu-id="8f1da-181">Resposta de erro de operação AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="8f1da-181">AddNewImContactToGroup operation error response</span></span>

<span data-ttu-id="8f1da-182">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **AddNewImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="8f1da-182">The following example shows an error response to a **AddNewImContactToGroup** operation request.</span></span> <span data-ttu-id="8f1da-183">Esta é uma resposta a uma solicitação para adicionar um contato a um grupo que não esteja na caixa de correio do solicitante.</span><span class="sxs-lookup"><span data-stu-id="8f1da-183">This is a response to a request to add a contact to a group that is not in the requester's mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="578" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddNewImContactToGroupResponse ResponseClass="Error" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox with such guid.</MessageText>
         <ResponseCode>ErrorNonExistentMailbox</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <MessageXml>
            <t:Value Name="MailboxGuid" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">d5fasdadcw3d-23de-2341-8f59-b71523fsddda</t:Value>
         </MessageXml>
      </AddNewImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="8f1da-184">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="8f1da-184">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="8f1da-185">AddNewImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="8f1da-185">AddNewImContactToGroupResponse</span></span>](addnewimcontacttogroupresponse.md)
    
- [<span data-ttu-id="8f1da-186">MessageText</span><span class="sxs-lookup"><span data-stu-id="8f1da-186">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="8f1da-187">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8f1da-187">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8f1da-188">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8f1da-188">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="8f1da-189">MessageXml</span><span class="sxs-lookup"><span data-stu-id="8f1da-189">MessageXml</span></span>](messagexml.md)
    
<span data-ttu-id="8f1da-190">Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="8f1da-190">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="8f1da-191">Confira também</span><span class="sxs-lookup"><span data-stu-id="8f1da-191">See also</span></span>



[<span data-ttu-id="8f1da-192">Operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="8f1da-192">AddImGroup operation</span></span>](addimgroup-operation.md)
  
[<span data-ttu-id="8f1da-193">Operação AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="8f1da-193">AddImContactToGroup operation</span></span>](addimcontacttogroup-operation.md)
  
[<span data-ttu-id="8f1da-194">Operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="8f1da-194">AddImGroup operation</span></span>](addimgroup-operation.md)
  
[<span data-ttu-id="8f1da-195">Operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="8f1da-195">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
  
[<span data-ttu-id="8f1da-196">Operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="8f1da-196">SetImGroup operation</span></span>](setimgroup-operation.md)


[<span data-ttu-id="8f1da-197">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8f1da-197">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)

