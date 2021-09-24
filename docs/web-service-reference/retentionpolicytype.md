---
title: RetentionPolicyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: abce5b3e-971d-42fc-aeea-caa7202214de
description: O elemento RetentionPolicyType especifica o tipo de política de retenção aplicado a itens em uma conversa.
ms.openlocfilehash: 961f72c35443e9f265e9313166fa77c8cd93d654
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509382"
---
# <a name="retentionpolicytype"></a>RetentionPolicyType

O **elemento RetentionPolicyType** especifica o tipo de política de retenção aplicado a itens em uma conversa. 
  
```XML
<RetentionPolicyType> Delete | Archive </RetentionPolicyType>
```

 **RetentionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[ConversationAction](conversationaction.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento RetentionPolicyType** é o tipo de retenção aplicado a itens em uma conversa. O valor de texto **de Delete** indica que os itens na conversa são excluídos quando a retenção expira. O valor de texto **de Archive** indica que os itens na conversa são movidos para a caixa de correio de arquivo morto quando a retenção expira. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

