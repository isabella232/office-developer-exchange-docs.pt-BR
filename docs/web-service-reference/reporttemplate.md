---
title: ReportTemplate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ReportTemplate
api_type:
- schema
ms.assetid: f528eee6-d5af-4745-8b00-a9834bf34be6
description: O elemento ReportTemplate representa o tipo de relatório a ser obter.
ms.openlocfilehash: 18fc98a8d9aaa777a590561aedd4e86fdf91f9af
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542796"
---
# <a name="reporttemplate"></a>ReportTemplate

O **elemento ReportTemplate** representa o tipo de relatório a ser obter. 
  
```xml
<ReportTemplate>Summary or RecipientPath</ReportTemplate>
```

 **MessageTrackingReportTemplateType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |Contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) recuperar o relatório de controle de mensagens completo para a ID especificada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o **elemento ReportTemplate.** 
  
**Valores do elemento ReportTemplate**

|**Valor**|**Descrição**|
|:-----|:-----|
|Resumo  <br/> |Especifica que o relatório exibirá todos os destinatários da mensagem e o status de entrega da mensagem para cada destinatário.  <br/> |
|RecipientPath  <br/> |Especifica que, para um único destinatário, o relatório exibirá um histórico completo dos eventos que ocorreram.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2010 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

