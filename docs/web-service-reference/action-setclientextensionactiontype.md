---
title: Ação (SetClientExtensionActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5624a87-3436-40ce-8d6b-cc01eecab64d
description: O elemento Action contém a ação que o Exchange server deve ser adotada em um aplicativo.
ms.openlocfilehash: a231cedfa6e4759dabfcbecfbe9a9b851f834247
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751041"
---
# <a name="action-setclientextensionactiontype"></a>Ação (SetClientExtensionActionType)

O elemento **Action** contém a ação que o Exchange server deve ser adotada em um aplicativo. 
  
```XML
<Action ActionId="" ExtensionId="">
   <ClientExtension/>
</Action>
```

 **SetClientExtensionActionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|ActionId  <br/> |Especifica o identificador da ação. Este atributo é necessário.  <br/> |
|ExtensionId  <br/> |Especifica o identificador da extensão. Este atributo é opcional.  <br/> |
   
#### <a name="actionid"></a>ActionId

|**Valor**|**Descrição**|
|:-----|:-----|
|Configurar  <br/> |Indica uma ação de configuração.  <br/> |
|Instalar  <br/> |Indica uma ação de instalação.  <br/> |
|Desinstalar  <br/> |Indica uma ação de desinstalação.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ClientExtension](clientextension.md) <br/> |Contém informações de usuário e de configuração sobre um aplicativo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Ações (ArrayOfSetClientExtensionActionsType)](actions-arrayofsetclientextensionactionstype.md) <br/> |Especifica uma matriz de elementos de **ação** .  <br/> |
   
## <a name="remarks"></a>Coment�rios

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

