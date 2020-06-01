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
description: O elemento DeliverMeetingRequests define como as solicitações de reunião são tratadas entre o representante e a entidade de segurança. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 3998443613437bca2267678f7bc2c5584b779135
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463675"
---
# <a name="delivermeetingrequests"></a>DeliverMeetingRequests

O elemento **DeliverMeetingRequests** define como as solicitações de reunião são tratadas entre o representante e a entidade de segurança. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```XML
<DeliverMeetingRequests>DelegatesOnly or DelegatesAndMe or DelegatesAndSendInformationToMe or NoForward</DeliverMeetingRequests>
```

 **DeliverMeetingRequestsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AddDelegate](adddelegate.md) <br/> |Define uma solicitação para adicionar representantes a uma caixa de correio. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Define uma solicitação para atualizar representantes em uma caixa de correio. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Contém o status e o resultado de uma solicitação getdelegate. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o elemento **DeliverMeetingRequests** . 
  
**Valores do elemento DeliverMeetingRequests**

|**Valor**|**Descrição**|
|:-----|:-----|
|DelegatesOnly  <br/> |As solicitações de reunião são encaminhadas para o representante e movidas para a pasta itens excluídos na caixa de correio da entidade de segurança.  <br/> |
|DelegatesAndMe  <br/> |As solicitações de reunião são encaminhadas para o representante e permanecem na pasta caixa de entrada na caixa de correio da entidade de segurança.  <br/> |
|DelegatesAndSendInformationToMe  <br/> |As solicitações de reunião são encaminhadas para o representante e permanecem na pasta caixa de entrada na caixa de correio da entidade de segurança, mas os botões aceitar, provisório e recusar não aparecem no painel de leitura do Microsoft Office Outlook.  <br/> |
|Noforward  <br/> |As solicitações de reunião não são encaminhadas para o representante.  <br/> |
   
## <a name="remarks"></a>Comentários

A configuração **DeliverMeetingRequests** afeta todos os representantes da caixa de correio de uma entidade. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação AddDelegate](adddelegate-operation.md)  
- [Operação UpdateDelegate](updatedelegate-operation.md)  
- [Operação getdelegate](getdelegate-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Adicionar representantes](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

