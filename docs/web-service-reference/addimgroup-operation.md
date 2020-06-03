---
title: Operação AddImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6df6e504-b7c8-4773-b10f-ffa5defac229
description: Encontre informações sobre a operação do EWS do AddImGroup.
ms.openlocfilehash: 38ed12a741d46fe998dc0079ed13973ce9edf5ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462812"
---
# <a name="addimgroup-operation"></a><span data-ttu-id="7ee8f-103">Operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="7ee8f-103">AddImGroup operation</span></span>

<span data-ttu-id="7ee8f-104">Encontre informações sobre a operação do EWS do **AddImGroup** .</span><span class="sxs-lookup"><span data-stu-id="7ee8f-104">Find information about the **AddImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="7ee8f-105">A operação do **AddImGroup** do serviços Web do Exchange (EWS) adiciona um novo grupo de mensagens instantâneas (IM) a uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-105">The **AddImGroup** Exchange Web Services (EWS) operation adds a new instant messaging (IM) group to a mailbox.</span></span> 
  
<span data-ttu-id="7ee8f-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addimgroup-operation"></a><span data-ttu-id="7ee8f-107">Usando a operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="7ee8f-107">Using the AddImGroup operation</span></span>

<span data-ttu-id="7ee8f-108">A operação **AddImGroup** usa apenas um único argumento de nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-108">The **AddImGroup** operation only takes a single display name argument.</span></span> 
  
<span data-ttu-id="7ee8f-109">Essa operação retorna o nome de exibição, o tipo de grupo e o identificador de repositório do Exchange do novo grupo.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-109">This operation returns the display name, group type, and Exchange store identifier of the new group.</span></span>
  
<span data-ttu-id="7ee8f-110">A operação **AddImGroup** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-110">The **AddImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="7ee8f-111">**Tabela 1. Cabeçalhos SOAP de operação AddImGroup**</span><span class="sxs-lookup"><span data-stu-id="7ee8f-111">**Table 1. AddImGroup operation SOAP headers**</span></span>

|<span data-ttu-id="7ee8f-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="7ee8f-112">**Header name**</span></span>|<span data-ttu-id="7ee8f-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7ee8f-113">**Element**</span></span>|<span data-ttu-id="7ee8f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7ee8f-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7ee8f-115">**Representação**</span><span class="sxs-lookup"><span data-stu-id="7ee8f-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="7ee8f-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="7ee8f-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="7ee8f-117">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="7ee8f-118">Isso se aplica a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-118">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7ee8f-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="7ee8f-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="7ee8f-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="7ee8f-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="7ee8f-121">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="7ee8f-122">Isso se aplica a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-122">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7ee8f-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="7ee8f-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="7ee8f-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="7ee8f-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="7ee8f-125">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="7ee8f-126">Isso se aplica a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-126">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7ee8f-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="7ee8f-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="7ee8f-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7ee8f-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="7ee8f-129">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="7ee8f-130">Isso se aplica a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-130">This is applicable to a response.</span></span>  <br/> |
   
## <a name="addimgroup-operation-request-example-create-a-new-im-group"></a><span data-ttu-id="7ee8f-131">Exemplo de solicitação de operação AddImGroup: criar um novo grupo de IM</span><span class="sxs-lookup"><span data-stu-id="7ee8f-131">AddImGroup operation request example: Create a new IM group</span></span>

<span data-ttu-id="7ee8f-132">O exemplo a seguir de uma solicitação de operação **AddImGroup** mostra como criar um grupo de mensagens instantâneas chamado mycustomerobject.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-132">The following example of an **AddImGroup** operation request shows how to create an IM group named MyCustomerGroup.</span></span> 
  
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
      <m:AddImGroup>
         <m:DisplayName>MyCustomGroup</m:DisplayName>
      </m:AddImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="7ee8f-133">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="7ee8f-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7ee8f-134">AddImGroup</span><span class="sxs-lookup"><span data-stu-id="7ee8f-134">AddImGroup</span></span>](addimgroup.md)
    
- [<span data-ttu-id="7ee8f-135">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="7ee8f-135">DisplayName (string)</span></span>](displayname-string.md)
    
## <a name="successful-addimgroup-operation-response"></a><span data-ttu-id="7ee8f-136">Resposta de operação AddImGroup bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="7ee8f-136">Successful AddImGroup operation response</span></span>

<span data-ttu-id="7ee8f-137">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **AddImGroup** .</span><span class="sxs-lookup"><span data-stu-id="7ee8f-137">The following example shows a successful response to an **AddImGroup** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0"
                           MajorBuildNumber="349"
                           MinorBuildNumber="0"
                           Version="Exchange2013"
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImGroupResponse ResponseClass="Success"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImGroup>
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">MyCustomGroup</DisplayName>
            <GroupType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">IPM.DistList.MOC.UserGroup</GroupType>
            <ExchangeStoreId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MAAA="
                             ChangeKey="EgAAAA=="
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/types"/>
         </ImGroup>
      </AddImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="7ee8f-138">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="7ee8f-138">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7ee8f-139">AddImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="7ee8f-139">AddImGroupResponse</span></span>](addimgroupresponse.md)
    
- [<span data-ttu-id="7ee8f-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7ee8f-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7ee8f-141">Imgroup</span><span class="sxs-lookup"><span data-stu-id="7ee8f-141">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="7ee8f-142">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="7ee8f-142">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="7ee8f-143">GroupType</span><span class="sxs-lookup"><span data-stu-id="7ee8f-143">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="7ee8f-144">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="7ee8f-144">ExchangeStoreId</span></span>](exchangestoreid.md)
    
## <a name="addimgroup-operation-error-response"></a><span data-ttu-id="7ee8f-145">Resposta de erro de operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="7ee8f-145">AddImGroup operation error response</span></span>

<span data-ttu-id="7ee8f-146">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **AddImGroup** .</span><span class="sxs-lookup"><span data-stu-id="7ee8f-146">The following example shows an error response to an **AddImGroup** operation request.</span></span> <span data-ttu-id="7ee8f-147">Esta é uma resposta a uma solicitação que contém um caractere que não pode ser usado em um nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-147">This is a response to a request that contains a character that cannot be used in a display name.</span></span> <span data-ttu-id="7ee8f-148">Observe que esta é uma falha SOAP e não uma mensagem de erro baseada em esquema.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-148">Note that this is a SOAP fault and not a schema-based error message.</span></span> <span data-ttu-id="7ee8f-149">O nome de exibição enviado na solicitação é ~! @ # $% ^ &amp; e o erro ocorre no &amp; caractere.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-149">The display name submitted in the request is ~!@#$%^&amp;, and the error occurs on the &amp; character.</span></span> <span data-ttu-id="7ee8f-150">O &amp; caractere ocorreu na linha 11 e no caractere 33rd na carga de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-150">The &amp; character occurred on the 11th line and 33rd character in the request payload.</span></span> <span data-ttu-id="7ee8f-151">A resposta foi retornada com um código HTTP 500.</span><span class="sxs-lookup"><span data-stu-id="7ee8f-151">The response was returned with an HTTP 500 code.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="https://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
         <faultstring xml:lang="en-US">The request failed schema validation: An error occurred while parsing EntityName. Line 11, position 33.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
            <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
            <t:MessageXml xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
               <t:LineNumber>11</t:LineNumber>
               <t:LinePosition>33</t:LinePosition>
               <t:Violation>An error occurred while parsing EntityName. Line 11, position 33.</t:Violation>
            </t:MessageXml>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="7ee8f-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="7ee8f-152">See also</span></span>

- [<span data-ttu-id="7ee8f-153">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7ee8f-153">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="7ee8f-154">Operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="7ee8f-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="7ee8f-155">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="7ee8f-155">SetImGroup</span></span>](setimgroup.md)
    

