---
title: Operação getpersona
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e2146df0-53d0-4caf-9758-b600bbc14b6a
description: Encontre informações sobre a operação do EWS GetPerson.
ms.openlocfilehash: 2b335c694a85f87c96432ea6d7c1c674613d2f17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460943"
---
# <a name="getpersona-operation"></a><span data-ttu-id="79712-103">Operação getpersona</span><span class="sxs-lookup"><span data-stu-id="79712-103">GetPersona operation</span></span>

<span data-ttu-id="79712-104">Encontre informações sobre a operação do EWS **GetPerson** .</span><span class="sxs-lookup"><span data-stu-id="79712-104">Find information about the **GetPersona** EWS operation.</span></span> 
  
<span data-ttu-id="79712-105">A operação **Getpersona** retorna um conjunto de propriedades que estão associadas a um persona.</span><span class="sxs-lookup"><span data-stu-id="79712-105">The **GetPersona** operation returns a set of properties that are associated with a persona.</span></span> 
  
<span data-ttu-id="79712-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="79712-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getpersona-operation"></a><span data-ttu-id="79712-107">Usando a operação getpersona</span><span class="sxs-lookup"><span data-stu-id="79712-107">Using the GetPersona operation</span></span>

<span data-ttu-id="79712-108">A operação **Getpersona** fornece acesso a informações de contato agregadas no formato de uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="79712-108">The **GetPersona** operation provides access to aggregated contact information in the form of a persona.</span></span> <span data-ttu-id="79712-109">O elemento [personaid](personaid.md) na solicitação identifica o persona a ser retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="79712-109">The [PersonaId](personaid.md) element in the request identifies the persona to return in the response.</span></span> <span data-ttu-id="79712-110">A resposta pode conter um conjunto padrão de propriedades persona ou um conjunto de propriedades personalizadas.</span><span class="sxs-lookup"><span data-stu-id="79712-110">The response can contain a default set of persona properties or a custom property set.</span></span> <span data-ttu-id="79712-111">Recomendamos que você especifique um conjunto de propriedades personalizadas para que as propriedades não usadas não sejam processadas e enviadas do servidor para o cliente.</span><span class="sxs-lookup"><span data-stu-id="79712-111">We recommend that you specify a custom property set so that unused properties are not processed and sent from the server to the client.</span></span> 
  
### <a name="getpersona-operation-soap-headers"></a><span data-ttu-id="79712-112">Cabeçalhos SOAP de operação getpersona</span><span class="sxs-lookup"><span data-stu-id="79712-112">GetPersona operation SOAP headers</span></span>

<span data-ttu-id="79712-113">A operação **Getpersona** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="79712-113">The **GetPersona** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="79712-114">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="79712-114">**Header name**</span></span>|<span data-ttu-id="79712-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="79712-115">**Element**</span></span>|<span data-ttu-id="79712-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="79712-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="79712-117">**Representação**</span><span class="sxs-lookup"><span data-stu-id="79712-117">**Impersonation**</span></span> <br/> |[<span data-ttu-id="79712-118">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="79712-118">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="79712-119">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="79712-119">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="79712-120">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="79712-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="79712-121">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="79712-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="79712-122">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="79712-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="79712-123">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="79712-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="79712-124">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="79712-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="79712-125">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="79712-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="79712-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="79712-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="79712-127">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="79712-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="79712-128">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="79712-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getpersona-operation-request-example-return-a-default-set-of-properties-for-a-persona"></a><span data-ttu-id="79712-129">Exemplo de solicitação de operação getpersona: retornar um conjunto padrão de propriedades de um persona</span><span class="sxs-lookup"><span data-stu-id="79712-129">GetPersona operation request example: Return a default set of properties for a persona</span></span>

<span data-ttu-id="79712-130">O exemplo a seguir de uma solicitação de operação **Getpersona** mostra como retornar um conjunto padrão de propriedades que estão associadas a um persona.</span><span class="sxs-lookup"><span data-stu-id="79712-130">The following example of a **GetPersona** operation request shows how to return a default set of properties that are associated with a persona.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GetPersona>
         <PersonaId Id="AAQkADEzAQAKtOtR/l4MlLqHWORfhSYKU="/>
      </GetPersona>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="79712-131">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="79712-131">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="79712-132">Getpersona</span><span class="sxs-lookup"><span data-stu-id="79712-132">GetPersona</span></span>](getpersona.md)
    
- [<span data-ttu-id="79712-133">Personaid</span><span class="sxs-lookup"><span data-stu-id="79712-133">PersonaId</span></span>](personaid.md)
    
## <a name="successful-getpersona-operation-response"></a><span data-ttu-id="79712-134">Resposta de operação getpersona bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="79712-134">Successful GetPersona operation response</span></span>

<span data-ttu-id="79712-135">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="79712-135">The following example shows a successful response to a **GetPersona** operation request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="79712-136">Todos os identificadores de item e as chaves de alteração deste artigo foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="79712-136">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="432" 
                           MinorBuildNumber="5" 
                           Version="Exchange2013"
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetPersonaResponseMessage ResponseClass="Success"
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <Persona>
            <PersonaId Id="AAQkADEzAQAKtOtR="
              xmlns="https://schemas.microsoft.com/exchange/services/2006/types"/>
            <PersonaType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
            <CreationTime xmlns="https://schemas.microsoft.com/exchange/services/2006/types">2012-06-01T17:00:34Z</CreationTime>
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayName>
            <DisplayNameFirstLast xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayNameFirstLast>
            <DisplayNameLastFirst xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnson Brian</DisplayNameLastFirst>
            <FileAs xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnson, Brian</FileAs>
            <FileAsId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
            <GivenName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian</GivenName>
            <Surname xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnsoon</Surname>
            <CompanyName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Contoso</CompanyName>
            <RelevanceScore xmlns="https://schemas.microsoft.com/exchange/services/2006/types">4255550110</RelevanceScore>
            <Attributions xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Attribution>
                  <Id>0</Id>
                  <SourceId Id="AAMkA =" ChangeKey="EQAAABY+"/>
                  <DisplayName>Outlook</DisplayName>
                  <IsWritable>true</IsWritable>
                  <IsQuickContact>false</IsQuickContact>
                  <IsHidden>false</IsHidden>
                  <FolderId Id="AAMkA=" ChangeKey="AQAAAA=="/>
               </Attribution>
            </Attributions>
            <DisplayNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </DisplayNames>
            <FileAses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson, Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAses>
            <FileAsIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>None</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAsIds>
            <GivenNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </GivenNames>
            <Surnames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </Surnames>
            <MobilePhones xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <PhoneNumberAttributedValue>
                  <Value>
                     <Number>(425)555-0110</Number>
                     <Type>Mobile</Type>
                  </Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </PhoneNumberAttributedValue>
            </MobilePhones>
            <CompanyNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Contoso</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </CompanyNames>
         </Persona>
      </GetPersonaResponseMessage>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="79712-137">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="79712-137">The response SOAP body contains the following elements:</span></span>
  
- <span data-ttu-id="79712-138">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="79712-138">GetPersonaResponseMessage</span></span>
    
- [<span data-ttu-id="79712-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="79712-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="79712-140">Pessoal</span><span class="sxs-lookup"><span data-stu-id="79712-140">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="79712-141">Personaid</span><span class="sxs-lookup"><span data-stu-id="79712-141">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="79712-142">Personatype</span><span class="sxs-lookup"><span data-stu-id="79712-142">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="79712-143">CreationTime</span><span class="sxs-lookup"><span data-stu-id="79712-143">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="79712-144">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="79712-144">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="79712-145">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="79712-145">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="79712-146">FileAs</span><span class="sxs-lookup"><span data-stu-id="79712-146">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="79712-147">FileAsId</span><span class="sxs-lookup"><span data-stu-id="79712-147">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="79712-148">GivenName</span><span class="sxs-lookup"><span data-stu-id="79712-148">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="79712-149">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="79712-149">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="79712-150">CompanyName</span><span class="sxs-lookup"><span data-stu-id="79712-150">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="79712-151">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="79712-151">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="79712-152">Atribuições (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="79712-152">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="79712-153">Atribuição (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="79712-153">Attribution (string)</span></span>](attribution-string.md)
    
- [<span data-ttu-id="79712-154">ID (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="79712-154">ID (String)</span></span>](id-string.md)
    
- <span data-ttu-id="79712-155">[SourceID](sourceid.md) SourceId</span><span class="sxs-lookup"><span data-stu-id="79712-155">[SourceId](sourceid.md) SourceId</span></span> 
    
- [<span data-ttu-id="79712-156">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="79712-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="79712-157">Iswritable</span><span class="sxs-lookup"><span data-stu-id="79712-157">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="79712-158">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="79712-158">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="79712-159">IsHidden</span><span class="sxs-lookup"><span data-stu-id="79712-159">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="79712-160">FolderId</span><span class="sxs-lookup"><span data-stu-id="79712-160">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="79712-161">Displaynames</span><span class="sxs-lookup"><span data-stu-id="79712-161">DisplayNames</span></span>](displaynames.md)
    
- [<span data-ttu-id="79712-162">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="79712-162">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="79712-163">Valor (ArrayOfStringValueType)</span><span class="sxs-lookup"><span data-stu-id="79712-163">Value (ArrayOfStringValueType)</span></span>](value-arrayofstringvaluetype.md)
    
- [<span data-ttu-id="79712-164">Atribuições (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="79712-164">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="79712-165">Atribuição (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="79712-165">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="79712-166">FileAses</span><span class="sxs-lookup"><span data-stu-id="79712-166">FileAses</span></span>](fileases.md)
    
- [<span data-ttu-id="79712-167">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="79712-167">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="79712-168">Dados fornecidos</span><span class="sxs-lookup"><span data-stu-id="79712-168">GivenNames</span></span>](givennames.md)
    
- [<span data-ttu-id="79712-169">Sobrenomes</span><span class="sxs-lookup"><span data-stu-id="79712-169">Surnames</span></span>](surnames.md)
    
- [<span data-ttu-id="79712-170">MobilePhones</span><span class="sxs-lookup"><span data-stu-id="79712-170">MobilePhones</span></span>](mobilephones.md)
    
- [<span data-ttu-id="79712-171">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="79712-171">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="79712-172">Valor (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="79712-172">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md)
    
- [<span data-ttu-id="79712-173">Número</span><span class="sxs-lookup"><span data-stu-id="79712-173">Number</span></span>](number.md)
    
- [<span data-ttu-id="79712-174">Tipo (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="79712-174">Type (string)</span></span>](type-string.md)
    
- [<span data-ttu-id="79712-175">CompanyNames</span><span class="sxs-lookup"><span data-stu-id="79712-175">CompanyNames</span></span>](companynames.md)
    
## <a name="getpersona-operation-error-response"></a><span data-ttu-id="79712-176">Resposta de erro de operação getpersona</span><span class="sxs-lookup"><span data-stu-id="79712-176">GetPersona operation error response</span></span>

<span data-ttu-id="79712-177">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="79712-177">The following example shows an error response to a **GetPersona** operation request.</span></span> <span data-ttu-id="79712-178">Esta é uma resposta a uma solicitação que contém um identificador persona especificado incorretamente.</span><span class="sxs-lookup"><span data-stu-id="79712-178">This is a response to a request that contains an incorrectly specified persona identifier.</span></span> 
  
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
      <GetPersonaResponseMessage ResponseClass="Error" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetPersonaResponseMessage>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="79712-179">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="79712-179">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="79712-180">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="79712-180">GetPersonaResponseMessage</span></span>](getpersonaresponsemessage.md)
    
- [<span data-ttu-id="79712-181">MessageText</span><span class="sxs-lookup"><span data-stu-id="79712-181">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="79712-182">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="79712-182">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="79712-183">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="79712-183">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="79712-184">Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="79712-184">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="79712-185">Também consulte</span><span class="sxs-lookup"><span data-stu-id="79712-185">See also</span></span>

- [<span data-ttu-id="79712-186">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="79712-186">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="79712-187">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="79712-187">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="79712-188">Operação FindPeople</span><span class="sxs-lookup"><span data-stu-id="79712-188">FindPeople operation</span></span>](findpeople-operation.md)
    

