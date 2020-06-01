---
title: Operação GetImItemList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e31d14e1-0c1f-4b69-98b7-157d59c13698
description: Encontre informações sobre a operação do EWS do GetImItemList.
ms.openlocfilehash: aabe84054b93e7de8af6145942493a0224932e45
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456063"
---
# <a name="getimitemlist-operation"></a><span data-ttu-id="19108-103">Operação GetImItemList</span><span class="sxs-lookup"><span data-stu-id="19108-103">GetImItemList operation</span></span>

<span data-ttu-id="19108-104">Encontre informações sobre a operação do EWS do **GetImItemList** .</span><span class="sxs-lookup"><span data-stu-id="19108-104">Find information about the **GetImItemList** EWS operation.</span></span> 
  
## <a name="using-the-getimitemlist-operation"></a><span data-ttu-id="19108-105">Usando a operação GetImItemList</span><span class="sxs-lookup"><span data-stu-id="19108-105">Using the GetImItemList operation</span></span>

<span data-ttu-id="19108-106">A operação **GetImItemList** recupera a lista de grupos de mensagens instantâneas (IM) e contato de mensagens instantâneas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="19108-106">The **GetImItemList** operation retrieves the list of instant messaging (IM) groups and IM contact personas in a mailbox.</span></span> <span data-ttu-id="19108-107">A operação **GetImItemList** não tem argumentos.</span><span class="sxs-lookup"><span data-stu-id="19108-107">The **GetImItemList** operation does not take any arguments.</span></span> 
  
<span data-ttu-id="19108-108">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="19108-108">This operation was introduced in Exchange Server 2013.</span></span>
  
### <a name="getimitemlist-operation-soap-headers"></a><span data-ttu-id="19108-109">Cabeçalhos SOAP de operação GetImItemList</span><span class="sxs-lookup"><span data-stu-id="19108-109">GetImItemList operation SOAP headers</span></span>

<span data-ttu-id="19108-110">A operação **GetImItemList** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="19108-110">The **GetImItemList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="19108-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="19108-111">**Header name**</span></span>|<span data-ttu-id="19108-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="19108-112">**Element**</span></span>|<span data-ttu-id="19108-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="19108-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="19108-114">**Representação**</span><span class="sxs-lookup"><span data-stu-id="19108-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="19108-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="19108-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="19108-116">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="19108-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="19108-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="19108-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="19108-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="19108-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="19108-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="19108-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="19108-120">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="19108-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="19108-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="19108-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="19108-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="19108-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="19108-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="19108-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="19108-124">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="19108-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="19108-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="19108-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="19108-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="19108-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="19108-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="19108-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="19108-128">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="19108-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="19108-129">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="19108-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getimitemlist-operation-request-example-request-your-im-items-list"></a><span data-ttu-id="19108-130">Exemplo de solicitação de operação GetImItemList: solicitar sua lista de itens de mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="19108-130">GetImItemList operation request example: Request your IM items list</span></span>

<span data-ttu-id="19108-131">O exemplo a seguir de uma solicitação de operação **GetImItemList** mostra como solicitar a lista de grupos de IM e pessoas de contato de mensagens instantâneas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="19108-131">The following example of a **GetImItemList** operation request shows how to request the list of IM groups and IM contact personas in a mailbox.</span></span> <span data-ttu-id="19108-132">O elemento **GetImItemList** é a única opção de elemento no corpo SOAP.</span><span class="sxs-lookup"><span data-stu-id="19108-132">The **GetImItemList** element is the only element option in the SOAP body.</span></span> 
  
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
      <m:GetImItemList/>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="19108-133">O corpo SOAP de solicitação contém o seguinte elemento:</span><span class="sxs-lookup"><span data-stu-id="19108-133">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="19108-134">GetImItemList</span><span class="sxs-lookup"><span data-stu-id="19108-134">GetImItemList</span></span>](getimitemlist.md)
    
## <a name="successful-getimitemlist-operation-response"></a><span data-ttu-id="19108-135">Resposta de operação GetImItemList bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="19108-135">Successful GetImItemList operation response</span></span>

<span data-ttu-id="19108-136">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetImItemList** .</span><span class="sxs-lookup"><span data-stu-id="19108-136">The following example shows a successful response to a **GetImItemList** operation request.</span></span> <span data-ttu-id="19108-137">A resposta contém quatro grupos de IM.</span><span class="sxs-lookup"><span data-stu-id="19108-137">The response contains four IM groups.</span></span> <span data-ttu-id="19108-138">Três dos grupos de mensagens instantâneas — outros contatos, marcados e favoritos — são grupos padrão no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="19108-138">Three of the IM groups — Other Contacts, Tagged, and Favorites — are default groups in the Exchange store.</span></span> <span data-ttu-id="19108-139">O grupo MyCustomGroup2 é um grupo personalizado criado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="19108-139">The MyCustomGroup2 group is a custom user-created group.</span></span> <span data-ttu-id="19108-140">Os outros contatos e grupos marcados não têm Membros.</span><span class="sxs-lookup"><span data-stu-id="19108-140">The Other Contacts and Tagged groups do not have members.</span></span> <span data-ttu-id="19108-141">O grupo favoritos tem um único membro de contato.</span><span class="sxs-lookup"><span data-stu-id="19108-141">The Favorites group has a single contact member.</span></span> <span data-ttu-id="19108-142">O MyCustomGroup2 tem dois contatos Membros.</span><span class="sxs-lookup"><span data-stu-id="19108-142">The MyCustomGroup2 has two member contacts.</span></span> <span data-ttu-id="19108-143">Os identificadores de item são fornecidos para que as solicitações subsequentes do **GetItem** possam ser realizadas para obter mais informações sobre os contatos de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="19108-143">The item identifiers are provided so that subsequent **GetItem** requests can be performed to get more information about the IM contacts.</span></span> 
  
<span data-ttu-id="19108-144">Este exemplo retorna duas personas.</span><span class="sxs-lookup"><span data-stu-id="19108-144">This example returns two personas.</span></span> <span data-ttu-id="19108-145">O primeiro persona representa dois itens de contato: Anthony Smith e Tony Smith.</span><span class="sxs-lookup"><span data-stu-id="19108-145">The first persona represents two contact items: Anthony Smith and Tony Smith.</span></span> <span data-ttu-id="19108-146">As informações de contato combinadas são retornadas no objeto **persona** .</span><span class="sxs-lookup"><span data-stu-id="19108-146">The combined contact information is returned in the **Persona** object.</span></span> <span data-ttu-id="19108-147">O segundo persona representa um único contato com o nome de exibição de Terence Adams.</span><span class="sxs-lookup"><span data-stu-id="19108-147">The second persona represents a single contact with the display name of Terence Adams.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="19108-148">Os identificadores de repositório do Exchange, identificadores de item, identificadores de origem, identificadores de pasta e identificadores persona foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="19108-148">The Exchange store identifiers, item identifiers, source identifiers, folder identifiers, and persona identifiers have been shortened to preserve readability.</span></span> 
  
```XML
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
      <GetImItemListResponse ResponseClass="Success" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
            <Personas xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="19108-149">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="19108-149">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="19108-150">GetImItemListResponse</span><span class="sxs-lookup"><span data-stu-id="19108-150">GetImItemListResponse</span></span>](getimitemlistresponse.md)
    
- [<span data-ttu-id="19108-151">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="19108-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="19108-152">Imitemlist</span><span class="sxs-lookup"><span data-stu-id="19108-152">ImItemList</span></span>](imitemlist.md)
    
- [<span data-ttu-id="19108-153">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="19108-153">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="19108-154">GroupType</span><span class="sxs-lookup"><span data-stu-id="19108-154">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="19108-155">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="19108-155">ExchangeStoreId</span></span>](exchangestoreid.md)
    
- [<span data-ttu-id="19108-156">MemberCorrelationKey</span><span class="sxs-lookup"><span data-stu-id="19108-156">MemberCorrelationKey</span></span>](membercorrelationkey.md)
    
- [<span data-ttu-id="19108-157">ItemId</span><span class="sxs-lookup"><span data-stu-id="19108-157">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="19108-158">Personas</span><span class="sxs-lookup"><span data-stu-id="19108-158">Personas</span></span>](personas-ex15websvcsotherref.md)
    
- [<span data-ttu-id="19108-159">Personaid</span><span class="sxs-lookup"><span data-stu-id="19108-159">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="19108-160">Personatype</span><span class="sxs-lookup"><span data-stu-id="19108-160">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="19108-161">CreationTime</span><span class="sxs-lookup"><span data-stu-id="19108-161">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="19108-162">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="19108-162">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="19108-163">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="19108-163">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="19108-164">FileAs</span><span class="sxs-lookup"><span data-stu-id="19108-164">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="19108-165">FileAsId</span><span class="sxs-lookup"><span data-stu-id="19108-165">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="19108-166">GivenName</span><span class="sxs-lookup"><span data-stu-id="19108-166">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="19108-167">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="19108-167">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="19108-168">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="19108-168">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="19108-169">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="19108-169">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="19108-170">RoutingType (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="19108-170">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="19108-171">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="19108-171">EmailAddresses (ArrayOfEmailAddressesType)</span></span>](emailaddresses-arrayofemailaddressestype.md)
    
- [<span data-ttu-id="19108-172">IMAddress (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="19108-172">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="19108-173">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="19108-173">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="19108-174">Atribuições (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="19108-174">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="19108-175">Atribuição (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="19108-175">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="19108-176">ID (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="19108-176">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="19108-177">SourceId</span><span class="sxs-lookup"><span data-stu-id="19108-177">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="19108-178">Iswritable</span><span class="sxs-lookup"><span data-stu-id="19108-178">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="19108-179">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="19108-179">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="19108-180">IsHidden</span><span class="sxs-lookup"><span data-stu-id="19108-180">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="19108-181">FolderId</span><span class="sxs-lookup"><span data-stu-id="19108-181">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="19108-182">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="19108-182">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="19108-183">FileAses</span><span class="sxs-lookup"><span data-stu-id="19108-183">FileAses</span></span>](fileases.md)
    
- [<span data-ttu-id="19108-184">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="19108-184">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="19108-185">Dados fornecidos</span><span class="sxs-lookup"><span data-stu-id="19108-185">GivenNames</span></span>](givennames.md)
    
- [<span data-ttu-id="19108-186">Sobrenomes</span><span class="sxs-lookup"><span data-stu-id="19108-186">Surnames</span></span>](surnames.md)
    
- [<span data-ttu-id="19108-187">HomePhones</span><span class="sxs-lookup"><span data-stu-id="19108-187">HomePhones</span></span>](homephones.md)
    
- [<span data-ttu-id="19108-188">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="19108-188">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="19108-189">MobilePhones</span><span class="sxs-lookup"><span data-stu-id="19108-189">MobilePhones</span></span>](mobilephones.md)
    
- [<span data-ttu-id="19108-190">Emails1</span><span class="sxs-lookup"><span data-stu-id="19108-190">Emails1</span></span>](emails1.md)
    
- [<span data-ttu-id="19108-191">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="19108-191">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
    
- [<span data-ttu-id="19108-192">Imendereços</span><span class="sxs-lookup"><span data-stu-id="19108-192">ImAddresses</span></span>](imaddresses.md)
    
- [<span data-ttu-id="19108-193">Valor (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="19108-193">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md)
    
## <a name="getimitemlist-operation-error-response"></a><span data-ttu-id="19108-194">Resposta de erro de operação GetImItemList</span><span class="sxs-lookup"><span data-stu-id="19108-194">GetImItemList operation error response</span></span>

<span data-ttu-id="19108-195">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetImItemList** .</span><span class="sxs-lookup"><span data-stu-id="19108-195">The following example shows an error response to a **GetImItemList** operation request.</span></span> <span data-ttu-id="19108-196">Esta é uma resposta a uma solicitação que contém uma versão de servidor solicitada incorreta no cabeçalho SOAP.</span><span class="sxs-lookup"><span data-stu-id="19108-196">This is a response to a request that contains an incorrect requested server version in the SOAP header.</span></span> <span data-ttu-id="19108-197">Essa resposta de erro é uma falha SOAP e não é representada no esquema do EWS.</span><span class="sxs-lookup"><span data-stu-id="19108-197">This error response is a SOAP fault and is not represented in the EWS schema.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="https://schemas.microsoft.com/exchange/services/2006/types">a:ErrorIncorrectSchemaVersion</faultcode>
         <faultstring xml:lang="en-US">The request is valid but does not specify the correct server version in the RequestServerVersion SOAP header.  Ensure that the RequestServerVersion SOAP header is set with the correct RequestServerVersionValue.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorIncorrectSchemaVersion</e:ResponseCode>
            <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The request is valid but does not specify the correct server version in the RequestServerVersion SOAP header.  Ensure that the RequestServerVersion SOAP header is set with the correct RequestServerVersionValue.</e:Message>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="19108-198">Também consulte</span><span class="sxs-lookup"><span data-stu-id="19108-198">See also</span></span>

- [<span data-ttu-id="19108-199">Operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="19108-199">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="19108-200">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="19108-200">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="19108-201">Operação GetImItems</span><span class="sxs-lookup"><span data-stu-id="19108-201">GetImItems operation</span></span>](getimitems-operation.md)
    

