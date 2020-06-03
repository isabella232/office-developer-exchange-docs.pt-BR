---
title: Getdelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegate
api_type:
- schema
ms.assetid: 6d5efe59-596f-46f8-bdc6-ca9cded9bb8e
description: O elemento getdelegate define uma solicitação para obter informações sobre representantes para uma caixa de correio. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: bd7fb55800b51eb2d69184bc4e04cdef3e6b9a89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461027"
---
# <a name="getdelegate"></a>Getdelegate

O elemento **Getdelegate** define uma solicitação para obter informações sobre representantes para uma caixa de correio. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<GetDelegate IncludePermissions="">
      <Mailbox/>
   <UserIds/>
</GetDelegate>
```

 **Getdelegatetype**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**IncludePermissions** <br/> |Indica se a resposta contém as configurações de permissão para cada usuário delegado.  <br/> |
   
#### <a name="includepermissions-attribute-values"></a>Valores de atributo IncludePermissions

|**Valor**|**Descrição**|
|:-----|:-----|
|**True** <br/> |As permissões de usuário delegadas são retornadas além das informações de usuário delegado que são retornadas no elemento [userid](userid.md) .  <br/> |
|**Falso** <br/> |As informações de [userid](userid.md) são retornadas.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixa de Correio](mailbox.md) <br/> |Identifica a caixa de correio da entidade de segurança.  <br/> |
|[UserIds](userids.md) <br/> |Contém uma matriz de usuários delegados para obter da caixa de correio de uma entidade de segurança. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação getdelegate](getdelegate-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

