---
title: AddressListId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: a3334bb2-90dc-4fe1-96d9-890b13d9ff30
description: O elemento AddressListId especifica o identificador de uma lista de endereços.
ms.openlocfilehash: 5348c6877e24fcc0c8873df1098f8a8e30fe4c1c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541557"
---
# <a name="addresslistid"></a>AddressListId

O **elemento AddressListId** especifica o identificador de uma lista de endereços. 
  
```XML
<AddressListId Id="">
</AddressListId>
```

 **AddressListIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Id** <br/> |Um identificador de lista de endereços de cadeia de caracteres. Esse atributo é necessário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Indica a pasta direcionada para ações que usam pastas. Esse elemento deve estar presente ao copiar, excluir, mover e definir o estado de leitura em itens de conversa em uma pasta de destino.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Especifica o identificador da pasta para a qual os itens de email são copiados.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indica a pasta de destino para copiar e mover ações.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Especifica o identificador da pasta para a qual os itens de email são movidos  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Tipo de esquema  <br/> |
|Arquivo de validação  <br/> |types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

