---
title: ExchangeStoreId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5acceb42-a757-4c74-ab1c-b1abf7bf1e0a
description: O elemento ExchangeStoreId especifica o identificador de grupo de mensagens instantâneas (IM).
ms.openlocfilehash: dba2d97fa135583efd70ec6d555b71f356282728
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513798"
---
# <a name="exchangestoreid"></a>ExchangeStoreId

O **elemento ExchangeStoreId** especifica o identificador de grupo de mensagens instantâneas (IM). 
  
```XML
<ExchangeStoreId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Id  <br/> |O valor de texto do **atributo Id** é o identificador do grupo.  <br/> |
|ChangeKey  <br/> |O valor de texto do **atributo ChangeKey** é a chave de alteração do grupo.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ImGroup](imgroup.md) <br/> |Representa um grupo de mensagens instantâneas.  <br/> |
   
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

