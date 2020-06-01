---
title: String
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- String
api_type:
- schema
ms.assetid: e6e362b1-4526-49e1-b283-1c4bc4295874
description: O elemento string representa uma cadeia de caracteres que é usada por itens, contatos, tarefas e conversas.
ms.openlocfilehash: fbb4219d35c4acdc2c80b21b73e6479a2ef317f7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463101"
---
# <a name="string"></a>String

O elemento **String** representa uma cadeia de caracteres que é usada por itens, contatos, tarefas e conversas. 
  
```XML
<String/>
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
|[Categories](categories-ex15websvcsotherref.md) <br/> |Contém uma coleção de cadeias de caracteres que identificam a quais categorias um item da caixa de correio pertence.  <br/> |
|[Filhos](children.md) <br/> |Contém os nomes dos filhos de um contato.  <br/> |
|[Companies](companies.md) <br/> |Representa a coleção de empresas que estão associadas a um contato ou a uma tarefa.  <br/> |
|[Contatos](contacts-ex15websvcsotherref.md) <br/> |Contém uma lista de contatos que estão associados a uma tarefa.  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |Contém a lista de categorias de todos os itens de conversa em uma caixa de correio.  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |Contém a lista de destinatários de uma conversa agregada em uma caixa de correio.  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |Contém uma lista de todos os remetentes de itens de conversa na caixa de correio.  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |Contém uma lista de todas as pessoas que enviaram mensagens não lidas atualmente nesta conversa em todas as pastas da caixa de correio.  <br/> |
|[Doclasss](itemclasses.md) <br/> |Contém uma lista de classes de item que devem ser carimbadas em mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |Contém uma lista das classificações de mensagem que devem ser carimbadas nas mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |Contém a lista de destinatários da conversa. Este elemento é somente leitura.  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |Contém uma lista de todos os remetentes dos itens de conversa na pasta atual. Este elemento é somente leitura.  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |Contém uma lista de todas as pessoas que enviaram mensagens não lidas atualmente nesta conversa na pasta atual.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto desse elemento é uma cadeia de caracteres que representa uma categoria, o filho de um contato, uma empresa, um destinatário exclusivo de uma conversa ou um contato associado a uma tarefa.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindConversation](findconversation-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

