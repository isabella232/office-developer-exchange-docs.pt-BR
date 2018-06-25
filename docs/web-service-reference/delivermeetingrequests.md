---
title: DeliverMeetingRequests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliverMeetingRequests
api_type:
- schema
ms.assetid: 04b999af-0b27-4e6d-a8b1-400955a1afaa
description: O elemento de DeliverMeetingRequests define como as solicitações de reunião são manipuladas entre o delegado e a entidade. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 803bd2da72bdb21b507a59cc11635a40d4431acf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751773"
---
# <a name="delivermeetingrequests"></a>DeliverMeetingRequests

O elemento de **DeliverMeetingRequests** define como as solicitações de reunião são manipuladas entre o delegado e a entidade. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```XML
<DeliverMeetingRequests>DelegatesOnly or DelegatesAndMe or DelegatesAndSendInformationToMe or NoForward</DeliverMeetingRequests>
```

 **DeliverMeetingRequestsType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AddDelegate](adddelegate.md) <br/> |Define uma solicitação para adicionar representantes para uma caixa de correio. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Define uma solicitação de atualização de representantes em uma caixa de correio. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Contém o status e o resultado de uma solicitação de GetDelegate. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Text value

A tabela a seguir lista os valores possíveis para o elemento **DeliverMeetingRequests** . 
  
**Valores de elemento DeliverMeetingRequests**

|**Valor**|**Descrição**|
|:-----|:-----|
|DelegatesOnly  <br/> |Solicitações de reunião são encaminhadas para o representante e movidas para a pasta Itens excluídos na caixa de correio do principal.  <br/> |
|DelegatesAndMe  <br/> |Solicitações de reunião são encaminhadas para o representante e permanecem na pasta caixa de entrada na caixa de correio do principal.  <br/> |
|DelegatesAndSendInformationToMe  <br/> |Solicitações de reunião são encaminhadas para o representante e permanecem na pasta caixa de entrada na caixa de correio da entidade de segurança, mas os botões de aceitar, recusar e provisório não aparecem no painel de leitura do Microsoft Office Outlook.  <br/> |
|NoForward  <br/> |Solicitações de reunião não são encaminhadas para o representante.  <br/> |
   
## <a name="remarks"></a>Comentários

A configuração de **DeliverMeetingRequests** afeta todos os delegados na caixa de correio da entidade de segurança. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação AddDelegate](adddelegate-operation.md)  
- [Operação UpdateDelegate](updatedelegate-operation.md)  
- [Operação GetDelegate](getdelegate-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Adicionando representantes](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

