---
title: AddressListId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a3334bb2-90dc-4fe1-96d9-890b13d9ff30
description: O elemento AddressListId Especifica o identificador de uma lista de endereços.
ms.openlocfilehash: d8a513559b7d127559537b43d7c6c0a4db121702
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751069"
---
# <a name="addresslistid"></a>AddressListId

O elemento **AddressListId** Especifica o identificador de uma lista de endereços. 
  
```XML
<AddressListId Id="">
</AddressListId>
```

 **AddressListIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**ID de** <br/> |Um identificador de lista de endereços de cadeia de caracteres. Este atributo é necessário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Indica a pasta que está programada para ações que usam pastas. Este elemento deve estar presente quando copiar, excluir, mover e definindo o estado lido em itens da conversa em uma pasta de destino.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Especifica o identificador da pasta para o qual os itens de email são copiados.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indica a pasta de destino para cópia e mover ações.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Especifica o identificador da pasta para o qual os itens de email são movidos  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

