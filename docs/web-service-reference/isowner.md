---
title: IsOwner
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ea0f0afc-32fe-46cb-8530-62a6ce9490f6
description: O elemento IsOwner especifica se o usuário de email especificado é o proprietário.
ms.openlocfilehash: 7e3baaf0f3fb2eac028117622eedd57088d71612
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541004"
---
# <a name="isowner"></a>IsOwner

O **elemento IsOwner** especifica se o usuário de email especificado é o proprietário. 
  
```XML
<IsOwner>true | false</IsOwner>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RightsManagementLicenseData](rightsmanagementlicensedata.md) <br/> |Especifica informações sobre a licença de gerenciamento de direitos.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para o **elemento IsOwner** indica que o usuário é o proprietário dos direitos emitidos em um item. Um valor **false** indica que o usuário não é o proprietário dos direitos emitidos em um item. 
  
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

