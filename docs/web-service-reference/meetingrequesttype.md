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
description: O elemento MeetingRequestType descreve o tipo de solicitação de reunião.
ms.openlocfilehash: 7269587e2fa72aeb9070a7b53ee9215829729329
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824432"
---
# <a name="meetingrequesttype"></a>MeetingRequestType

O elemento **MeetingRequestType** descreve o tipo de solicitação de reunião. 
  
```xml
<MeetingRequestType/>
```

 **MeetingRequestTypeType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no armazenamento do Exchange.  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. A tabela a seguir lista os valores de texto possíveis para esse elemento.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|FullUpdate  <br/> |Identifica a solicitação de reunião como uma atualização completa para uma solicitação existente. Uma atualização completa atualizou o tempo e o conteúdo informativo.  <br/> |
|InformationalUpdate  <br/> |Identifica a solicitação de reunião como contendo apenas atualizados conteúdo informativo.  <br/> |
|NewMeetingRequest  <br/> |Identifica a solicitação de reunião como uma nova solicitação de reunião.  <br/> |
|None  <br/> |Indica o tipo de solicitação de reunião não está definido.  <br/> |
|Desatualizadas  <br/> |Identifica a solicitação de reunião como desatualizados.  <br/> |
|PrincipalWantsCopy  <br/> |Indica que a solicitação de reunião pertence a uma entidade de segurança que tem encaminhadas mensagens de reunião para um representante e tem suas cópias marcadas como informativas.  <br/> |
|SilentUpdate  <br/> |Identifica a solicitação de reunião como uma atualização silenciosa a uma reunião existente.  <br/> |
   
## <a name="remarks"></a>Coment�rios

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

