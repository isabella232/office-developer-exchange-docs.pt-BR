---
title: GetServerTimeZones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZones
api_type:
- schema
ms.assetid: 2a89098b-d89b-4d01-827b-50be00f7cbe9
description: O elemento GetServerTimeZones é o elemento raiz em uma solicitação para recuperar definições de fuso horário do Exchange Server.
ms.openlocfilehash: 797e4543c94b0628242bcf544fe9a735ebaa5a63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460936"
---
# <a name="getservertimezones"></a>GetServerTimeZones

O elemento **GetServerTimeZones** é o elemento raiz em uma solicitação para recuperar definições de fuso horário do Exchange Server. 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 **GetServerTimeZonesType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ReturnFullTimeZoneData** <br/> |Especifica se a [operação GetServerTimeZones](getservertimezones-operation.md) retorna a definição completa ou apenas o nome e o identificador de cada fuso horário. Esse atributo é opcional. O valor padrão é **true**.  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a>Atributo ReturnFullTimeZoneData

|**Valor**|**Descrição**|
|:-----|:-----|
|**verdadeiro** <br/> |Retorna as definições completas de cada fuso horário.  <br/> |
|**false** <br/> |Retornar apenas o nome e o identificador de cada fuso horário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Código](ids.md) <br/> |Contém uma matriz de identificadores de definição de fuso horário que especifica as definições de fuso horário solicitadas. Este elemento é opcional. Se esse elemento não estiver incluído na solicitação de [operação GetServerTimeZones](getservertimezones-operation.md) , todas as definições de fuso horário disponíveis no servidor serão retornadas na resposta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetServerTimeZones](getservertimezones-operation.md)
  
[GetServerTimeZonesResponse](getservertimezonesresponse.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

