---
title: WebClientReadFormQueryString
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WebClientReadFormQueryString
api_type:
- schema
ms.assetid: 13e8871a-32a6-4bb9-9493-864c4c07efff
description: O elemento WebClientReadFormQueryString representa uma URL para concatenar no ponto de extremidade do Outlook Web App para ler um item no Outlook Web App.
ms.openlocfilehash: 8096c14956d132a631b0ade6f2eae12a2bff9c06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838055"
---
# <a name="webclientreadformquerystring"></a>WebClientReadFormQueryString

O elemento **WebClientReadFormQueryString** representa uma URL para concatenar no ponto de extremidade do Outlook Web App para ler um item no Outlook Web App. 
  
```XML
<WebClientReadFormQueryString/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato do Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[1.1](item.md) <br/> |Representa um item no armazenamento do Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa o cancelamento da reunião no armazenamento do Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no armazenamento do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no armazenamento do Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no armazenamento do Exchange.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Representa um item de postagem no armazenamento do Exchange.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Remove um item de armazenamento do Exchange.  <br/> |
|[Task](task.md) <br/> |Representa uma tarefa no armazenamento do Exchange.  <br/> |
   
## <a name="text-value"></a>Text value

Se este elemento for usado, será necessário um valor de texto que representa uma cadeia de caracteres.
  
## <a name="remarks"></a>Comentários

O identificador do item de um URL do Outlook Web App é o identificador do EWS do item. Você pode codificar o URL o identificador de item do EWS e acrescentá-la para a cadeia de caracteres de consulta para obter a URL do Outlook Web App para um item.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
### <a name="version-differences"></a>Diferenças de versão

Versões do Exchange, começando com a versão principal 15 e terminando com o Exchange Server 2013 build 15.0.775.38 (CU3) e o Exchange Online versão 15.00.0775.009 não retornam um fragmento de cadeia de caracteres de consulta correta no elemento **WebClientReadFormQueryString** . 
  
Em versões anteriores à versão principal 15 do Exchange, o identificador do item para as URLs do Outlook Web App é um identificador do Outlook Web App. Se você está direcionando uma versão do Exchange anterior à versão principal 15, você precisa usar a [operação ConvertId](convertid-operation.md) para converter o identificador. 
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

