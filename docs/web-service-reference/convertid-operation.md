---
title: Operação ConvertId
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
description: Encontre informações sobre o EWS ConvertId operação.
ms.openlocfilehash: 5f1bcd8a9f0adc25b7c598ef10cc6bb139dfe02d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751536"
---
# <a name="convertid-operation"></a>Operação ConvertId

Encontre informações sobre a operação de EWS **ConvertId** . 
  
A operação de serviços Web do Exchange (EWS) **ConvertId** converte identificadores de item e pasta entre formatos que são aceitos pelo Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange, começando com o Exchange Server no local 2013. 
  
## <a name="using-the-convertid-operation"></a>Usando a operação ConvertId
<a name="bk_usingConvertId"> </a>

Você pode converter os seguintes identificadores usando a operação **ConvertId** : 
  
- O formato do identificador de EWS na versão inicial do Exchange 2007. Isso é representado pelo `EwsLegacyId` valor de enumeração na enumeração [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) . 
    
- O formato do identificador de EWS no Exchange 2007 SP1 ou Exchange 2010. Isso é representado pelo `EwsId` valor de enumeração em [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- O identificador MAPI, como a propriedade **PR_ENTRYID** . Isso é representado pelo `EntryId` valor de enumeração na enumeração [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) . 
    
- O identificador de eventos de calendário de disponibilidade. Esta é uma representação hexadecimal codificado da propriedade **PR_ENTRYID** . Isso é representado pelo `HexEntryId` valor de enumeração em [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).
    
- O identificador de repositório do Exchange. Isso é representado pelo `StoreId` valor de enumeração em [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx). A operação **ConvertId** não converte os identificadores de pasta pública do identificador EWS para o identificador do repositório. 
    
- O identificador do Outlook Web App. Isso é representado pelo `OwaId` valor de enumeração em [IdFormat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)
    
    Não há suporte para a passagem de URLs que são criados a partir esse identificador para o Outlook Web App. O identificador do Outlook Web App é aplicável para o Exchange 2007 e Exchange 2010. Outlook Web App para Exchange Online e versões do Exchange, começando com o Exchange Server 2013 usa identificadores EWS.
    
A operação **ConvertId** não funciona conforme o esperado, ao converter identificadores de pasta pública o identificador do EWS para o identificador de repositório no Exchange Online e Exchange 2013. Você pode atualizar manualmente o identificador retornado como uma solução alternativa. Para atualizar manualmente o identificador: 
  
1. Em seu código de aplicativo, determine se o item/pasta de destino está em uma pasta pública. 
    
2. Decodificar a sequência identifier codificado na Base64.
    
3. Verificar se o byte tipo (21 de byte) tem o valor 7. O valor 7 indica que o identificador está no formato incorreto.
    
4. Ignore os primeiros quatro bytes. Eles devem ser definidos como zero.
    
5. Atualizar o próximo de 16 bytes com a seguinte GUID: 1A447390AA6611CD9BC800AA002FC45A
    
6. Atualize o próximo byte (tipo byte) com um valor de 9.
    
7. Altere o identificador para uma cadeia de caracteres codificado na Base64.
    
> [!NOTE]
> A operação **ConvertId** valida que um determinado endereço SMTP tem um formato válido. A operação não determinará se um endereço SMTP representa uma caixa de correio válida. 
  
A operação **ConvertId** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir. 
  
**Tabela 1. Cabeçalhos SOAP ConvertId operação**

|**Header**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|Representação  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Isso é aplicável a uma solicitação.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação, que isso é aplicável a uma solicitação.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Isso é aplicável a uma resposta.  <br/> |
   
## <a name="convertid-operation-request-example"></a>Exemplo de solicitação de operação ConvertId
<a name="bk_usingConvertId"> </a>

O exemplo a seguir de uma solicitação de **ConvertId** mostra como converter a partir de um identificador do EWS e um identificador do Outlook Web App. 
  
O elemento [RequestServerVersion](requestserverversion.md) no cabeçalho SOAP deve ser definido como Exchange2007_SP1 ou posterior para esta operação trabalhar. 
  
> [!NOTE]
> O identificador do item foi reduzido para preservar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <ConvertId xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               DestinationFormat="OwaId">
      <SourceIds>
        <t:AlternateId Format="EwsId" Id="AAMkAGZhN2IxYTA0LWNiNzItN="
                       Mailbox="user1@example.com"/>
      </SourceIds>
    </ConvertId>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-response-example"></a>Exemplo de resposta da operação de ConvertId
<a name="bk_usingConvertId"> </a>

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação **ConvertId** . Este exemplo resposta contém um identificador do Outlook Web App. 
  
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
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

O exemplo a seguir mostra a resposta a uma solicitação que contém o tipo de formato de identificador incorreto.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                       MajorBuildNumber="206" MinorBuildNumber="0"
                       Version="Exchange2010" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

O formato de identificador do EWS alterado entre a versão de lançamento inicial do Exchange 2007 e Exchange 2007 Service Pack 1 (SP1). Exchange Online como parte do Office 365, Exchange Online e a versões locais do Exchange, começando com o Exchange 2010 usam o mesmo formato de identificador que usa o Exchange 2007 SP1.
  
A operação **ConvertId** converte os identificadores de pasta pública do identificador do EWS para o identificador de repositório no Exchange 2007 e Exchange 2010. 
  
## <a name="see-also"></a>Confira também
<a name="bk_ConvertIdVersionDiff"> </a>

- [Convertendo identificadores](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [ConvertIdType](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [ConvertId](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

