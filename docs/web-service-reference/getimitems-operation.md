---
title: Operação GetImItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 51186691-46d2-4d5c-b8bc-4ee2bb20fbe7
description: Encontre informações sobre o EWS GetImItems operação.
ms.openlocfilehash: 4335cc22b22dc5f102f2221f7fdb22a506ba026f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752527"
---
# <a name="getimitems-operation"></a><span data-ttu-id="74738-103">Operação GetImItems</span><span class="sxs-lookup"><span data-stu-id="74738-103">GetImItems operation</span></span>

<span data-ttu-id="74738-104">Encontre informações sobre a operação de EWS **GetImItems** .</span><span class="sxs-lookup"><span data-stu-id="74738-104">Find information about the **GetImItems** EWS operation.</span></span> 
  
<span data-ttu-id="74738-105">A operação **GetImItems** recupera informações sobre grupos de mensagens Instantâneas instantânea e personagens de contato de mensagens Instantâneas.</span><span class="sxs-lookup"><span data-stu-id="74738-105">The **GetImItems** operation retrieves information about instant messaging (IM) groups and IM contact personas.</span></span> 
  
<span data-ttu-id="74738-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="74738-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getimitems-operation"></a><span data-ttu-id="74738-107">Usando a operação GetImItems</span><span class="sxs-lookup"><span data-stu-id="74738-107">Using the GetImItems operation</span></span>

<span data-ttu-id="74738-108">A operação **GetImItems** aceita o grupo e contato identificadores de item e retorna um conjunto de informações sobre os grupos e contatos.</span><span class="sxs-lookup"><span data-stu-id="74738-108">The **GetImItems** operation accepts group and contact item identifiers and returns a set of information about the groups and contacts.</span></span> <span data-ttu-id="74738-109">Os conjuntos de propriedade retornados na resposta são identificados por propriedades estendidas, vários identificadores de contato, identificadores de grupo e estendidos de definições de propriedade como argumentos.</span><span class="sxs-lookup"><span data-stu-id="74738-109">The property sets returned in the response are identified by extended properties, multiple contact identifiers, group identifiers, and extended property definitions as arguments.</span></span> 
  
### <a name="getimitems-operation-soap-headers"></a><span data-ttu-id="74738-110">Cabeçalhos SOAP GetImItems operação</span><span class="sxs-lookup"><span data-stu-id="74738-110">GetImItems operation SOAP headers</span></span>

<span data-ttu-id="74738-111">A operação **GetImItems** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="74738-111">The **GetImItems** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="74738-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="74738-112">**Header name**</span></span>|<span data-ttu-id="74738-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="74738-113">**Element**</span></span>|<span data-ttu-id="74738-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="74738-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="74738-115">**Representação**</span><span class="sxs-lookup"><span data-stu-id="74738-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="74738-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="74738-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="74738-117">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="74738-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="74738-118">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="74738-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="74738-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="74738-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="74738-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="74738-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="74738-121">Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74738-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="74738-122">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="74738-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="74738-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="74738-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="74738-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="74738-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="74738-125">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="74738-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="74738-126">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="74738-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="74738-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="74738-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="74738-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="74738-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="74738-129">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="74738-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="74738-130">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="74738-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getimitems-operation-request-example-get-detailed-information-about-im-contacts-and-groups"></a><span data-ttu-id="74738-131">Exemplo de solicitação de operação GetImItems: obter informações detalhadas sobre contatos de mensagens Instantâneas e grupos</span><span class="sxs-lookup"><span data-stu-id="74738-131">GetImItems operation request example: Get detailed information about IM contacts and groups</span></span>

<span data-ttu-id="74738-132">O exemplo a seguir de uma solicitação de operação **GetImItems** mostra como solicitar informações detalhadas sobre contatos de mensagens Instantâneas e grupos.</span><span class="sxs-lookup"><span data-stu-id="74738-132">The following example of a **GetImItems** operation request shows how to request detailed information about IM contacts and groups.</span></span> <span data-ttu-id="74738-133">Uma operação de **GetImItems** pode solicitar um ou mais contatos ou detalhes de grupo.</span><span class="sxs-lookup"><span data-stu-id="74738-133">A **GetImItems** operation can request one or more contact or group details.</span></span> <span data-ttu-id="74738-134">Você também pode usar propriedades estendidas para obter as propriedades personalizadas em grupos e contatos.</span><span class="sxs-lookup"><span data-stu-id="74738-134">You can also use extended properties to get custom properties on groups and contacts.</span></span> <span data-ttu-id="74738-135">Se uma propriedade estendida solicitado não existir em um item, a resposta ignorará a propriedade solicitada e retorna a resposta para o conjunto de propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="74738-135">If a requested extended property does not exist on an item, the response will ignore the requested property and return the response for the default property set.</span></span> <span data-ttu-id="74738-136">Este exemplo mostra como obter o nome para exibição usando as propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="74738-136">This example shows you how to get the display name by using extended properties.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="74738-137">Todos os identificadores de itens e teclas de alteração neste artigo foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="74738-137">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> <span data-ttu-id="74738-138">Observe que alterar teclas são ignorados pelo serviço para essa operação.</span><span class="sxs-lookup"><span data-stu-id="74738-138">Note that change keys are ignored by the service for this operation.</span></span> 
  
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

<span data-ttu-id="74738-139">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="74738-139">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="74738-140">GetImItems</span><span class="sxs-lookup"><span data-stu-id="74738-140">GetImItems</span></span>](getimitems.md)
    
- [<span data-ttu-id="74738-141">ContactIds</span><span class="sxs-lookup"><span data-stu-id="74738-141">ContactIds</span></span>](contactids.md)
    
- [<span data-ttu-id="74738-142">ItemId</span><span class="sxs-lookup"><span data-stu-id="74738-142">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="74738-143">IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="74738-143">GroupIds</span></span>](groupids.md)
    
- [<span data-ttu-id="74738-144">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span><span class="sxs-lookup"><span data-stu-id="74738-144">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span></span>](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [<span data-ttu-id="74738-145">ExtendedProperty (PathToExtendedFieldType)</span><span class="sxs-lookup"><span data-stu-id="74738-145">ExtendedProperty (PathToExtendedFieldType)</span></span>](extendedproperty-pathtoextendedfieldtype.md)
    
## <a name="successful-getimitems-operation-response"></a><span data-ttu-id="74738-146">Resposta de operação GetImItems bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="74738-146">Successful GetImItems operation response</span></span>

<span data-ttu-id="74738-147">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de **GetImItems** para obter um contato de mensagens Instantâneas e o grupo.</span><span class="sxs-lookup"><span data-stu-id="74738-147">The following example shows a successful response to a **GetImItems** request to get an IM contact and group.</span></span> <span data-ttu-id="74738-148">O nome para exibição é solicitado em uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="74738-148">The display name is requested in an extended property.</span></span> <span data-ttu-id="74738-149">Contatos de mensagens Instantâneas são retornados na forma de uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="74738-149">IM contacts are returned in the form of a persona.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetImItemsResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
            <Personas xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="74738-150">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="74738-150">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="74738-151">GetImItemsResponse</span><span class="sxs-lookup"><span data-stu-id="74738-151">GetImItemsResponse</span></span>](getimitemsresponse.md)
    
- [<span data-ttu-id="74738-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="74738-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="74738-153">ImItemList</span><span class="sxs-lookup"><span data-stu-id="74738-153">ImItemList</span></span>](imitemlist.md)
    
- [<span data-ttu-id="74738-154">Grupos (ArrayOfImGroupType)</span><span class="sxs-lookup"><span data-stu-id="74738-154">Groups (ArrayOfImGroupType)</span></span>](groups-arrayofimgrouptype.md)
    
- [<span data-ttu-id="74738-155">ImGroup</span><span class="sxs-lookup"><span data-stu-id="74738-155">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="74738-156">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="74738-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="74738-157">GroupType</span><span class="sxs-lookup"><span data-stu-id="74738-157">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="74738-158">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="74738-158">ExchangeStoreId</span></span>](exchangestoreid.md)
    
- [<span data-ttu-id="74738-159">MemberCorrelationKey</span><span class="sxs-lookup"><span data-stu-id="74738-159">MemberCorrelationKey</span></span>](membercorrelationkey.md)
    
- [<span data-ttu-id="74738-160">ItemId</span><span class="sxs-lookup"><span data-stu-id="74738-160">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="74738-161">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span><span class="sxs-lookup"><span data-stu-id="74738-161">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span></span>](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [<span data-ttu-id="74738-162">ExtendedProperty (PathToExtendedFieldType)</span><span class="sxs-lookup"><span data-stu-id="74738-162">ExtendedProperty (PathToExtendedFieldType)</span></span>](extendedproperty-pathtoextendedfieldtype.md)
    
- [<span data-ttu-id="74738-163">Personagens</span><span class="sxs-lookup"><span data-stu-id="74738-163">Personas</span></span>](personas-ex15websvcsotherref.md)
    
- [<span data-ttu-id="74738-164">PersonaId</span><span class="sxs-lookup"><span data-stu-id="74738-164">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="74738-165">PersonaType</span><span class="sxs-lookup"><span data-stu-id="74738-165">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="74738-166">CreationTime</span><span class="sxs-lookup"><span data-stu-id="74738-166">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="74738-167">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="74738-167">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="74738-168">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="74738-168">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="74738-169">FileAs</span><span class="sxs-lookup"><span data-stu-id="74738-169">FileAs</span></span>](fileas.md)
    
- <span data-ttu-id="74738-170">[FileAsId](fileasid.md) FileAsId</span><span class="sxs-lookup"><span data-stu-id="74738-170">[FileAsId](fileasid.md) FileAsId</span></span> 
    
- [<span data-ttu-id="74738-171">ImAddress (String)</span><span class="sxs-lookup"><span data-stu-id="74738-171">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="74738-172">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="74738-172">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="74738-173">Atribuições (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="74738-173">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="74738-174">Atribuição (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="74738-174">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="74738-175">ID (String)</span><span class="sxs-lookup"><span data-stu-id="74738-175">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="74738-176">SourceId</span><span class="sxs-lookup"><span data-stu-id="74738-176">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="74738-177">IsWritable</span><span class="sxs-lookup"><span data-stu-id="74738-177">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="74738-178">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="74738-178">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="74738-179">IsHidden</span><span class="sxs-lookup"><span data-stu-id="74738-179">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="74738-180">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="74738-180">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="74738-181">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="74738-181">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="74738-182">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="74738-182">ImAddresses</span></span>](imaddresses.md)
    
- [<span data-ttu-id="74738-183">Valor (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="74738-183">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md)
    
## <a name="getimitems-operation-error-response"></a><span data-ttu-id="74738-184">Resposta de erro de operação GetImItems</span><span class="sxs-lookup"><span data-stu-id="74738-184">GetImItems operation error response</span></span>

<span data-ttu-id="74738-185">A operação **GetImItems** não valida identificadores e não retornará a resposta esperada de erro de **ErrorInvalidImContactId** ou **ErrorInvalidImGroupId** se um contato inválido ou identificador de grupo é fornecido para o serviço.</span><span class="sxs-lookup"><span data-stu-id="74738-185">The **GetImItems** operation does not validate identifiers and will not return the expected **ErrorInvalidImContactId** or **ErrorInvalidImGroupId** error response if an invalid contact or group identifier is provided to the service.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="74738-186">Confira também</span><span class="sxs-lookup"><span data-stu-id="74738-186">See also</span></span>

- [<span data-ttu-id="74738-187">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="74738-187">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="74738-188">Operação GetImItemList</span><span class="sxs-lookup"><span data-stu-id="74738-188">GetImItemList operation</span></span>](getimitemlist-operation.md)
    

