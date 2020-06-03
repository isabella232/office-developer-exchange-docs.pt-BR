---
title: DataType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DataType
api_type:
- schema
ms.assetid: 267fe5aa-f9b1-4d4c-ac11-0f2e50ec2627
description: O elemento DataType descreve o tipo de dados que é compartilhado por uma pasta compartilhada.
ms.openlocfilehash: a7df8d38e10f0ab31038d790d8f35208d1be66d5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458828"
---
# <a name="datatype"></a>DataType

O elemento **DataType** descreve o tipo de dados que é compartilhado por uma pasta compartilhada. 
  
```xml
<DataType>Calendar or Contacts</DataType>
```

**SharingDataType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetSharingFolder](getsharingfolder.md) <br/> |Define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o elemento **DataType** . 
  
**Valores do elemento DataType**

|**Valor**|**Descrição**|
|:-----|:-----|
|Calendário  <br/> |Indica que a pasta compartilhada contém informações do calendário.  <br/> |
|Contatos  <br/> |Indica que a pasta compartilhada contém informações de contato.  <br/> |
   
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

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

