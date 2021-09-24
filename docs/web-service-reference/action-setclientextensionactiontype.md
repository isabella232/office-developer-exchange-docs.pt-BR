---
title: Action (SetClientExtensionActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c5624a87-3436-40ce-8d6b-cc01eecab64d
description: O elemento Action contém a ação que o Exchange servidor deve tomar em um aplicativo.
ms.openlocfilehash: a0f5c2743ef976db2faddbb7509a8a015ef4dd8f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510376"
---
# <a name="action-setclientextensionactiontype"></a>Action (SetClientExtensionActionType)

O **elemento Action** contém a ação que o Exchange servidor deve tomar em um aplicativo. 
  
```XML
<Action ActionId="" ExtensionId="">
   <ClientExtension/>
</Action>
```

 **SetClientExtensionActionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|ActionId  <br/> |Especifica o identificador da ação. Esse atributo é necessário.  <br/> |
|ExtensionId  <br/> |Especifica o identificador da extensão. Esse atributo é opcional.  <br/> |
   
#### <a name="actionid"></a>ActionId

|**Valor**|**Descrição**|
|:-----|:-----|
|Configurar  <br/> |Indica uma ação de configuração.  <br/> |
|Instalar  <br/> |Indica uma ação de instalação.  <br/> |
|Desinstalar  <br/> |Indica uma ação de desinstalação.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ClientExtension](clientextension.md) <br/> |Contém informações de usuário e configuração sobre um aplicativo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Actions (ArrayOfSetClientExtensionActionsType)](actions-arrayofsetclientextensionactionstype.md) <br/> |Especifica uma matriz de **elementos Action.**  <br/> |
   
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

