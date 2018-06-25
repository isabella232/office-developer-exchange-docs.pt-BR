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
description: O elemento de cadeia de caracteres representa uma cadeia de caracteres que é usada pelo itens, contatos, tarefas e conversas.
ms.openlocfilehash: 66260c7ebcb56049a78c5eddbe057dfa8d61f193
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825607"
---
# <a name="string"></a>String

O elemento de **cadeia de caracteres** representa uma cadeia de caracteres que é usada pelo itens, contatos, tarefas e conversas. 
  
```XML
<String/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Categories](categories-ex15websvcsotherref.md) <br/> |Contém uma coleção de cadeias de caracteres que identificam a quais categorias de um item na caixa de correio pertence.  <br/> |
|[Filhos](children.md) <br/> |Contém os nomes dos filhos de um contato.  <br/> |
|[Empresas](companies.md) <br/> |Representa a coleção de empresas que estão associados um contato ou uma tarefa.  <br/> |
|[Contatos](contacts-ex15websvcsotherref.md) <br/> |Contém uma lista de contatos que estão associados uma tarefa.  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |Contém a lista de categorias para todos os itens de conversa em uma caixa de correio.  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |Contém a lista de destinatários de uma conversa agregada em uma caixa de correio.  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |Contém uma lista de todos os remetentes dos itens de conversa na caixa de correio.  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |Contém uma lista de todas as pessoas que tenham enviado mensagens que estão atualmente não lidas nesta conversa entre todas as pastas na caixa de correio.  <br/> |
|[ItemClasses](itemclasses.md) <br/> |Contém uma lista das classes item que deve ser marcada em mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |Contém uma lista das classificações de mensagem que deve ser marcada em mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |Contém a lista de destinatários da conversa. Este elemento é somente leitura.  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |Contém uma lista de todos os remetentes dos itens de conversa na pasta atual. Este elemento é somente leitura.  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |Contém uma lista de todas as pessoas que tenham enviado mensagens que estão atualmente não lidas nesta conversa na pasta atual.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto deste elemento é uma cadeia de caracteres que representa uma categoria, o filho de um contato, uma empresa, um único destinatário de uma conversa ou um contato que está associado uma tarefa.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação FindConversation](findconversation-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

