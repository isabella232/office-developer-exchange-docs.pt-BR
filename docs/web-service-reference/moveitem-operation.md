---
title: Operação MoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MoveItem
api_type:
- schema
ms.assetid: dcf40fa7-7796-4a5c-bf5b-7a509a18d208
description: A operação MoveItem é usada para mover um ou mais itens para uma única pasta de destino.
ms.openlocfilehash: 2d86d06e522e0d42815971c92e754308224f5e8f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544847"
---
# <a name="moveitem-operation"></a>Operação MoveItem

A **operação MoveItem** é usada para mover um ou mais itens para uma única pasta de destino. 
  
## <a name="moveitem-request-example"></a>Exemplo de solicitação MoveItem

### <a name="description"></a>Descrição

O exemplo a seguir de **uma solicitação MoveItem** mostra como mover um item para a pasta Rascunhos. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ToFolderId>
        <t:DistinguishedFolderId Id="drafts"/>
      </ToFolderId>
      <ItemIds>
        <t:ItemId Id="AAAtAEF/swbAAA=" ChangeKey="EwAAABYA/s4b"/>
      </ItemIds>
    </MoveItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

O [elemento ToFolderId](tofolderid.md) especifica a pasta para a qual os itens serão movidos. Observe que todos os itens listados na [coleção ItemIds](itemids.md) terminarão na pasta de destino. Você deve fazer chamadas **moveItem** separadas para colocar itens em pastas de destino diferentes. 
  
> [!NOTE]
> O identificador de item e a chave de alteração foram reduzidos para preservar a capacidade de leitura. 
  
### <a name="request-elements"></a>Elementos request

Os seguintes elementos são usados na solicitação:
  
- [MoveItem](moveitem.md)
    
- [ToFolderId](tofolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="moveitem-response-example"></a>Exemplo de resposta MoveItem

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida a uma **solicitação MoveItem.** 
  
O identificador de item do novo item é retornado na mensagem de resposta. Os identificadores de item não são retornados em respostas para caixas de correio cruzada ou caixa de correio para operações **MoveItem de** pasta pública. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <MoveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemID Id="AAMkAd" ChangeKey="FwAAABY" />
            </t:Message>
          </m:Items>
        </m:MoveItemResponseMessage>
      </m:ResponseMessages>
    </MoveItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

A **operação MoveItem** indicará sucesso se a movimentação foi bem-sucedida. 
  
### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [MoveItemResponse](moveitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MoveItemResponseMessage](moveitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Itens](items.md)
    
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

