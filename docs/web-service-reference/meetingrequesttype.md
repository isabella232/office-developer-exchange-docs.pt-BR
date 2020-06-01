---
title: MeetingRequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingRequestType
api_type:
- schema
ms.assetid: bcd5c97c-19aa-4b1d-a8e8-e8c4bd473dd9
description: O elemento MeetingRequestType descreve o tipo da solicitação de reunião.
ms.openlocfilehash: e90c44dd4124d698ca5ef7655f6429a7167673e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44465783"
---
# <a name="meetingrequesttype"></a>MeetingRequestType

O elemento **MeetingRequestType** descreve o tipo da solicitação de reunião. 
  
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
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no repositório do Exchange.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. A tabela a seguir lista os valores de texto possíveis para este elemento.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|FullUpdate  <br/> |Identifica a solicitação de reunião como uma atualização completa para uma solicitação existente. Uma atualização completa atualizou o tempo e o conteúdo informativo.  <br/> |
|InformationalUpdate  <br/> |Identifica a solicitação de reunião como somente com conteúdo atualizado de informações.  <br/> |
|NewMeetingRequest  <br/> |Identifica a solicitação de reunião como uma nova solicitação de reunião.  <br/> |
|Nenhum  <br/> |Indica que o tipo de solicitação de reunião não está definido.  <br/> |
|Atualizados  <br/> |Identifica a solicitação de reunião como desatualizada.  <br/> |
|PrincipalWantsCopy  <br/> |Indica que a solicitação de reunião pertence a uma entidade de segurança que encaminhou mensagens de reunião para um representante e tem suas cópias marcadas como informativas.  <br/> |
|SilentUpdate  <br/> |Identifica a solicitação de reunião como uma atualização silenciosa para uma reunião existente.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

