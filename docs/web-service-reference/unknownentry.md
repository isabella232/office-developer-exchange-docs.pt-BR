---
title: UnknownEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UnknownEntry
api_type:
- schema
ms.assetid: 3cb4c62e-052a-4326-8639-8c41dfd047b2
description: O elemento UnknownEntry representa uma única entrada de permissão desconhecida que não pode ser resolvida no serviço de diretório do Active Directory. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 62d006de35955e0fe495d8435dce6f199b46249a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515037"
---
# <a name="unknownentry"></a>UnknownEntry

O **elemento UnknownEntry** representa uma única entrada de permissão desconhecida que não pode ser resolvida no serviço de diretório do Active Directory. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<UnknownEntry/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UnknownEntries](unknownentries.md) <br/> |Contém uma matriz de entradas de permissão desconhecidas que não podem ser resolvidas em relação ao Active Directory. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor do texto representa uma entrada de permissão que não pode ser resolvida em relação ao Active Directory. O valor do texto representa um identificador de segurança (SID).
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Definindo Folder-Level Permissões](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

