---
title: Operação convertid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 47d96cf6-9e2f-4fc0-9682-7258d3fbf918
description: Encontre informações sobre a operação convertid do EWS.
ms.openlocfilehash: 36bd47d3fc7c7ca7cea7b38222abb25fba6074ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452549"
---
# <a name="convertid-operation"></a>Operação convertid

Encontre informações sobre a operação **convertid** do EWS. 
  
A operação **convertid** de serviços Web do Exchange (EWS) converte os identificadores de item e pasta entre os formatos aceitos pelo Exchange Online, o Exchange Online como parte do Office 365 e as versões locais do Exchange a partir do exchange server 2013. 
  
## <a name="using-the-convertid-operation"></a>Usando a operação convertid
<a name="bk_usingConvertId"> </a>

Você pode converter os seguintes identificadores usando a operação **convertid** : 
  
- O formato do identificador para EWS na versão inicial do Exchange 2007. Isso é representado pelo `EwsLegacyId` valor de enumeração na enumeração [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) . 
    
- O formato do identificador para EWS no Exchange 2007 SP1 ou no Exchange 2010. Isso é representado pelo `EwsId` valor de enumeração no [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- O identificador MAPI, como na propriedade **PR_ENTRYID** . Isso é representado pelo `EntryId` valor de enumeração na enumeração [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) . 
    
- O identificador de eventos do calendário de disponibilidade. Esta é uma representação codificada em hexadecimal da propriedade **PR_ENTRYID** . Isso é representado pelo `HexEntryId` valor de enumeração no [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- O identificador do repositório do Exchange. Isso é representado pelo `StoreId` valor de enumeração no [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx). A operação **convertid** não converte identificadores de pasta pública do identificador EWS no identificador de repositório. 
    
- O identificador do Outlook Web App. Isso é representado pelo `OwaId` valor de enumeração no [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)
    
    Não há suporte para a passagem de URLs criadas a partir deste identificador para o Outlook Web App. O identificador do Outlook Web App é aplicável ao Exchange 2007 e ao Exchange 2010. Outlook Web App para Exchange Online e versões do Exchange a partir do Exchange Server 2013 usa identificadores EWS.
    
A operação **convertid** não funciona como esperado ao converter identificadores de pasta pública do identificador EWS para o identificador de repositório no Exchange Online e no Exchange 2013. Você pode atualizar manualmente o identificador que é retornado como uma solução alternativa. Para atualizar manualmente o identificador: 
  
1. No código do aplicativo, determine se o item/pasta de destino está em uma pasta pública. 
    
2. Decodifique a cadeia de caracteres do identificador codificado em base64.
    
3. Verifique se o byte de tipo (21 byte) tem um valor de 7. O valor 7 indica que o identificador está no formato incorreto.
    
4. Pule os primeiros quatro bytes. Eles devem ser definidos como zero.
    
5. Atualize os próximos 16 bytes com o seguinte GUID: 1A447390AA6611CD9BC800AA002FC45A
    
6. Atualize o próximo byte (tipo Byte) com um valor de 9.
    
7. Altere o identificador para uma cadeia de caracteres codificada em base64.
    
> [!NOTE]
> A operação **convertid** valida que um determinado endereço SMTP tem um formato válido. A operação não determina se um endereço SMTP representa uma caixa de correio válida. 
  
A operação **convertid** pode usar os cabeçalhos SOAP listados na tabela a seguir. 
  
**Tabela 1. Cabeçalhos SOAP da operação convertid**

|**Header**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|Representação  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Isso se aplica a uma solicitação.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação isso se aplica a uma solicitação.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Isso se aplica a uma resposta.  <br/> |
   
## <a name="convertid-operation-request-example"></a>Exemplo de solicitação de operação convertid
<a name="bk_usingConvertId"> </a>

O exemplo a seguir de uma solicitação **convertid** mostra como converter de um identificador EWS para um identificador do Outlook Web App. 
  
O elemento [RequestServerVersion](requestserverversion.md) no cabeçalho SOAP deve ser definido como Exchange2007_SP1 ou posterior para que essa operação funcione. 
  
> [!NOTE]
> O identificador de item foi reduzido para preservar a legibilidade. 
  
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

## <a name="convertid-operation-response-example"></a>Exemplo de resposta de convertid
<a name="bk_usingConvertId"> </a>

O exemplo a seguir mostra uma resposta bem-sucedida para uma solicitação **convertid** . Este exemplo de resposta contém um identificador do Outlook Web App. 
  
> [!NOTE]
> O identificador do Outlook Web App foi reduzido para preservar a legibilidade. 
  
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

## <a name="convertid-operation-error-response-example"></a>Exemplo de resposta de erro de operação convertid
<a name="bk_usingConvertId"> </a>

O exemplo a seguir mostra a resposta a uma solicitação que contém o tipo incorreto de formato de identificador.
  
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

O formato do identificador EWS foi alterado entre a versão inicial do Exchange 2007 e do Exchange 2007 Service Pack 1 (SP1). O Exchange Online como parte do Office 365, do Exchange Online e das versões locais do Exchange a partir do Exchange 2010 usam o mesmo formato de identificador que o Exchange 2007 SP1 usa.
  
A operação **convertid** converte identificadores de pasta pública do identificador do EWS para o identificador de repositório no Exchange 2007 e no Exchange 2010. 
  
## <a name="see-also"></a>Confira também
<a name="bk_ConvertIdVersionDiff"> </a>

- [Convertendo identificadores](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [ConvertIdType](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [ConvertId](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

