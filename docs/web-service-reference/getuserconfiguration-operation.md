---
title: Operação GetUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserConfiguration
api_type:
- schema
ms.assetid: 71d50e3c-92bd-435f-8118-b28bb85f8138
description: A operação GetUserConfiguration Obtém um objeto de configuração de usuário de uma pasta.
ms.openlocfilehash: fb28e88d1a47b0ea8f63ed33b1efacae8538e1c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458205"
---
# <a name="getuserconfiguration-operation"></a><span data-ttu-id="b6da7-103">Operação GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="b6da7-103">GetUserConfiguration operation</span></span>

<span data-ttu-id="b6da7-104">A operação **GetUserConfiguration** Obtém um objeto de configuração de usuário de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="b6da7-104">The **GetUserConfiguration** operation gets a user configuration object from a folder.</span></span> 
  
## <a name="getuserconfiguration-request-example"></a><span data-ttu-id="b6da7-105">Exemplo de solicitação GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="b6da7-105">GetUserConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="b6da7-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6da7-106">Description</span></span>

<span data-ttu-id="b6da7-107">O exemplo a seguir de uma solicitação **GetUserConfiguration** mostra como formar uma solicitação para obter um objeto de configuração do usuário na pasta Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="b6da7-107">The following example of a **GetUserConfiguration** request shows how to form a request to get a user configuration object on the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b6da7-108">Código</span><span class="sxs-lookup"><span data-stu-id="b6da7-108">Code</span></span>

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
    <m:GetUserConfiguration>
      <m:UserConfigurationName Name="TestConfig">
        <t:DistinguishedFolderId Id="drafts"/>
      </m:UserConfigurationName>
      <m:UserConfigurationProperties>Dictionary</m:UserConfigurationProperties>
    </m:GetUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

## <a name="getuserconfiguration-response-example"></a><span data-ttu-id="b6da7-109">Exemplo de resposta GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="b6da7-109">GetUserConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="b6da7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6da7-110">Description</span></span>

<span data-ttu-id="b6da7-111">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação **GetUserConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="b6da7-111">The following example shows a successful response to the **GetUserConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b6da7-112">Código</span><span class="sxs-lookup"><span data-stu-id="b6da7-112">Code</span></span>

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
    <m:GetUserConfigurationResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:UserConfiguration>
            <t:UserConfigurationName Name="TestConfig">
              <t:DistinguishedFolderId Id="drafts">
              </t:DistinguishedFolderId>
            </t:UserConfigurationName>
            <t:Dictionary>
              <t:DictionaryEntry>
                <t:DictionaryKey>
                  <t:Type>String</t:Type>
                  <t:Value>PhoneNumber</t:Value>
                </t:DictionaryKey>
                <t:DictionaryValue>
                  <t:Type>String</t:Type>
                  <t:Value>555-555-1111</t:Value>
                </t:DictionaryValue>
              </t:DictionaryEntry>
            </t:Dictionary>
          </m:UserConfiguration>
        </m:GetUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:GetUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="b6da7-113">Também consulte</span><span class="sxs-lookup"><span data-stu-id="b6da7-113">See also</span></span>



[<span data-ttu-id="b6da7-114">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b6da7-114">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="b6da7-115">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b6da7-115">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

