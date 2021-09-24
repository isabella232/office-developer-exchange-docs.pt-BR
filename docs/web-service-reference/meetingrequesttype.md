---
title: MeetingRequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MeetingRequestType
api_type:
- schema
ms.assetid: bcd5c97c-19aa-4b1d-a8e8-e8c4bd473dd9
description: O elemento MeetingRequestType descreve o tipo da solicitação de reunião.
ms.openlocfilehash: 1a8371331691bb9dee5595b0130ec0c3c75c47c5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539371"
---
# <a name="meetingrequesttype"></a>MeetingRequestType

O **elemento MeetingRequestType** descreve o tipo da solicitação de reunião. 
  
```xml
<MeetingRequestType/>
```

 **MeetingRequestTypeType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. A tabela a seguir lista os valores de texto possíveis para esse elemento.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|FullUpdate  <br/> |Identifica a solicitação de reunião como uma atualização completa de uma solicitação existente. Uma atualização completa atualizou o tempo e o conteúdo informacional.  <br/> |
|InformationalUpdate  <br/> |Identifica a solicitação de reunião como apenas contendo conteúdo informacional atualizado.  <br/> |
|NewMeetingRequest  <br/> |Identifica a solicitação de reunião como uma nova solicitação de reunião.  <br/> |
|Nenhum  <br/> |Indica que o tipo de solicitação de reunião não está definido.  <br/> |
|Desatualizado  <br/> |Identifica a solicitação de reunião como desatualizada.  <br/> |
|PrincipalWantsCopy  <br/> |Indica que a solicitação de reunião pertence a uma entidade que encaminhou mensagens de reunião para um representante e tem suas cópias marcadas como informativas.  <br/> |
|SilentUpdate  <br/> |Identifica a solicitação de reunião como uma atualização silenciosa para uma reunião existente.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2010 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

