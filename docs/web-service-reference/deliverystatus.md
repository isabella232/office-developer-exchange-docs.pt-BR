---
title: DeliveryStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeliveryStatus
api_type:
- schema
ms.assetid: eab55db3-affb-42be-a586-5caa04052433
description: O elemento DeliveryStatus especifica o status de uma mensagem.
ms.openlocfilehash: f11952f401e0d22d780725598bfb32cbd3a8d622
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543384"
---
# <a name="deliverystatus"></a>DeliveryStatus

O **elemento DeliveryStatus** especifica o status de uma mensagem. 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 **MessageTrackingDeliveryStatusType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |Contém informações de um único evento para um destinatário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores de texto possíveis para o **elemento DeliveryStatus.** 
  
**Valores do elemento DeliveryStatus**

|**Valor**|**Descrição**|
|:-----|:-----|
|Malsucedido  <br/> |Especifica que uma mensagem não foi entregue.  <br/> |
|Pendente  <br/> |Especifica que a mensagem está aguardando aprovação de um moderador.  <br/> |
|Entregue  <br/> |Especifica que a mensagem foi entregue a todos os destinatários especificados.  <br/> |
|Transferido  <br/> |Especifica que a mensagem foi transferida para um servidor fora do escopo de pesquisa.  <br/> |
|Ler  <br/> |Especifica que a mensagem foi entregue e lida pelos destinatários.  <br/> |
   
## <a name="remarks"></a>Comentários

O **elemento DeliveryStatus** era do tipo **MessageTrackingDeliveryStatusType** no Exchange Server 2010. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

