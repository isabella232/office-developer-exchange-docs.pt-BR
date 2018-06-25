---
title: Duração (UserOofSettings)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Duration
api_type:
- schema
ms.assetid: 01d67af3-658e-4acd-93e3-441ae827fdd3
description: O elemento de duração Especifica a duração em que o limite de status de ausência temporária será habilitado se o elemento OofState for definido como agendado.
ms.openlocfilehash: 62a5492372fd80173d58e965376b7c8c466825a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751945"
---
# <a name="duration-useroofsettings"></a>Duração (UserOofSettings)

O elemento de **duração** Especifica a duração em que o limite de status de ausência temporária será habilitado se o elemento [OofState](oofstate.md) for definido como **agendado**.
  
```XML
<Duration>
   <StartTime/>
   <EndTime/> 
</Duration>
```

 **Duração**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StartTime](starttime.md) <br/> |Representa o início do intervalo de tempo definido com um status de ausência temporária. Este elemento é obrigatório.  <br/> |
|[EndTime](endtime.md) <br/> |Representa o fim do intervalo de tempo definido com um status de ausência temporária. Este elemento é obrigatório.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UserOofSettings](useroofsettings.md) <br/> |Especifica as configurações de ausência temporária.  <br/><br/>Este é a expressão XPath para esse elemento:<br/><br/>`/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[OofSettings](oofsettings.md) <br/> |Contém as configurações de ausência temporária.<br/><br/>Este é a expressão XPath para esse elemento:<br/><br/>`/GetUserOofSettingsResponse/OofSettings` <br/> |
|[Fora do escritório](outofoffice.md) <br/> |Define a mensagem de resposta de ausência temporária e um tempo de duração para enviar a mensagem de resposta para uma caixa de correio.  <br/> |
   
## <a name="remarks"></a>Comentários

O tipo de **duração** também é o tipo para os elementos [DetailedSuggestionsWindow](detailedsuggestionswindow.md) [TimeWindow](timewindow.md)e [fora do escritório](outofoffice.md) . 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="example"></a>Exemplo

O exemplo a seguir de uma solicitação de [operação SetUserOofSettings](setuseroofsettings-operation.md) define o [OofState](oofstate.md) como **habilitado**, as mensagens de ausência temporária internas e externas e define a duração de ausência temporária para 10 dias.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2005-10-05T00:00:00</StartTime>
          <EndTime>2005-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
        <SetByLegacyClient>false</SetByLegacyClient>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação GetUserOofSettings](getuseroofsettings-operation.md)  
- [Operação SetUserOofSettings](setuseroofsettings-operation.md)

