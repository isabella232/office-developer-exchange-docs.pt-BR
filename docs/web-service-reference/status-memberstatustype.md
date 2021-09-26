---
title: Status (MemberStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Status
api_type:
- schema
ms.assetid: 4f8a860b-0a48-4a0d-9a7a-69a0304aa747
description: O elemento Status fornece informações sobre o status de um membro da lista de distribuição no servidor.
ms.openlocfilehash: 0142ac1fa88c4cc4e513f23bbfad2869e7df32e7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544595"
---
# <a name="status-memberstatustype"></a>Status (MemberStatusType)

O **elemento Status** fornece informações sobre o status de um membro da lista de distribuição no servidor. 
  
```
<Status>Unrecognized or Normal or Demoted</Status>
```

 **MemberStatusType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Membro](member-ex15websvcsotherref.md) <br/> |Representa um membro de uma lista de distribuição.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o **elemento Status.** 
  
**Valores do elemento Status**

|**Valor**|**Descrição**|
|:-----|:-----|
|Unrecognized  <br/> |As informações do membro são inválidas ou não-recognizadas.  <br/> |
|Normal  <br/> |As informações de membro em uma lista de distribuição estão em sincronia com o objeto referenciado.  <br/> |
|Rebaixado  <br/> |O objeto referenciado não está disponível.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

