---
title: ExpandDL
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: affe84a5-ad98-4aba-83f4-8732938b763d
description: O elemento ExpandDL define uma solicitação para expandir uma lista de distribuição.
ms.openlocfilehash: 53c713ac21204be3d49e909bebd0bc8927856476
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545157"
---
# <a name="expanddl"></a>ExpandDL

O **elemento ExpandDL** define uma solicitação para expandir uma lista de distribuição. 
  
```xml
<ExpandDL>
   <Mailbox/>
</ExpandDL>
```

 **ExpandDLType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhuma
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixa de Correio](mailbox.md) <br/> |Identifica um endereço de email totalmente resolvido ou uma lista de distribuição. Essa caixa de correio representa a lista de distribuição a ser expandida.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

Uma expansão de lista de distribuição só será executada para uma única lista de distribuição. Uma expansão de lista de distribuição não é recursiva.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação ExpandDL](expanddl-operation.md)

