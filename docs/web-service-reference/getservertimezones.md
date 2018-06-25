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
description: O GetServerTimeZones é o elemento raiz em uma solicitação para recuperar as definições de fuso horário do servidor Exchange.
ms.openlocfilehash: 1ad503ff312497189f57bce9a3670571aedad5ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752630"
---
# <a name="getservertimezones"></a>GetServerTimeZones

O **GetServerTimeZones** é o elemento raiz em uma solicitação para recuperar as definições de fuso horário do servidor Exchange. 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 **GetServerTimeZonesType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**ReturnFullTimeZoneData** <br/> |Especifica se a [operação GetServerTimeZones](getservertimezones-operation.md) retorna a definição completa ou apenas o nome e o identificador de cada fuso horário. Este atributo é opcional. O valor padrão é **true**.  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a>Atributo ReturnFullTimeZoneData

|**Valor**|**Descrição**|
|:-----|:-----|
|**True** <br/> |Retorne as definições de completas para cada fuso horário.  <br/> |
|**False** <br/> |Retorne somente o nome e o identificador de cada fuso horário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[IDs](ids.md) <br/> |Contém uma matriz de identificadores de definição de fuso horário que especifica as definições de fuso solicitada. Esse elemento é opcional. Se esse elemento não estiver incluído na solicitação de [operação GetServerTimeZones](getservertimezones-operation.md) , todas as definições de fuso horário que estão disponíveis no servidor são retornadas na resposta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetServerTimeZones](getservertimezones-operation.md)
  
[GetServerTimeZonesResponse](getservertimezonesresponse.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

