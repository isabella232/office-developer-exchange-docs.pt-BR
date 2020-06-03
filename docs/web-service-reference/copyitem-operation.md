---
title: Operação CopyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItem
api_type:
- schema
ms.assetid: bcc68f9e-d511-4c29-bba6-ed535524624a
description: A operação CopyItem copia itens e coloca os itens em uma pasta diferente.
ms.openlocfilehash: ec07700a5ebbdc8774aa2134919634b8dfd02406
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462175"
---
# <a name="copyitem-operation"></a>Operação CopyItem

A operação **CopyItem** copia itens e coloca os itens em uma pasta diferente. 
  
## <a name="copyitem-request-example"></a>Exemplo de solicitação CopyItem

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação **CopyItem** mostra como formar uma solicitação para copiar um item para a caixa de entrada. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <ItemIds>
        <t:ItemId Id="AS4AUnV="/>
      </ItemIds>
    </CopyItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

> [!NOTE]
> A ID da pasta e a chave de alteração foram reduzidas para preservar a legibilidade. 
  
### <a name="request-elements"></a>Elementos Request

Os seguintes elementos são usados na solicitação:
  
- [CopyItem](copyitem.md)
    
- [ToFolderId](tofolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
> [!NOTE]
> O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada. 
  
Para encontrar outras opções para a mensagem de solicitação da operação **CopyItem** , explore a hierarquia de esquema. Inicie no elemento [CopyItem](copyitem.md) . 
  
## <a name="successful-copyitem-response"></a>Resposta CopyItem bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida à solicitação **CopyItem** . 
  
O identificador de item do novo item é retornado na mensagem de resposta. Os identificadores de item não são retornados em respostas para as operações de **CopyItem** de caixa de correio ou de caixa de correio de pasta pública. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemID Id="AAMkAd" ChangeKey="FwAAABY" />
            </t:Message>
          </m:Items>
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CopyItemResponse](copyitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CopyItemResponseMessage](copyitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Itens](items.md)
    
Para encontrar outras opções para a mensagem de resposta da operação **CopyItem** , explore a hierarquia do esquema. Inicie no elemento [CopyItemResponse](copyitemresponse.md) . 
  
## <a name="copyitem-error-response"></a>Resposta de erro CopyItem

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma solicitação **CopyItem** . 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Elementos de resposta de erro

Os seguintes elementos são usados na resposta de erro:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CopyItemResponse](copyitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CopyItemResponseMessage](copyitemresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Itens](items.md)
    
Para encontrar outras opções para a mensagem de resposta de erro da operação **CopyItem** , explore a hierarquia de esquema. Inicie no elemento [CopyItemResponse](copyitemresponse.md) . 
  
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

