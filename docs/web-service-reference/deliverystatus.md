---
title: DeliveryStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliveryStatus
api_type:
- schema
ms.assetid: eab55db3-affb-42be-a586-5caa04052433
description: O elemento DeliveryStatus Especifica o status de uma mensagem.
ms.openlocfilehash: 4e6f31e8ef4f98d8e838ba91167c7dd5d6ab2590
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751774"
---
# <a name="deliverystatus"></a>DeliveryStatus

O elemento **DeliveryStatus** Especifica o status de uma mensagem. 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 **MessageTrackingDeliveryStatusType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |Contém informações para um único evento de um destinatário.  <br/> |
   
## <a name="text-value"></a>Text value

A tabela a seguir lista os valores de texto possíveis para o elemento **DeliveryStatus** . 
  
**Valores de elemento DeliveryStatus**

|**Valor**|**Descrição**|
|:-----|:-----|
|Sem êxito  <br/> |Especifica que uma mensagem não foi entregue.  <br/> |
|Pendente  <br/> |Especifica que a mensagem está aguardando aprovação do moderador.  <br/> |
|Entregue  <br/> |Especifica que a mensagem foi entregue a todos os destinatários especificados.  <br/> |
|Transferido  <br/> |Especifica que a mensagem foi transferida para um servidor fora do escopo de pesquisa.  <br/> |
|Ler  <br/> |Especifica que a mensagem foi entregue e leia pelos destinatários.  <br/> |
   
## <a name="remarks"></a>Coment�rios

O elemento **DeliveryStatus** era do tipo **MessageTrackingDeliveryStatusType** no Exchange Server 2010. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

