---
title: ExternalAudience
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExternalAudience
api_type:
- schema
ms.assetid: 79dc2a4c-f7dd-46d1-8f31-149116e1f76e
description: O elemento ExternalAudience define ou contém um valor que determina para quem as mensagens externas fora do Office (OOF) são enviadas.
ms.openlocfilehash: da318bfcf4a43d880b86379364c6e40aa9861f83
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545136"
---
# <a name="externalaudience"></a>ExternalAudience

O **elemento ExternalAudience** define ou contém um valor que determina para quem mensagens externas fora de Office (OOF) são enviadas. 
  
```xml
<ExternalAudience>None or Known or All</ExternalAudience>
```

 **ExternalAudience**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UserOofSettings](useroofsettings.md) <br/> |Especifica as configurações OOF.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[OofSettings](oofsettings.md) <br/> |Contém as configurações OOF.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário para esse elemento. A tabela a seguir lista os valores possíveis para esse elemento.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|**Nenhum** <br/> |Os destinatários de email fora da organização do usuário da caixa de correio que enviam mensagens para o usuário não receberão uma resposta de mensagem OOF externa.  <br/> |
|**Known** <br/> |Os remetentes de email fora da organização do usuário da caixa de correio que enviam mensagens para o usuário receberão apenas uma resposta de mensagem OOF externa se o remetente estiver na lista de contatos do Exchange store do usuário.  <br/> |
|**Tudo** <br/> |Os destinatários de email fora da organização do usuário da caixa de correio que enviam mensagens para o usuário receberão uma resposta de mensagem OOF externa.  <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento compartilha o mesmo tipo que o [elemento AllowExternalOof.](allowexternaloof.md) 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="example"></a>Exemplo

O exemplo a seguir de uma solicitação SetUserOofSettings define o OoFState como **Habilitado**, define o público externo como Todos **,** define a duração do OOF como 10 dias e define as mensagens OOF internas e externas.
  
```
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



[Operação GetUserOofSettings](getuseroofsettings-operation.md)
  
[Operação SetUserOofSettings](setuseroofsettings-operation.md)

