---
title: Duration (UserOofSettings)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Duration
api_type:
- schema
ms.assetid: 01d67af3-658e-4acd-93e3-441ae827fdd3
description: O elemento Duration especifica a duração em que o status OOF está habilitado se o elemento OofState estiver definido como Scheduled.
ms.openlocfilehash: cb6529bfe3799ff41550d7fe3ce2c79b8a4197e2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544154"
---
# <a name="duration-useroofsettings"></a>Duration (UserOofSettings)

O **elemento Duration** especifica a duração em que o status OOF está habilitado se o elemento [OofState](oofstate.md) estiver definido como **Scheduled**.
  
```XML
<Duration>
   <StartTime/>
   <EndTime/> 
</Duration>
```

 **Duration**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StartTime](starttime.md) <br/> |Representa o início do conjunto de intervalos de tempo com um status OOF. Este elemento é obrigatório.  <br/> |
|[EndTime](endtime.md) <br/> |Representa o fim do conjunto de intervalos de tempo com um status OOF. Este elemento é obrigatório.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UserOofSettings](useroofsettings.md) <br/> |Especifica as configurações OOF.  <br/><br/>Veja a seguir a expressão XPath para este elemento:<br/><br/>`/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[OofSettings](oofsettings.md) <br/> |Contém as configurações OOF.<br/><br/>Veja a seguir a expressão XPath para este elemento:<br/><br/>`/GetUserOofSettingsResponse/OofSettings` <br/> |
|[OutOfOffice](outofoffice.md) <br/> |Define a mensagem de resposta Out of Office (OOF) e um tempo de duração para enviar a mensagem de resposta para uma caixa de correio.  <br/> |
   
## <a name="remarks"></a>Comentários

O **tipo Duration** também é o tipo para os elementos [DetailedSuggestionsWindow,](detailedsuggestionswindow.md) [TimeWindow](timewindow.md)e [OutOfOffice.](outofoffice.md) 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="example"></a>Exemplo

O exemplo a seguir de uma solicitação de operação [SetUserOofSettings](setuseroofsettings-operation.md) define o [OofState](oofstate.md) como **Enabled**, as mensagens OOF internas e externas e define a duração do OOF por 10 dias.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserOofSettings](getuseroofsettings-operation.md)  
- [Operação SetUserOofSettings](setuseroofsettings-operation.md)

