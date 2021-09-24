---
title: AddNewTelUriContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: cff8ef19-3e19-4107-9b35-c8a2b87a41bc
description: O elemento AddNewTelUriContactToGroup especifica os dados de entrada para a operação WSDL AddNewTelUriContactToGroup.
ms.openlocfilehash: 0d260679da8ca1ae78afef200f047263808d6e32
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522177"
---
# <a name="addnewteluricontacttogroup"></a>AddNewTelUriContactToGroup

O **elemento AddNewTelUriContactToGroup** especifica os dados de entrada para a operação WSDL **AddNewTelUriContactToGroup.** 
  
```XML
<AddNewTelUriContactToGroup>
   <TelUriAddress/>
   <ImContactSipUriAddress/>
   <ImTelephoneNumber/>
   <GroupId/>
</AddNewTelUriContactToGroup>
```

 **AddNewTelUriContactToGroupType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[TelUriAddress](teluriaddress.md)  |  [ImContactSipUriAddress](imcontactsipuriaddress.md)  |  [ImTelephoneNumber](imtelephonenumber.md)  |  [GroupId](groupid.md)
  
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação AddNewTelUriContactToGroup](addnewteluricontacttogroup-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

