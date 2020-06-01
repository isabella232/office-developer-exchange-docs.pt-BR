---
title: Operação AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cb5525f-faa3-48f1-9551-df55ffc26f46
description: Encontre informações sobre a operação do EWS do AddNewImContactToGroup.
ms.openlocfilehash: e91cc067b4161b366e6713a9adc16873e63b1562
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465026"
---
# <a name="addnewimcontacttogroup-operation"></a><span data-ttu-id="da201-103">Operação AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="da201-103">AddNewImContactToGroup operation</span></span>

<span data-ttu-id="da201-104">Encontre informações sobre a operação do EWS do **AddNewImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="da201-104">Find information about the **AddNewImContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="da201-105">A operação **AddNewImContactToGroup** adiciona um novo contato a um grupo de mensagens instantâneas (IM).</span><span class="sxs-lookup"><span data-stu-id="da201-105">The **AddNewImContactToGroup** operation adds a new contact to an instant messaging (IM) group.</span></span> 
  
<span data-ttu-id="da201-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="da201-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addnewimcontacttogroup-operation"></a><span data-ttu-id="da201-107">Usando a operação AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="da201-107">Using the AddNewImContactToGroup operation</span></span>

<span data-ttu-id="da201-108">A operação **AddNewImContactToGroup** aceita os três argumentos a seguir para adicionar um novo contato a um grupo de mensagens instantâneas:</span><span class="sxs-lookup"><span data-stu-id="da201-108">The **AddNewImContactToGroup** operation takes the following three arguments to add a new contact to an IM group:</span></span> 
  
- <span data-ttu-id="da201-109">Propriedade **IMAddress** – identifica o endereço de im do contato.</span><span class="sxs-lookup"><span data-stu-id="da201-109">**ImAddress** property - Identifies the contact's IM address.</span></span> <span data-ttu-id="da201-110">Essa propriedade é obrigatória.</span><span class="sxs-lookup"><span data-stu-id="da201-110">This property is required.</span></span> 
    
- <span data-ttu-id="da201-111">Propriedade **DisplayName** -identifica o nome de exibição do contato.</span><span class="sxs-lookup"><span data-stu-id="da201-111">**DisplayName** property - Identifies the contact's display name.</span></span> 
    
- <span data-ttu-id="da201-112">Propriedade **GroupId** -identifica o grupo ao qual o contato é adicionado.</span><span class="sxs-lookup"><span data-stu-id="da201-112">**GroupId** property - Identifies the group that the contact is added to.</span></span> 
    
<span data-ttu-id="da201-113">Essa operação retorna a pessoa do contato que foi adicionada ao grupo.</span><span class="sxs-lookup"><span data-stu-id="da201-113">This operation returns the persona of the contact that was added to the group.</span></span>
  
### <a name="addnewimcontacttogroup-operation-soap-headers"></a><span data-ttu-id="da201-114">Cabeçalhos SOAP de operação AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="da201-114">AddNewImContactToGroup operation SOAP headers</span></span>

<span data-ttu-id="da201-115">A operação **AddNewImContactToGroup** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="da201-115">The **AddNewImContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="da201-116">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="da201-116">**Header name**</span></span>|<span data-ttu-id="da201-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="da201-117">**Element**</span></span>|<span data-ttu-id="da201-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="da201-118">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="da201-119">**Representação**</span><span class="sxs-lookup"><span data-stu-id="da201-119">**Impersonation**</span></span> <br/> |[<span data-ttu-id="da201-120">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="da201-120">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="da201-121">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="da201-121">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="da201-122">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="da201-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="da201-123">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="da201-123">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="da201-124">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="da201-124">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="da201-125">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="da201-125">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="da201-126">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="da201-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="da201-127">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="da201-127">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="da201-128">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="da201-128">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="da201-129">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="da201-129">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="da201-130">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="da201-130">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="da201-131">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="da201-131">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="da201-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="da201-132">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="da201-133">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="da201-133">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="da201-134">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="da201-134">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addnewimcontacttogroup-operation-request-example-add-a-new-im-contact-to-a-group"></a><span data-ttu-id="da201-135">Exemplo de solicitação de operação AddNewImContactToGroup: adicionar um novo contato de mensagens instantâneas a um grupo</span><span class="sxs-lookup"><span data-stu-id="da201-135">AddNewImContactToGroup operation request example: Add a new IM contact to a group</span></span>

<span data-ttu-id="da201-136">O exemplo a seguir de uma solicitação de operação **AddNewImContactToGroup** mostra como adicionar um novo contato a um grupo de im existente.</span><span class="sxs-lookup"><span data-stu-id="da201-136">The following example of an **AddNewImContactToGroup** operation request shows how to add a new contact to an existing IM group.</span></span> <span data-ttu-id="da201-137">O valor da propriedade **GroupId** para este exemplo foi retornado dos resultados da [operação AddImGroup](addimgroup-operation.md).</span><span class="sxs-lookup"><span data-stu-id="da201-137">The **GroupId** property value for this example was returned from results of the [AddImGroup operation](addimgroup-operation.md).</span></span> <span data-ttu-id="da201-138">A propriedade **ExchangeStoreId** contém o valor da propriedade **GroupId** .</span><span class="sxs-lookup"><span data-stu-id="da201-138">The **ExchangeStoreId** property contains the **GroupId** property value.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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
> <span data-ttu-id="da201-139">O valor de **GroupId** foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="da201-139">The **GroupId** value has been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="da201-140">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="da201-140">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="da201-141">AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="da201-141">AddNewImContactToGroup</span></span>](addnewimcontacttogroup.md)
    
- [<span data-ttu-id="da201-142">IMAddress (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="da201-142">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="da201-143">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="da201-143">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="da201-144">GroupId</span><span class="sxs-lookup"><span data-stu-id="da201-144">GroupId</span></span>](groupid.md)
    
## <a name="successful-addnewimcontacttogroup-operation-response"></a><span data-ttu-id="da201-145">Resposta de operação AddNewImContactToGroup bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="da201-145">Successful AddNewImContactToGroup operation response</span></span>

<span data-ttu-id="da201-146">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **AddNewImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="da201-146">The following example shows a successful response to an **AddNewImContactToGroup** operation request.</span></span> <span data-ttu-id="da201-147">A resposta contém a pessoa do contato recém-criado.</span><span class="sxs-lookup"><span data-stu-id="da201-147">The response contains the persona of the newly created contact.</span></span> <span data-ttu-id="da201-148">O contato é adicionado à pasta Contatos rápidos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="da201-148">The contact is added to the Quick Contacts folder in Exchange.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="da201-149">Os identificadores foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="da201-149">Identifiers have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="349" 
                         MinorBuildNumber="0" 
                         Version="Exchange2013" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <AddNewImContactToGroupResponse ResponseClass="Success" 
                                    xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Persona>
        <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MTYzNGNkZmRkYQAQAJ3EkhEEXN5KufGbSYJanZk=" 
                   xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
        <PersonaType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
        <CreationTime xmlns="https://schemas.microsoft.com/exchange/services/2006/types">2012-01-05T23:06:58Z</CreationTime>
        <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayName>
        <DisplayNameFirstLast xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayNameFirstLast>
        <DisplayNameLastFirst xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayNameLastFirst>
        <FileAsId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
        <EmailAddress xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Tony Smith</Name>
          <Address>tsmith@contoso.com</Address>
          <RoutingType>SMTP</RoutingType>
        </EmailAddress>
        <EmailAddresses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <EmailAddress>
            <Name>Tony Smith</Name>
            <Address>tsmith@contoso.com</Address>
            <RoutingType>SMTP</RoutingType>
          </EmailAddress>
        </EmailAddresses>
        <ImAddress xmlns="https://schemas.microsoft.com/exchange/services/2006/types">tsmith@contoso.com</ImAddress>
        <RelevanceScore xmlns="https://schemas.microsoft.com/exchange/services/2006/types">2147483647</RelevanceScore>
        <Attributions xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
        <DisplayNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>Tony Smith</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </DisplayNames>
        <FileAsIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>None</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </FileAsIds>
        <Emails1 xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
        <ImAddresses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="da201-150">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="da201-150">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="da201-151">AddNewImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="da201-151">AddNewImContactToGroupResponse</span></span>](addnewimcontacttogroupresponse.md)
    
- [<span data-ttu-id="da201-152">Pessoal</span><span class="sxs-lookup"><span data-stu-id="da201-152">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="da201-153">Personaid</span><span class="sxs-lookup"><span data-stu-id="da201-153">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="da201-154">Personatype</span><span class="sxs-lookup"><span data-stu-id="da201-154">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="da201-155">CreationTime</span><span class="sxs-lookup"><span data-stu-id="da201-155">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="da201-156">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="da201-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="da201-157">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="da201-157">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="da201-158">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="da201-158">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="da201-159">FileAsId</span><span class="sxs-lookup"><span data-stu-id="da201-159">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="da201-160">EmailAddress (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="da201-160">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="da201-161">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="da201-161">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="da201-162">Endereço (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="da201-162">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="da201-163">RoutingType (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="da201-163">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="da201-164">IMAddress (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="da201-164">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="da201-165">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="da201-165">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="da201-166">Atribuições (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="da201-166">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="da201-167">Atribuição (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="da201-167">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="da201-168">ID (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="da201-168">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="da201-169">SourceId</span><span class="sxs-lookup"><span data-stu-id="da201-169">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="da201-170">Iswritable</span><span class="sxs-lookup"><span data-stu-id="da201-170">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="da201-171">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="da201-171">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="da201-172">IsHidden</span><span class="sxs-lookup"><span data-stu-id="da201-172">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="da201-173">FolderId</span><span class="sxs-lookup"><span data-stu-id="da201-173">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="da201-174">Displaynames</span><span class="sxs-lookup"><span data-stu-id="da201-174">DisplayNames</span></span>](displaynames.md)
    
- [<span data-ttu-id="da201-175">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="da201-175">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="da201-176">Valor (ArrayOfStringValueType)</span><span class="sxs-lookup"><span data-stu-id="da201-176">Value (ArrayOfStringValueType)</span></span>](value-arrayofstringvaluetype.md)
    
- [<span data-ttu-id="da201-177">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="da201-177">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="da201-178">Emails1</span><span class="sxs-lookup"><span data-stu-id="da201-178">Emails1</span></span>](emails1.md)
    
- [<span data-ttu-id="da201-179">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="da201-179">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
    
- [<span data-ttu-id="da201-180">Imendereços</span><span class="sxs-lookup"><span data-stu-id="da201-180">ImAddresses</span></span>](imaddresses.md)
    
## <a name="addnewimcontacttogroup-operation-error-response"></a><span data-ttu-id="da201-181">Resposta de erro de operação AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="da201-181">AddNewImContactToGroup operation error response</span></span>

<span data-ttu-id="da201-182">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **AddNewImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="da201-182">The following example shows an error response to a **AddNewImContactToGroup** operation request.</span></span> <span data-ttu-id="da201-183">Esta é uma resposta a uma solicitação para adicionar um contato a um grupo que não está na caixa de correio do solicitante.</span><span class="sxs-lookup"><span data-stu-id="da201-183">This is a response to a request to add a contact to a group that is not in the requester's mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="578" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddNewImContactToGroupResponse ResponseClass="Error" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox with such guid.</MessageText>
         <ResponseCode>ErrorNonExistentMailbox</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <MessageXml>
            <t:Value Name="MailboxGuid" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">d5fasdadcw3d-23de-2341-8f59-b71523fsddda</t:Value>
         </MessageXml>
      </AddNewImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="da201-184">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="da201-184">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="da201-185">AddNewImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="da201-185">AddNewImContactToGroupResponse</span></span>](addnewimcontacttogroupresponse.md)
    
- [<span data-ttu-id="da201-186">MessageText</span><span class="sxs-lookup"><span data-stu-id="da201-186">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="da201-187">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="da201-187">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="da201-188">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="da201-188">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="da201-189">MessageXml</span><span class="sxs-lookup"><span data-stu-id="da201-189">MessageXml</span></span>](messagexml.md)
    
<span data-ttu-id="da201-190">Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="da201-190">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="da201-191">Também consulte</span><span class="sxs-lookup"><span data-stu-id="da201-191">See also</span></span>



[<span data-ttu-id="da201-192">Operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="da201-192">AddImGroup operation</span></span>](addimgroup-operation.md)
  
[<span data-ttu-id="da201-193">Operação AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="da201-193">AddImContactToGroup operation</span></span>](addimcontacttogroup-operation.md)
  
[<span data-ttu-id="da201-194">Operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="da201-194">AddImGroup operation</span></span>](addimgroup-operation.md)
  
[<span data-ttu-id="da201-195">Operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="da201-195">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
  
[<span data-ttu-id="da201-196">Operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="da201-196">SetImGroup operation</span></span>](setimgroup-operation.md)


[<span data-ttu-id="da201-197">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="da201-197">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)

