---
title: Operação GetImItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 51186691-46d2-4d5c-b8bc-4ee2bb20fbe7
description: Encontre informações sobre a operação do EWS do GetImItems.
ms.openlocfilehash: 960f4683dd478b0e5f8cf18fa8d1593b7433a249
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456042"
---
# <a name="getimitems-operation"></a><span data-ttu-id="26462-103">Operação GetImItems</span><span class="sxs-lookup"><span data-stu-id="26462-103">GetImItems operation</span></span>

<span data-ttu-id="26462-104">Encontre informações sobre a operação do EWS do **GetImItems** .</span><span class="sxs-lookup"><span data-stu-id="26462-104">Find information about the **GetImItems** EWS operation.</span></span> 
  
<span data-ttu-id="26462-105">A operação **GetImItems** recupera informações sobre grupos de mensagens instantâneas (IM) e pessoas de contato de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="26462-105">The **GetImItems** operation retrieves information about instant messaging (IM) groups and IM contact personas.</span></span> 
  
<span data-ttu-id="26462-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="26462-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getimitems-operation"></a><span data-ttu-id="26462-107">Usando a operação GetImItems</span><span class="sxs-lookup"><span data-stu-id="26462-107">Using the GetImItems operation</span></span>

<span data-ttu-id="26462-108">A operação **GetImItems** aceita identificadores de item de contato e grupo e retorna um conjunto de informações sobre os grupos e contatos.</span><span class="sxs-lookup"><span data-stu-id="26462-108">The **GetImItems** operation accepts group and contact item identifiers and returns a set of information about the groups and contacts.</span></span> <span data-ttu-id="26462-109">Os conjuntos de propriedades retornados na resposta são identificados por propriedades estendidas, vários identificadores de contato, identificadores de grupo e definições de propriedades estendidas como argumentos.</span><span class="sxs-lookup"><span data-stu-id="26462-109">The property sets returned in the response are identified by extended properties, multiple contact identifiers, group identifiers, and extended property definitions as arguments.</span></span> 
  
### <a name="getimitems-operation-soap-headers"></a><span data-ttu-id="26462-110">Cabeçalhos SOAP de operação GetImItems</span><span class="sxs-lookup"><span data-stu-id="26462-110">GetImItems operation SOAP headers</span></span>

<span data-ttu-id="26462-111">A operação **GetImItems** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="26462-111">The **GetImItems** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="26462-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="26462-112">**Header name**</span></span>|<span data-ttu-id="26462-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="26462-113">**Element**</span></span>|<span data-ttu-id="26462-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="26462-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="26462-115">**Representação**</span><span class="sxs-lookup"><span data-stu-id="26462-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="26462-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="26462-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="26462-117">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="26462-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="26462-118">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="26462-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="26462-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="26462-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="26462-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="26462-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="26462-121">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="26462-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="26462-122">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="26462-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="26462-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="26462-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="26462-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="26462-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="26462-125">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="26462-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="26462-126">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="26462-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="26462-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="26462-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="26462-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="26462-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="26462-129">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="26462-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="26462-130">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="26462-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getimitems-operation-request-example-get-detailed-information-about-im-contacts-and-groups"></a><span data-ttu-id="26462-131">Exemplo de solicitação de operação GetImItems: obter informações detalhadas sobre contatos e grupos de mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="26462-131">GetImItems operation request example: Get detailed information about IM contacts and groups</span></span>

<span data-ttu-id="26462-132">O exemplo a seguir de uma solicitação de operação do **GetImItems** mostra como solicitar informações detalhadas sobre contatos e grupos de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="26462-132">The following example of a **GetImItems** operation request shows how to request detailed information about IM contacts and groups.</span></span> <span data-ttu-id="26462-133">Uma operação **GetImItems** pode solicitar um ou mais detalhes de contato ou grupo.</span><span class="sxs-lookup"><span data-stu-id="26462-133">A **GetImItems** operation can request one or more contact or group details.</span></span> <span data-ttu-id="26462-134">Você também pode usar propriedades estendidas para obter propriedades personalizadas em grupos e contatos.</span><span class="sxs-lookup"><span data-stu-id="26462-134">You can also use extended properties to get custom properties on groups and contacts.</span></span> <span data-ttu-id="26462-135">Se uma propriedade estendida solicitada não existir em um item, a resposta irá ignorar a propriedade solicitada e retornará a resposta para o conjunto de propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="26462-135">If a requested extended property does not exist on an item, the response will ignore the requested property and return the response for the default property set.</span></span> <span data-ttu-id="26462-136">Este exemplo mostra como obter o nome de exibição usando propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="26462-136">This example shows you how to get the display name by using extended properties.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="26462-137">Todos os identificadores de item e as chaves de alteração deste artigo foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="26462-137">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> <span data-ttu-id="26462-138">Observe que as chaves de alteração são ignoradas pelo serviço para esta operação.</span><span class="sxs-lookup"><span data-stu-id="26462-138">Note that change keys are ignored by the service for this operation.</span></span> 
  
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
      <m:GetImItems>
         <m:ContactIds>
            <t:ItemId Id="AAMkADEzOTExYACABmEhpSAAA=" ChangeKey="EQAAABBmNDjF"/>
         </m:ContactIds>
         <m:GroupIds>
            <t:ItemId Id="AAMkADEzOTExYjJkBY7+0EAAA=" ChangeKey="EgAAAA=="/>
         </m:GroupIds>         
         <m:ExtendedProperties>
            <t:ExtendedProperty PropertyTag="0x3001" PropertyType="String"/>
         </m:ExtendedProperties>
      </m:GetImItems>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="26462-139">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="26462-139">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="26462-140">GetImItems</span><span class="sxs-lookup"><span data-stu-id="26462-140">GetImItems</span></span>](getimitems.md)
    
- [<span data-ttu-id="26462-141">ContactIds</span><span class="sxs-lookup"><span data-stu-id="26462-141">ContactIds</span></span>](contactids.md)
    
- [<span data-ttu-id="26462-142">ItemId</span><span class="sxs-lookup"><span data-stu-id="26462-142">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="26462-143">GroupIds</span><span class="sxs-lookup"><span data-stu-id="26462-143">GroupIds</span></span>](groupids.md)
    
- [<span data-ttu-id="26462-144">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span><span class="sxs-lookup"><span data-stu-id="26462-144">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span></span>](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [<span data-ttu-id="26462-145">Extended (PathToExtendedFieldType)</span><span class="sxs-lookup"><span data-stu-id="26462-145">ExtendedProperty (PathToExtendedFieldType)</span></span>](extendedproperty-pathtoextendedfieldtype.md)
    
## <a name="successful-getimitems-operation-response"></a><span data-ttu-id="26462-146">Resposta de operação GetImItems bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="26462-146">Successful GetImItems operation response</span></span>

<span data-ttu-id="26462-147">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação do **GetImItems** para obter um contato de mensagens instantâneas e um grupo.</span><span class="sxs-lookup"><span data-stu-id="26462-147">The following example shows a successful response to a **GetImItems** request to get an IM contact and group.</span></span> <span data-ttu-id="26462-148">O nome para exibição é solicitado em uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="26462-148">The display name is requested in an extended property.</span></span> <span data-ttu-id="26462-149">Os contatos de mensagens instantâneas são retornados no formato de uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="26462-149">IM contacts are returned in the form of a persona.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetImItemsResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <ImGroup>
                  <DisplayName>Exchange SDK Team</DisplayName>
                  <GroupType>IPM.DistList.MOC.UserGroup</GroupType>
                  <ExchangeStoreId Id="AAMkADEzQrAABY7+0EAAA=" ChangeKey="EgAAAA=="/>
                  <MemberCorrelationKey>
                     <ItemId Id="AAMkADEzOTExYjeGgGqm4QrAABmEhpSAAA=" ChangeKey="EQAAAA=="/>
                  </MemberCorrelationKey>
                  <ExtendedProperties>
                     <ExtendedProperty>
                        <ExtendedFieldURI PropertyTag="0x3001" PropertyType="String"/>
                        <Value>Exchange SDK Team</Value>
                     </ExtendedProperty>
                  </ExtendedProperties>
               </ImGroup>
            </Groups>
            <Personas xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Persona>
                  <PersonaId Id="AAQkADEzOTBZImBzN5J/uHXc="/>
                  <PersonaType>Person</PersonaType>
                  <CreationTime>2012-11-07T00:10:35Z</CreationTime>
                  <DisplayName>Tony Smith</DisplayName>
                  <DisplayNameFirstLast>Tony Smith</DisplayNameFirstLast>
                  <DisplayNameLastFirst>Tony Smith</DisplayNameLastFirst>
                  <FileAs/>
                  <FileAsId>None</FileAsId>
                  <ImAddress>tsmith@contoso.com</ImAddress>
                  <RelevanceScore>2147483647</RelevanceScore>
                  <Attributions>
                     <Attribution>
                        <Id>0</Id>
                        <SourceId Id="AAMkADEzhQaoeGgGqm4QrAABmEhpSAAA=" ChangeKey="EQArAABmNDjF"/>
                        <DisplayName>Lync Contacts</DisplayName>
                        <IsWritable>false</IsWritable>
                        <IsQuickContact>true</IsQuickContact>
                        <IsHidden>false</IsHidden>
                     </Attribution>
                  </Attributions>
                  <DisplayNames>
                     <StringAttributedValue>
                        <Value>Tony Smith</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </DisplayNames>
                  <FileAsIds>
                     <StringAttributedValue>
                        <Value>None</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </FileAsIds>
                  <ImAddresses>
                     <StringAttributedValue>
                        <Value>tsmith@contoso.com</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </ImAddresses>
                  <ExtendedProperties>
                     <ExtendedPropertyAttributedValue>
                        <Value>
                           <ExtendedFieldURI PropertyTag="0x3001" PropertyType="String"/>
                           <Value>Tony Smith</Value>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </ExtendedPropertyAttributedValue>
                  </ExtendedProperties>
               </Persona>
            </Personas>
         </ImItemList>
      </GetImItemsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="26462-150">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="26462-150">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="26462-151">GetImItemsResponse</span><span class="sxs-lookup"><span data-stu-id="26462-151">GetImItemsResponse</span></span>](getimitemsresponse.md)
    
- [<span data-ttu-id="26462-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="26462-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="26462-153">Imitemlist</span><span class="sxs-lookup"><span data-stu-id="26462-153">ImItemList</span></span>](imitemlist.md)
    
- [<span data-ttu-id="26462-154">Grupos (ArrayOfImGroupType)</span><span class="sxs-lookup"><span data-stu-id="26462-154">Groups (ArrayOfImGroupType)</span></span>](groups-arrayofimgrouptype.md)
    
- [<span data-ttu-id="26462-155">Imgroup</span><span class="sxs-lookup"><span data-stu-id="26462-155">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="26462-156">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="26462-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="26462-157">GroupType</span><span class="sxs-lookup"><span data-stu-id="26462-157">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="26462-158">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="26462-158">ExchangeStoreId</span></span>](exchangestoreid.md)
    
- [<span data-ttu-id="26462-159">MemberCorrelationKey</span><span class="sxs-lookup"><span data-stu-id="26462-159">MemberCorrelationKey</span></span>](membercorrelationkey.md)
    
- [<span data-ttu-id="26462-160">ItemId</span><span class="sxs-lookup"><span data-stu-id="26462-160">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="26462-161">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span><span class="sxs-lookup"><span data-stu-id="26462-161">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span></span>](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [<span data-ttu-id="26462-162">Extended (PathToExtendedFieldType)</span><span class="sxs-lookup"><span data-stu-id="26462-162">ExtendedProperty (PathToExtendedFieldType)</span></span>](extendedproperty-pathtoextendedfieldtype.md)
    
- [<span data-ttu-id="26462-163">Personas</span><span class="sxs-lookup"><span data-stu-id="26462-163">Personas</span></span>](personas-ex15websvcsotherref.md)
    
- [<span data-ttu-id="26462-164">Personaid</span><span class="sxs-lookup"><span data-stu-id="26462-164">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="26462-165">Personatype</span><span class="sxs-lookup"><span data-stu-id="26462-165">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="26462-166">CreationTime</span><span class="sxs-lookup"><span data-stu-id="26462-166">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="26462-167">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="26462-167">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="26462-168">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="26462-168">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="26462-169">FileAs</span><span class="sxs-lookup"><span data-stu-id="26462-169">FileAs</span></span>](fileas.md)
    
- <span data-ttu-id="26462-170">[FileAsId](fileasid.md) FileAsId</span><span class="sxs-lookup"><span data-stu-id="26462-170">[FileAsId](fileasid.md) FileAsId</span></span> 
    
- [<span data-ttu-id="26462-171">IMAddress (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="26462-171">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="26462-172">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="26462-172">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="26462-173">Atribuições (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="26462-173">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="26462-174">Atribuição (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="26462-174">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="26462-175">ID (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="26462-175">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="26462-176">SourceId</span><span class="sxs-lookup"><span data-stu-id="26462-176">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="26462-177">Iswritable</span><span class="sxs-lookup"><span data-stu-id="26462-177">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="26462-178">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="26462-178">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="26462-179">IsHidden</span><span class="sxs-lookup"><span data-stu-id="26462-179">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="26462-180">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="26462-180">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="26462-181">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="26462-181">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="26462-182">Imendereços</span><span class="sxs-lookup"><span data-stu-id="26462-182">ImAddresses</span></span>](imaddresses.md)
    
- [<span data-ttu-id="26462-183">Valor (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="26462-183">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md)
    
## <a name="getimitems-operation-error-response"></a><span data-ttu-id="26462-184">Resposta de erro de operação GetImItems</span><span class="sxs-lookup"><span data-stu-id="26462-184">GetImItems operation error response</span></span>

<span data-ttu-id="26462-185">A operação **GetImItems** não valida identificadores e não retornará a resposta de erro **ErrorInvalidImContactId** ou **ErrorInvalidImGroupId** esperada se um identificador de contato ou de grupo inválido for fornecido ao serviço.</span><span class="sxs-lookup"><span data-stu-id="26462-185">The **GetImItems** operation does not validate identifiers and will not return the expected **ErrorInvalidImContactId** or **ErrorInvalidImGroupId** error response if an invalid contact or group identifier is provided to the service.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="26462-186">Confira também</span><span class="sxs-lookup"><span data-stu-id="26462-186">See also</span></span>

- [<span data-ttu-id="26462-187">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="26462-187">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="26462-188">Operação GetImItemList</span><span class="sxs-lookup"><span data-stu-id="26462-188">GetImItemList operation</span></span>](getimitemlist-operation.md)
    

