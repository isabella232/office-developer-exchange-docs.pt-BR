---
title: Operação CreateUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateUserConfiguration
api_type:
- schema
ms.assetid: eb5b8ab6-9743-481c-aac9-f9aa889bd353
description: A operação CreateUserConfiguration cria um objeto de configuração do usuário em uma pasta.
ms.openlocfilehash: 0c9233146d21c7014be15896426b968106485200
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463780"
---
# <a name="createuserconfiguration-operation"></a><span data-ttu-id="7cfb7-103">Operação CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="7cfb7-103">CreateUserConfiguration operation</span></span>

<span data-ttu-id="7cfb7-104">A operação **CreateUserConfiguration** cria um objeto de configuração do usuário em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="7cfb7-104">The **CreateUserConfiguration** operation creates a user configuration object on a folder.</span></span> 
  
## <a name="createuserconfiguration-request-example"></a><span data-ttu-id="7cfb7-105">Exemplo de solicitação CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="7cfb7-105">CreateUserConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="7cfb7-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cfb7-106">Description</span></span>

<span data-ttu-id="7cfb7-107">O exemplo a seguir de uma solicitação **CreateUserConfiguration** mostra como formar uma solicitação para criar um objeto de configuração do usuário na pasta Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="7cfb7-107">The following example of a **CreateUserConfiguration** request shows how to form a request to create a user configuration object on the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7cfb7-108">Código</span><span class="sxs-lookup"><span data-stu-id="7cfb7-108">Code</span></span>

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
    <m:CreateUserConfiguration>
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
    </m:CreateUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

## <a name="createuserconfiguration-response-example"></a><span data-ttu-id="7cfb7-109">Exemplo de resposta CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="7cfb7-109">CreateUserConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="7cfb7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cfb7-110">Description</span></span>

<span data-ttu-id="7cfb7-111">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação **CreateUserConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="7cfb7-111">The following example shows a successful response to the **CreateUserConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7cfb7-112">Código</span><span class="sxs-lookup"><span data-stu-id="7cfb7-112">Code</span></span>

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
    <m:CreateUserConfigurationResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:CreateUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:CreateUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="7cfb7-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="7cfb7-113">See also</span></span>



[<span data-ttu-id="7cfb7-114">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7cfb7-114">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="7cfb7-115">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7cfb7-115">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

