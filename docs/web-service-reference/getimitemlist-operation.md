---
title: Operação GetImItemList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e31d14e1-0c1f-4b69-98b7-157d59c13698
description: Encontre informações sobre o EWS GetImItemList operação.
ms.openlocfilehash: 3977b0ad31e819cd973ce261ba3152b3840003b3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752526"
---
# <a name="getimitemlist-operation"></a><span data-ttu-id="c30d0-103">Operação GetImItemList</span><span class="sxs-lookup"><span data-stu-id="c30d0-103">GetImItemList operation</span></span>

<span data-ttu-id="c30d0-104">Encontre informações sobre a operação de EWS **GetImItemList** .</span><span class="sxs-lookup"><span data-stu-id="c30d0-104">Find information about the **GetImItemList** EWS operation.</span></span> 
  
## <a name="using-the-getimitemlist-operation"></a><span data-ttu-id="c30d0-105">Usando a operação GetImItemList</span><span class="sxs-lookup"><span data-stu-id="c30d0-105">Using the GetImItemList operation</span></span>

<span data-ttu-id="c30d0-106">A operação **GetImItemList** recupera a lista de grupos de mensagens instantâneas e mensagens Instantâneas entre em contato com personagens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c30d0-106">The **GetImItemList** operation retrieves the list of instant messaging (IM) groups and IM contact personas in a mailbox.</span></span> <span data-ttu-id="c30d0-107">A operação **GetImItemList** não usa argumentos.</span><span class="sxs-lookup"><span data-stu-id="c30d0-107">The **GetImItemList** operation does not take any arguments.</span></span> 
  
<span data-ttu-id="c30d0-108">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c30d0-108">This operation was introduced in Exchange Server 2013.</span></span>
  
### <a name="getimitemlist-operation-soap-headers"></a><span data-ttu-id="c30d0-109">Cabeçalhos SOAP GetImItemList operação</span><span class="sxs-lookup"><span data-stu-id="c30d0-109">GetImItemList operation SOAP headers</span></span>

<span data-ttu-id="c30d0-110">A operação **GetImItemList** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="c30d0-110">The **GetImItemList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="c30d0-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="c30d0-111">**Header name**</span></span>|<span data-ttu-id="c30d0-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c30d0-112">**Element**</span></span>|<span data-ttu-id="c30d0-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c30d0-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c30d0-114">**Representação**</span><span class="sxs-lookup"><span data-stu-id="c30d0-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="c30d0-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="c30d0-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="c30d0-116">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="c30d0-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="c30d0-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c30d0-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c30d0-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="c30d0-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="c30d0-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="c30d0-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="c30d0-120">Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c30d0-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="c30d0-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c30d0-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c30d0-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="c30d0-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="c30d0-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="c30d0-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="c30d0-124">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="c30d0-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="c30d0-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c30d0-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c30d0-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="c30d0-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="c30d0-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c30d0-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="c30d0-128">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="c30d0-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="c30d0-129">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="c30d0-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getimitemlist-operation-request-example-request-your-im-items-list"></a><span data-ttu-id="c30d0-130">Exemplo de solicitação de operação GetImItemList: solicitar sua lista de itens de mensagens Instantâneas</span><span class="sxs-lookup"><span data-stu-id="c30d0-130">GetImItemList operation request example: Request your IM items list</span></span>

<span data-ttu-id="c30d0-131">O exemplo a seguir de uma solicitação de operação **GetImItemList** mostra como solicitar a lista de grupos de mensagens Instantâneas e mensagens Instantâneas entre em contato com personagens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c30d0-131">The following example of a **GetImItemList** operation request shows how to request the list of IM groups and IM contact personas in a mailbox.</span></span> <span data-ttu-id="c30d0-132">O elemento **GetImItemList** é a opção de único elemento no corpo SOAP.</span><span class="sxs-lookup"><span data-stu-id="c30d0-132">The **GetImItemList** element is the only element option in the SOAP body.</span></span> 
  
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
      <m:GetImItemList/>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="c30d0-133">A solicitação de corpo SOAP contém o elemento a seguir:</span><span class="sxs-lookup"><span data-stu-id="c30d0-133">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="c30d0-134">GetImItemList</span><span class="sxs-lookup"><span data-stu-id="c30d0-134">GetImItemList</span></span>](getimitemlist.md)
    
## <a name="successful-getimitemlist-operation-response"></a><span data-ttu-id="c30d0-135">Resposta de operação GetImItemList bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="c30d0-135">Successful GetImItemList operation response</span></span>

<span data-ttu-id="c30d0-136">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetImItemList** .</span><span class="sxs-lookup"><span data-stu-id="c30d0-136">The following example shows a successful response to a **GetImItemList** operation request.</span></span> <span data-ttu-id="c30d0-137">A resposta conterá quatro grupos de mensagens Instantâneas.</span><span class="sxs-lookup"><span data-stu-id="c30d0-137">The response contains four IM groups.</span></span> <span data-ttu-id="c30d0-138">Três dos grupos a IM — outros contatos, marcada e favoritos — são grupos padrão no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c30d0-138">Three of the IM groups — Other Contacts, Tagged, and Favorites — are default groups in the Exchange store.</span></span> <span data-ttu-id="c30d0-139">O grupo de MyCustomGroup2 é um grupo personalizado de criado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="c30d0-139">The MyCustomGroup2 group is a custom user-created group.</span></span> <span data-ttu-id="c30d0-140">Os grupos outros contatos e marcada não têm membros.</span><span class="sxs-lookup"><span data-stu-id="c30d0-140">The Other Contacts and Tagged groups do not have members.</span></span> <span data-ttu-id="c30d0-141">O grupo de favoritos tem um único membro de contato.</span><span class="sxs-lookup"><span data-stu-id="c30d0-141">The Favorites group has a single contact member.</span></span> <span data-ttu-id="c30d0-142">O MyCustomGroup2 tem dois contatos do membro.</span><span class="sxs-lookup"><span data-stu-id="c30d0-142">The MyCustomGroup2 has two member contacts.</span></span> <span data-ttu-id="c30d0-143">Os identificadores de item são fornecidos para que as solicitações de **GetItem** subsequentes podem ser executadas para obter mais informações sobre os contatos de mensagens Instantâneas.</span><span class="sxs-lookup"><span data-stu-id="c30d0-143">The item identifiers are provided so that subsequent **GetItem** requests can be performed to get more information about the IM contacts.</span></span> 
  
<span data-ttu-id="c30d0-144">Este exemplo retorna dois personagens.</span><span class="sxs-lookup"><span data-stu-id="c30d0-144">This example returns two personas.</span></span> <span data-ttu-id="c30d0-145">A primeira pessoa representa dois itens de contato: Anthony Smith e Tony Smith.</span><span class="sxs-lookup"><span data-stu-id="c30d0-145">The first persona represents two contact items: Anthony Smith and Tony Smith.</span></span> <span data-ttu-id="c30d0-146">As informações de contato combinadas são retornadas no objeto **pessoa** .</span><span class="sxs-lookup"><span data-stu-id="c30d0-146">The combined contact information is returned in the **Persona** object.</span></span> <span data-ttu-id="c30d0-147">A segunda pessoa representa um único contato com o nome de exibição do Terence Adams.</span><span class="sxs-lookup"><span data-stu-id="c30d0-147">The second persona represents a single contact with the display name of Terence Adams.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="c30d0-148">Os identificadores de repositório do Exchange, identificadores de item, identificadores de origem, identificadores de pasta e identificadores de pessoa tem sido reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c30d0-148">The Exchange store identifiers, item identifiers, source identifiers, folder identifiers, and persona identifiers have been shortened to preserve readability.</span></span> 
  
```XML
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
      <GetImItemListResponse ResponseClass="Success" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <ImGroup>
                  <DisplayName>Other Contacts</DisplayName>
                  <GroupType>IPM.DistList.MOC.OtherContacts</GroupType>
                  <ExchangeStoreId Id="AAMkAGQ1MjJjMTBkLThQoTbWAAAAAAQUAAA=" 
                                   ChangeKey="EgAAAA==" />
               </ImGroup>
               <ImGroup>
                  <DisplayName>Tagged</DisplayName>
                  <GroupType>IPM.DistList.MOC.Tagged</GroupType>
                  <ExchangeStoreId Id="AAMkAGQ1MjJAAQTAAA=" 
                                   ChangeKey="EgAAAA==" />
               </ImGroup>
               <ImGroup>
                  <DisplayName>Favorites</DisplayName>
                  <GroupType>IPM.DistList.MOC.Favorites</GroupType>
                  <ExchangeStoreId Id="AAMkAGQ1MjJjMTAAAAAQSAAA=" 
                                   ChangeKey="EgAAAA==" />
                  <MemberCorrelationKey>
                     <ItemId Id="AAMkAGQ1MjJtt/bhQoTbWAAAAAAvcAAA=" 
                             ChangeKey="EQAAAA==" />
                  </MemberCorrelationKey>
               </ImGroup>
               <ImGroup>
                  <DisplayName>MyCustomGroup2</DisplayName>
                  <GroupType>IPM.DistList.MOC.UserGroup</GroupType>
                  <ExchangeStoreId Id="AAMkAGQ1MjJjKAAA=" 
                                   ChangeKey="EgAAAA==" />
                  <MemberCorrelationKey>
                     <ItemId Id="AAMkAGQ1Matt/bhQoTbWAAAAAAvcAAA=" 
                             ChangeKey="EQAAAA==" />
                     <ItemId Id="AAMkAGQ1MjJjMTBkTbWAAAAAAveAAA=" 
                             ChangeKey="EQAAAA==" />
                  </MemberCorrelationKey>
               </ImGroup>
            </Groups>
            <Personas xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Persona>
                  <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4YkZmRkYQAQAFgxE1nBcqRGgYWWorM9/+s=" />
                  <PersonaType>Person</PersonaType>
                  <CreationTime>2012-01-12T22:14:36Z</CreationTime>
                  <DisplayName>Anthony Smith</DisplayName>
                  <DisplayNameFirstLast>Anthony Smith</DisplayNameFirstLast>
                  <DisplayNameLastFirst>Smith Anthony</DisplayNameLastFirst>
                  <FileAs>Smith, Anthony</FileAs>
                  <FileAsId>LastCommaFirst</FileAsId>
                  <GivenName>Anthony</GivenName>
                  <Surname>Smith</Surname>
                  <EmailAddress>
                     <Name>tsmith@contoso.com</Name>
                     <EmailAddress>tsmith@contoso.com</EmailAddress>
                     <RoutingType>SMTP</RoutingType>
                  </EmailAddress>
                  <EmailAddresses>
                     <EmailAddress>
                        <Name>tsmith@contoso.com</Name>
                        <EmailAddress>tsmith@contoso.com</EmailAddress>
                        <RoutingType>SMTP</RoutingType>
                     </EmailAddress>
                  </EmailAddresses>
                  <ImAddress>tsmith@contoso.com</ImAddress>
                  <RelevanceScore>2147483647</RelevanceScore>
                  <Attributions>
                     <Attribution>
                        <Id>0</Id>
                        <SourceId Id="AQMkAGQ1MjIAYzEwZC03OGNlLTQ5Bq239uFChNtYAAAIvDAAAAA==" 
                                  ChangeKey="EQAAABYAAABtF8oI7iVOQatt/bhQoTbWAAAAADB3" />
                        <DisplayName>Outlook</DisplayName>
                        <IsWritable>true</IsWritable>
                        <IsQuickContact>false</IsQuickContact>
                        <IsHidden>false</IsHidden>
                        <FolderId Id="AQMkAGQ1MjIAYzEMikE3AQBtF8oI7iVOQatt/bhQoTbWAAADEAAAAA==" 
                                  ChangeKey="AQAAAA==" />
                     </Attribution>
                     <Attribution>
                        <Id>1</Id>
                        <SourceId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04/bhQoTbWAAAAAAveAAA=" 
                                  ChangeKey="EQAAABYAAABtF8oI7iVOQatt/bhQoTbWAAAAAAym" />
                        <DisplayName>Outlook</DisplayName>
                        <IsWritable>true</IsWritable>
                        <IsQuickContact>true</IsQuickContact>
                        <IsHidden>false</IsHidden>
                        <FolderId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Qatt/bhQoTbWAAAAAAvZAAA=" 
                                  ChangeKey="AQAAAA==" />
                     </Attribution>
                  </Attributions>
                  <DisplayNames>
                     <StringAttributedValue>
                        <Value>Anthony Smith</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                     <StringAttributedValue>
                        <Value>Tony Smith</Value>
                        <Attributions>
                           <Attribution>1</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </DisplayNames>
                  <FileAses>
                     <StringAttributedValue>
                        <Value>Smith, Anthony</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </FileAses>
                  <FileAsIds>
                     <StringAttributedValue>
                        <Value>LastCommaFirst</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                     <StringAttributedValue>
                        <Value>None</Value>
                        <Attributions>
                           <Attribution>1</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </FileAsIds>
                  <GivenNames>
                     <StringAttributedValue>
                        <Value>Anthony</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </GivenNames>
                  <Surnames>
                     <StringAttributedValue>
                        <Value>Smith</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </Surnames>
                  <HomePhones>
                     <PhoneNumberAttributedValue>
                        <Value>
                           <Number>4255550110</Number>
                           <Type>Home</Type>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </PhoneNumberAttributedValue>
                  </HomePhones>
                  <MobilePhones>
                     <PhoneNumberAttributedValue>
                        <Value>
                           <Number>4255550120</Number>
                           <Type>Mobile</Type>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </PhoneNumberAttributedValue>
                  </MobilePhones>
                  <Emails1>
                     <EmailAddressAttributedValue>
                        <Value>
                           <Name>tsmith@contoso.com</Name>
                           <EmailAddress>tsmith@contoso.com</EmailAddress>
                           <RoutingType>SMTP</RoutingType>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                           <Attribution>1</Attribution>
                        </Attributions>
                     </EmailAddressAttributedValue>
                  </Emails1>
                  <ImAddresses>
                     <StringAttributedValue>
                        <Value>tsmith@contoso.com</Value>
                        <Attributions>
                           <Attribution>1</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </ImAddresses>
               </Persona>
               <Persona>
                  <PersonaId Id="AAQkAGQ1MjJjMTBkLkYQAQAJ3EkhEEXN5KufGbSYJanZk=" />
                  <PersonaType>Person</PersonaType>
                  <CreationTime>2012-01-05T23:06:58Z</CreationTime>
                  <DisplayName>Terence Adams</DisplayName>
                  <DisplayNameFirstLast>Terence Adams</DisplayNameFirstLast>
                  <DisplayNameLastFirst>Terence Adams</DisplayNameLastFirst>
                  <FileAsId>None</FileAsId>
                  <EmailAddress>
                     <Name>Terence Adams</Name>
                     <EmailAddress>tadams@contoso.com</EmailAddress>
                     <RoutingType>SMTP</RoutingType>
                  </EmailAddress>
                  <EmailAddresses>
                     <EmailAddress>
                        <Name>Terence Adams</Name>
                        <EmailAddress>tadams@contoso.com</EmailAddress>
                        <RoutingType>SMTP</RoutingType>
                     </EmailAddress>
                  </EmailAddresses>
                  <ImAddress>tadams@contoso.com</ImAddress>
                  <RelevanceScore>2147483647</RelevanceScore>
                  <Attributions>
                     <Attribution>
                        <Id>0</Id>
                        <SourceId Id="AAMkAGQ1MjVOQatt/bhQoTbWAAAA7iVOQatt/bhQoTbWAAAAAAvcAAA=" 
                                  ChangeKey="EQAAABYAAABtF8oI7iVOQatt/bhQoTbWAAAAAAyg" />
                        <DisplayName>Outlook</DisplayName>
                        <IsWritable>true</IsWritable>
                        <IsQuickContact>true</IsQuickContact>
                        <IsHidden>false</IsHidden>
                        <FolderId Id="AAMkAGQ1MjJjMTBkLTc4Y2rBtF8oI7iVOQatt/bhQoTbWAAAAAAvZAAA=" 
                                  ChangeKey="AQAAAA==" />
                     </Attribution>
                  </Attributions>
                  <DisplayNames>
                     <StringAttributedValue>
                        <Value>Terence Adams</Value>
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
                  <Emails1>
                     <EmailAddressAttributedValue>
                        <Value>
                           <Name>Terence Adams</Name>
                           <EmailAddress>tadams@contoso.com</EmailAddress>
                           <RoutingType>SMTP</RoutingType>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </EmailAddressAttributedValue>
                  </Emails1>
                  <ImAddresses>
                     <StringAttributedValue>
                        <Value>tadams@contoso.com</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </ImAddresses>
               </Persona>
            </Personas>
         </ImItemList>
      </GetImItemListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="c30d0-149">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="c30d0-149">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c30d0-150">GetImItemListResponse</span><span class="sxs-lookup"><span data-stu-id="c30d0-150">GetImItemListResponse</span></span>](getimitemlistresponse.md)
    
- [<span data-ttu-id="c30d0-151">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c30d0-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c30d0-152">ImItemList</span><span class="sxs-lookup"><span data-stu-id="c30d0-152">ImItemList</span></span>](imitemlist.md)
    
- [<span data-ttu-id="c30d0-153">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="c30d0-153">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="c30d0-154">GroupType</span><span class="sxs-lookup"><span data-stu-id="c30d0-154">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="c30d0-155">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="c30d0-155">ExchangeStoreId</span></span>](exchangestoreid.md)
    
- [<span data-ttu-id="c30d0-156">MemberCorrelationKey</span><span class="sxs-lookup"><span data-stu-id="c30d0-156">MemberCorrelationKey</span></span>](membercorrelationkey.md)
    
- [<span data-ttu-id="c30d0-157">ItemId</span><span class="sxs-lookup"><span data-stu-id="c30d0-157">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="c30d0-158">Personagens</span><span class="sxs-lookup"><span data-stu-id="c30d0-158">Personas</span></span>](personas-ex15websvcsotherref.md)
    
- [<span data-ttu-id="c30d0-159">PersonaId</span><span class="sxs-lookup"><span data-stu-id="c30d0-159">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="c30d0-160">PersonaType</span><span class="sxs-lookup"><span data-stu-id="c30d0-160">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="c30d0-161">CreationTime</span><span class="sxs-lookup"><span data-stu-id="c30d0-161">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="c30d0-162">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="c30d0-162">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="c30d0-163">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="c30d0-163">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="c30d0-164">FileAs</span><span class="sxs-lookup"><span data-stu-id="c30d0-164">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="c30d0-165">FileAsId</span><span class="sxs-lookup"><span data-stu-id="c30d0-165">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="c30d0-166">GivenName</span><span class="sxs-lookup"><span data-stu-id="c30d0-166">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="c30d0-167">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="c30d0-167">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="c30d0-168">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="c30d0-168">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="c30d0-169">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="c30d0-169">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="c30d0-170">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="c30d0-170">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="c30d0-171">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="c30d0-171">EmailAddresses (ArrayOfEmailAddressesType)</span></span>](emailaddresses-arrayofemailaddressestype.md)
    
- [<span data-ttu-id="c30d0-172">ImAddress (String)</span><span class="sxs-lookup"><span data-stu-id="c30d0-172">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="c30d0-173">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="c30d0-173">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="c30d0-174">Atribuições (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="c30d0-174">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="c30d0-175">Atribuição (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="c30d0-175">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="c30d0-176">ID (String)</span><span class="sxs-lookup"><span data-stu-id="c30d0-176">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="c30d0-177">SourceId</span><span class="sxs-lookup"><span data-stu-id="c30d0-177">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="c30d0-178">IsWritable</span><span class="sxs-lookup"><span data-stu-id="c30d0-178">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="c30d0-179">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="c30d0-179">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="c30d0-180">IsHidden</span><span class="sxs-lookup"><span data-stu-id="c30d0-180">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="c30d0-181">FolderId</span><span class="sxs-lookup"><span data-stu-id="c30d0-181">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="c30d0-182">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="c30d0-182">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="c30d0-183">FileAses</span><span class="sxs-lookup"><span data-stu-id="c30d0-183">FileAses</span></span>](fileases.md)
    
- [<span data-ttu-id="c30d0-184">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="c30d0-184">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="c30d0-185">GivenNames</span><span class="sxs-lookup"><span data-stu-id="c30d0-185">GivenNames</span></span>](givennames.md)
    
- [<span data-ttu-id="c30d0-186">Sobrenomes</span><span class="sxs-lookup"><span data-stu-id="c30d0-186">Surnames</span></span>](surnames.md)
    
- [<span data-ttu-id="c30d0-187">HomePhones</span><span class="sxs-lookup"><span data-stu-id="c30d0-187">HomePhones</span></span>](homephones.md)
    
- [<span data-ttu-id="c30d0-188">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="c30d0-188">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="c30d0-189">MobilePhones</span><span class="sxs-lookup"><span data-stu-id="c30d0-189">MobilePhones</span></span>](mobilephones.md)
    
- [<span data-ttu-id="c30d0-190">Emails1</span><span class="sxs-lookup"><span data-stu-id="c30d0-190">Emails1</span></span>](emails1.md)
    
- [<span data-ttu-id="c30d0-191">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="c30d0-191">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
    
- [<span data-ttu-id="c30d0-192">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="c30d0-192">ImAddresses</span></span>](imaddresses.md)
    
- [<span data-ttu-id="c30d0-193">Valor (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="c30d0-193">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md)
    
## <a name="getimitemlist-operation-error-response"></a><span data-ttu-id="c30d0-194">Resposta de erro de operação GetImItemList</span><span class="sxs-lookup"><span data-stu-id="c30d0-194">GetImItemList operation error response</span></span>

<span data-ttu-id="c30d0-195">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetImItemList** .</span><span class="sxs-lookup"><span data-stu-id="c30d0-195">The following example shows an error response to a **GetImItemList** operation request.</span></span> <span data-ttu-id="c30d0-196">Esta é uma resposta a uma solicitação que contém uma versão incorreta do servidor solicitado no cabeçalho SOAP.</span><span class="sxs-lookup"><span data-stu-id="c30d0-196">This is a response to a request that contains an incorrect requested server version in the SOAP header.</span></span> <span data-ttu-id="c30d0-197">Essa resposta de erro de falha de SOAP e não é representada no esquema do EWS.</span><span class="sxs-lookup"><span data-stu-id="c30d0-197">This error response is a SOAP fault and is not represented in the EWS schema.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="http://schemas.microsoft.com/exchange/services/2006/types">a:ErrorIncorrectSchemaVersion</faultcode>
         <faultstring xml:lang="en-US">The request is valid but does not specify the correct server version in the RequestServerVersion SOAP header.  Ensure that the RequestServerVersion SOAP header is set with the correct RequestServerVersionValue.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">ErrorIncorrectSchemaVersion</e:ResponseCode>
            <e:Message xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">The request is valid but does not specify the correct server version in the RequestServerVersion SOAP header.  Ensure that the RequestServerVersion SOAP header is set with the correct RequestServerVersionValue.</e:Message>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="c30d0-198">Confira também</span><span class="sxs-lookup"><span data-stu-id="c30d0-198">See also</span></span>

- [<span data-ttu-id="c30d0-199">Operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="c30d0-199">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="c30d0-200">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c30d0-200">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="c30d0-201">Operação GetImItems</span><span class="sxs-lookup"><span data-stu-id="c30d0-201">GetImItems operation</span></span>](getimitems-operation.md)
    

