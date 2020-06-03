---
title: Member
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Member
api_type:
- schema
ms.assetid: af9c5ff8-02a4-41fc-876d-14ac05f1ee77
description: O elemento member representa um membro de uma lista de distribuição.
ms.openlocfilehash: e84223b7c41846ca2f174293bff46a8825777a0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457302"
---
# <a name="member"></a>Member

O elemento **Member** representa um membro de uma lista de distribuição. 
  
```xml
<Member Key="">
   <Mailbox/>
   <Status/>
</Member>
```

**MemberType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Chave  <br/> |Fornece um identificador exclusivo para o membro da lista de distribuição. Esse atributo é opcional.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixa de Correio](mailbox.md) <br/> |Representa o endereço de email do membro da lista de distribuição. Este elemento é opcional.  <br/> |
|[Status (MemberStatusType)](status-memberstatustype.md) <br/> |Fornece informações sobre o status de um membro da lista de distribuição. Este elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Membros (MemberListType)](members-memberlisttype.md) <br/> |Contém uma lista de membros da lista de distribuição.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

