---
title: GetMessageTrackingReportResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetMessageTrackingReportResponse
api_type:
- schema
ms.assetid: 41177894-2008-44a6-86f8-bc34c0a48e36
description: O elemento GetMessageTrackingReportResponse contém a resposta para a operação GetMessageTrackingReport.
ms.openlocfilehash: d4377d44337555c4f8d93bc6a57d8d3b2fc583e9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520539"
---
# <a name="getmessagetrackingreportresponse"></a>GetMessageTrackingReportResponse

O **elemento GetMessageTrackingReportResponse** contém a resposta para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).
  
```xml
<GetMessageTrackingReportResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MessageTrackingReport/>
   <Diagnostics/>
   <Errors/>
   <Properties/>
</GetMessageTrackingReportResponse>
```

 **GetMessageTrackingReportResponseMessageType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ResponseClass** <br/> | Descreve o status da resposta. <br/><br/>Os seguintes valores são válidos para este atributo:  <br/><br/>- Sucesso  <br/>- Aviso  <br/>- Erro  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valores de atributo ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|**Success** <br/> |Descreve uma solicitação que é atendida.  <br/> |
|**Aviso** <br/> | Descreve uma solicitação que não foi processada. Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e os itens subsequentes não puderam ser processados.<br/><br/> Veja a seguir exemplos de fontes de avisos:  <br/><br/>- O Exchange store está offline durante o lote.  <br/>- O Serviço de Domínio do Active Directory (AD DS) está offline.  <br/>- As caixas de correio foram movidas.  <br/>- O banco de dados de mensagens (MDB) está offline.  <br/>- Uma senha expirou.  <br/>- Uma cota foi excedida.  <br/> |
|**Erro** <br/> | Descreve uma solicitação que não pode ser atendida. <br/><br/>Veja a seguir exemplos de fontes de erros:  <br/>  Atributos ou elementos inválidos  <br/><br/>- Atributos ou elementos que estão fora do intervalo  <br/>- Uma marca desconhecida  <br/>- Um atributo ou elemento que não é válido no contexto  <br/>- Uma tentativa de acesso não autorizada por qualquer cliente  <br/>- Uma falha no lado do servidor em resposta a uma chamada válida do lado do cliente  <br/><br/>  Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText.](messagetext.md)  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece um código de erro que identifica o erro específico encontrado pela solicitação.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Atualmente não usado e reservado para uso futuro. Esse elemento contém um valor 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta a erros.  <br/> |
|[MessageTrackingReport](messagetrackingreport.md) <br/> |Contém uma única mensagem retornada em uma [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).  <br/> |
|[Diagnostics](diagnostics.md) <br/> |Fornece informações de tempo e desempenho usadas para relatórios em um DataCenter.  <br/> |
|[Erros](errors-ex15websvcsotherref.md) <br/> |Contém um pacote de propriedades para armazenar erros retornados por meio do serviço Web.  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Contém uma lista de uma ou mais propriedades de controle.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetMessageTrackingReport](getmessagetrackingreport-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

