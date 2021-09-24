---
title: UserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UserOofSettings
api_type:
- schema
ms.assetid: 0a95ca63-660e-4cc0-82e4-3f74fb4ae21c
description: O elemento UserOofSettings especifica as configurações Out of Office (OOF).
ms.openlocfilehash: 0fa550a97464414570faf391d3633243ff2e2144
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513966"
---
# <a name="useroofsettings"></a>UserOofSettings

O **elemento UserOofSettings** especifica as configurações Out of Office (OOF). 
  
[SetUserOofSettingsRequest](setuseroofsettingsrequest.md)
  
[UserOofSettings](useroofsettings.md)
  
```xml
<UserOofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</UserOofSettings>
```

 **UserOofSettings**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OofState](oofstate.md) <br/> |Define o estado OOF do usuário.  <br/> |
|[ExternalAudience](externalaudience.md) <br/> |Define ou contém um valor que determina para quem as mensagens OOF externas são enviadas.  <br/> |
|[Duration (UserOofSettings)](duration-useroofsettings.md) <br/> |Especifica a duração para a qual o status OOF está habilitado se o [elemento OofState](oofstate.md) estiver definido como **Scheduled**. Se o [elemento OofState](oofstate.md) estiver definido como **Habilitado** ou **Desabilitado,** o valor desse elemento será ignorado.  <br/> |
|[InternalReply](internalreply.md) <br/> |Contém a resposta OOF enviada a outros usuários no domínio do usuário ou domínios confiáveis.  <br/> |
|[ExternalReply](externalreply.md) <br/> |Contém a resposta OOF enviada a endereços fora do domínio do destinatário ou domínios confiáveis.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SetUserOofSettingsRequest](setuseroofsettingsrequest.md) <br/> |Contém os argumentos usados para definir as configurações e mensagens OOF de um usuário de caixa de correio.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="example"></a>Exemplo

O exemplo a seguir de uma solicitação SetUserOofSettings define o OoFState como **Habilitado**, define a duração do OOF para 10 dias e define as mensagens OOF internas e externas.
  
```xml
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
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação SetUserOofSettings](setuseroofsettings-operation.md)

