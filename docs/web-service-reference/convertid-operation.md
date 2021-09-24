---
title: Operação ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 47d96cf6-9e2f-4fc0-9682-7258d3fbf918
description: Encontre informações sobre a operação ConvertId EWS.
ms.openlocfilehash: 04f20d8446ab3117adb3f00ea17f93c068eeffb9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536628"
---
# <a name="convertid-operation"></a>Operação ConvertId

Encontre informações sobre a **operação ConvertId** EWS. 
  
A operação **ConvertId** Exchange Web Services (EWS) converte identificadores de item e pasta entre formatos aceitos pelo Exchange Online, Exchange Online como parte do Office 365 e versões locais do Exchange Exchange Server 2013. 
  
## <a name="using-the-convertid-operation"></a>Usando a operação ConvertId
<a name="bk_usingConvertId"> </a>

Você pode converter os seguintes identificadores usando a **operação ConvertId:** 
  
- O formato identificador do EWS na versão inicial do Exchange 2007. Isso é representado pelo valor `EwsLegacyId` de enumeração na enumeração [IdFormat.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) 
    
- O formato identificador do EWS no Exchange 2007 SP1 ou Exchange 2010. Isso é representado pelo valor  `EwsId` de enumeração em [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- O identificador MAPI, como na propriedade **PR_ENTRYID.** Isso é representado pelo valor `EntryId` de enumeração na enumeração [IdFormat.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) 
    
- O identificador de evento do calendário de disponibilidade. Esta é uma representação codificada por hexadecimal da **propriedade PR_ENTRYID.** Isso é representado pelo valor  `HexEntryId` de enumeração em [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- O Exchange de armazenamento. Isso é representado pelo valor  `StoreId` de enumeração em [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx). A **operação ConvertId** não converte identificadores de pasta pública do identificador EWS para o identificador do armazenamento. 
    
- O Outlook Web App identificador. Isso é representado pelo valor  `OwaId` de enumeração em [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)
    
    Não há suporte para a passagem de URLs criadas a partir desse identificador para Outlook Web App. O Outlook Web App é aplicável ao Exchange 2007 e Exchange 2010. Outlook Web App para Exchange Online e versões do Exchange a partir do Exchange Server 2013 usa identificadores EWS.
    
A **operação ConvertId** não funciona conforme o esperado ao converter identificadores de pasta pública do identificador EWS para o identificador da loja no Exchange Online e Exchange 2013. Você pode atualizar manualmente o identificador retornado como uma solução alternativa. Para atualizar manualmente o identificador: 
  
1. No código do aplicativo, determine se o item/pasta de destino está em uma pasta pública. 
    
2. Decodificar a cadeia de caracteres de identificador codificado por Base64.
    
3. Verifique se o tipo byte (21st byte) tem um valor 7. Um valor 7 indica que o identificador está no formato incorreto.
    
4. Ignore os quatro primeiros bytes. Eles devem ser definidos como zero.
    
5. Atualize os próximos 16 bytes com o seguinte GUID: 1A447390AAA6611CD9BC800AAA002FC45A
    
6. Atualize o próximo byte (tipo byte) com um valor 9.
    
7. Altere o identificador para uma cadeia de caracteres codificada com Base64.
    
> [!NOTE]
> A **operação ConvertId** valida que um determinado endereço SMTP tem um formato válido. A operação não determina se um endereço SMTP representa uma caixa de correio válida. 
  
A **operação ConvertId** pode usar os headers SOAP listados na tabela a seguir. 
  
**Tabela 1. Headers SOAP da operação ConvertId**

|**Header**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|Representação  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Isso é aplicável a uma solicitação.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação Isso é aplicável a uma solicitação.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Isso é aplicável a uma resposta.  <br/> |
   
## <a name="convertid-operation-request-example"></a>Exemplo de solicitação de operação ConvertId
<a name="bk_usingConvertId"> </a>

O exemplo a seguir de **uma solicitação ConvertId** mostra como converter de um identificador EWS para um Outlook Web App identificador. 
  
O [elemento RequestServerVersion](requestserverversion.md) no header SOAP deve ser definido como Exchange2007_SP1 ou posterior para que essa operação funcione. 
  
> [!NOTE]
> O identificador de item foi reduzido para preservar a capacidade de leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <ConvertId xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               DestinationFormat="OwaId">
      <SourceIds>
        <t:AlternateId Format="EwsId" Id="AAMkAGZhN2IxYTA0LWNiNzItN="
                       Mailbox="user1@example.com"/>
      </SourceIds>
    </ConvertId>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-response-example"></a>Exemplo de resposta de operação ConvertId
<a name="bk_usingConvertId"> </a>

O exemplo a seguir mostra uma resposta bem-sucedida a uma **solicitação ConvertId.** Este exemplo de resposta contém um Outlook Web App identificador. 
  
> [!NOTE]
> O Outlook Web App identificador foi reduzido para preservar a capacidade de leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                         MajorBuildNumber="191" MinorBuildNumber="0" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <ConvertIdResponseMessage ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <AlternateId xsi:type="t:AlternateIdType" Format="OwaId" Id="RgAAAAAS2%2" 
                         Mailbox="user@example.com" />
        </ConvertIdResponseMessage>
      </ResponseMessages>
    </ConvertIdResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-error-response-example"></a>Exemplo de resposta de erro de operação ConvertId
<a name="bk_usingConvertId"> </a>

O exemplo a seguir mostra a resposta a uma solicitação que contém o tipo de identificador errado.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                       MajorBuildNumber="206" MinorBuildNumber="0"
                       Version="Exchange2010" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <ConvertIdResponseMessage ResponseClass="Error">
          <MessageText>Id is malformed.</MessageText>
          <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
          <DescriptiveLinkKey>0</DescriptiveLinkKey>
        </ConvertIdResponseMessage>
      </ResponseMessages>
    </ConvertIdResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="version-differences"></a>Diferenças de versão
<a name="bk_ConvertIdVersionDiff"> </a>

O formato do identificador EWS foi alterado entre a versão inicial do Exchange 2007 e Exchange 2007 Service Pack 1 (SP1). Exchange Online como parte das versões Office 365, Exchange Online e local do Exchange a partir do Exchange 2010 usam o mesmo formato identificador que o Exchange 2007 SP1 usa.
  
A **operação ConvertId** converte identificadores de pasta pública do identificador EWS para o identificador do armazenamento no Exchange 2007 e Exchange 2010. 
  
## <a name="see-also"></a>Confira também
<a name="bk_ConvertIdVersionDiff"> </a>

- [Convertendo identificadores](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [ConvertIdType](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [ConvertId](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

