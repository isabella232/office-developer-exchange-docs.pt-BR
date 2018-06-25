---
title: messageSnapshot
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- messageSnapshot
api_type:
- schema
ms.assetid: f157e44c-b950-463f-b086-31d5da94b7ff
description: 'Modificado pela última vez: 17 de setembro de 2015'
ms.openlocfilehash: 4b814def8eef8fb452d2e754c5f6787d644055f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751024"
---
# <a name="messagesnapshot"></a>messageSnapshot

**Aplica-se a:** Exchange Server 2013
  
O elemento **messageSnapshot** contém um atributo que especifica se o recurso de rastreamento de pipeline está habilitado para o servidor do Exchange que tem o acesso para cliente ou a função de servidor de caixa de correio instalada. 
  
- [configuração](configuration.md)  
- [mexRuntime](mexruntime.md) 
- [monitoramento](monitoring.md) 
- [messageSnapshot](messagesnapshot.md)
  
```XML
<messageSnapshot enabled="" />
```

**messageSnapshotType (booleano)**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**habilitado** <br/> |Um valor Boolean que indica se o recurso de rastreamento de pipeline está habilitado para o acesso do cliente ou o servidor de caixa de correio. O valor é **true** se o rastreamento de pipeline estiver habilitado; Caso contrário, o valor é **false** , ou o elemento não está presente.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[monitoramento](monitoring.md) <br/> |Contém informações de configuração que define como e quando o serviço de transporte monitora os operadores que estão instalados.  <br/> |
   
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |Esse arquivo não define um namespace.  <br/> |
|Nome do esquema  <br/> |Não disponível.  <br/> |
|Arquivo de validação  <br/> |Não disponível.  <br/> |
|Pode ser vazio  <br/> |Falso.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos de arquivo de configuração de agentes para o Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

