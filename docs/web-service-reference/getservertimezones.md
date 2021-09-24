---
title: GetServerTimeZones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetServerTimeZones
api_type:
- schema
ms.assetid: 2a89098b-d89b-4d01-827b-50be00f7cbe9
description: O elemento GetServerTimeZones é o elemento raiz de uma solicitação para recuperar definições de fuso horário do servidor Exchange.
ms.openlocfilehash: b710334e5778f8bc27ba7ac07c6bf9c2e2d3392e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533536"
---
# <a name="getservertimezones"></a>GetServerTimeZones

O **elemento GetServerTimeZones** é o elemento raiz em uma solicitação para recuperar definições de fuso horário do servidor Exchange. 
  
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
|**true** <br/> |Retorne as definições completas para cada fuso horário.  <br/> |
|**false** <br/> |Retorne apenas o nome e o identificador para cada fuso horário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Ids](ids.md) <br/> |Contém uma matriz de identificadores de definição de fuso horário que especifica as definições de fuso horário solicitadas. Esse elemento é opcional. Se esse elemento não estiver incluído na solicitação de operação [GetServerTimeZones,](getservertimezones-operation.md) todas as definições de fuso horário disponíveis no servidor serão retornadas na resposta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada.
  
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

