---
title: Operação GetServiceConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServiceConfiguration
api_type:
- schema
ms.assetid: 070cbfe5-325a-4955-8e4a-8230ea0459a7
description: A operação GetServiceConfiguration Obtém informações de configuração para o tipo de serviço especificado. Essa operação pode retornar definições de configuração para a Unificação de mensagens, regras de proteção e serviços de dicas de email.
ms.openlocfilehash: b8ea2cef366a52765850dddcc8c1ef1e8fa68b22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460908"
---
# <a name="getserviceconfiguration-operation"></a><span data-ttu-id="0b314-104">Operação GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b314-104">GetServiceConfiguration operation</span></span>

<span data-ttu-id="0b314-105">A operação **GetServiceConfiguration** Obtém informações de configuração para o tipo de serviço especificado.</span><span class="sxs-lookup"><span data-stu-id="0b314-105">The **GetServiceConfiguration** operation gets configuration information for the specified type of service.</span></span> <span data-ttu-id="0b314-106">Essa operação pode retornar definições de configuração para a Unificação de mensagens, regras de proteção e serviços de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="0b314-106">This operation can return configuration settings for the Unified Messaging, Protection Rules, and Mail Tips services.</span></span> 
  
## <a name="getserviceconfiguration-request-example"></a><span data-ttu-id="0b314-107">Exemplo de solicitação GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b314-107">GetServiceConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="0b314-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b314-108">Description</span></span>

<span data-ttu-id="0b314-109">O exemplo a seguir de uma solicitação **GetServiceConfiguration** mostra como formar uma solicitação para obter informações de configuração para o serviço de Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="0b314-109">The following example of a **GetServiceConfiguration** request shows how to form a request to get configuration information for the Unified Messaging service.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0b314-110">Código</span><span class="sxs-lookup"><span data-stu-id="0b314-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetServiceConfiguration>
      <m:RequestedConfiguration>
        <m:ConfigurationName>UnifiedMessagingConfiguration</m:ConfigurationName>
      </m:RequestedConfiguration>
    </m:GetServiceConfiguration>
  </soap:Body>
</soap:Envelope>
```

## <a name="getserviceconfiguration-response-example"></a><span data-ttu-id="0b314-111">Exemplo de resposta GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b314-111">GetServiceConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="0b314-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b314-112">Description</span></span>

<span data-ttu-id="0b314-113">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação **GetServiceConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="0b314-113">The following example shows a successful response to the **GetServiceConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0b314-114">Código</span><span class="sxs-lookup"><span data-stu-id="0b314-114">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetServiceConfigurationResponse ResponseClass="Success" 
                                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <ResponseMessages>
        <ServiceConfigurationResponseMessageType ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <m:UnifiedMessagingConfiguration xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
            <t:UmEnabled xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">true</t:UmEnabled>
            <t:PlayOnPhoneDialString xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">user@contoso.com</t:PlayOnPhoneDialString>
            <t:PlayOnPhoneEnabled xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">true</t:PlayOnPhoneEnabled>
          </m:UnifiedMessagingConfiguration>
        </ServiceConfigurationResponseMessageType>
      </ResponseMessages>
    </GetServiceConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="getserviceconfiguration-error-response-example"></a><span data-ttu-id="0b314-115">Exemplo de resposta de erro GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b314-115">GetServiceConfiguration Error response example</span></span>

### <a name="description"></a><span data-ttu-id="0b314-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b314-116">Description</span></span>

<span data-ttu-id="0b314-117">O exemplo a seguir mostra uma resposta de erro para a solicitação **GetServiceConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="0b314-117">The following example shows an error response to the **GetServiceConfiguration** request.</span></span> <span data-ttu-id="0b314-118">Este erro foi causado por um nome de configuração incorreto.</span><span class="sxs-lookup"><span data-stu-id="0b314-118">This error was caused by an incorrect configuration name.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0b314-119">Código</span><span class="sxs-lookup"><span data-stu-id="0b314-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body>
    <s:Fault>
      <faultcode xmlns:a="https://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
      <faultstring xml:lang="en-US">The request failed schema validation: 
      The 'https://schemas.microsoft.com/exchange/services/2006/messages:ConfigurationName' element 
      is invalid - The value 'UUnifiedMessagingConfiguration' is invalid according to its 
      datatype 'https://schemas.microsoft.com/exchange/services/2006/types:ServiceConfigurationType' 
      - The Enumeration constraint failed.</faultstring>
      <detail>
        <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
        <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
        <t:MessageXml xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
          <t:LineNumber>13</t:LineNumber>
          <t:LinePosition>62</t:LinePosition>
          <t:Violation>The 'https://schemas.microsoft.com/exchange/services/2006/messages:ConfigurationName' element 
          is invalid - The value 'UUnifiedMessagingConfiguration' is invalid according to its 
          datatype 'https://schemas.microsoft.com/exchange/services/2006/types:ServiceConfigurationType'
          - The Enumeration constraint failed.</t:Violation>
        </t:MessageXml>
      </detail>
    </s:Fault>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="0b314-120">Também consulte</span><span class="sxs-lookup"><span data-stu-id="0b314-120">See also</span></span>



[<span data-ttu-id="0b314-121">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0b314-121">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="0b314-122">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0b314-122">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

