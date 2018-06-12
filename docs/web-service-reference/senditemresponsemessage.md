---
title: SendItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItemResponseMessage
api_type:
- schema
ms.assetid: 264f6a2f-c8cc-4c96-86e1-1aabb6f9d8ab
description: O elemento SendItemResponseMessage contém o status e o resultado de uma única solicitação de operação SendItem.
ms.openlocfilehash: 70355aa2b46303bfceafa2cfe89f1c84896f3158
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825344"
---
# <a name="senditemresponsemessage"></a>SendItemResponseMessage

O elemento **SendItemResponseMessage** contém o status e o resultado de uma única [operação SendItem](senditem-operation.md) solicitação. 
  
```xml
<SendItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</SendItemResponseMessage>
```

 **ResponseMessageType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**ResponseClass** <br/> | Descreve o status de uma resposta de [operação SendItem](senditem-operation.md) . <br/><br/>Os seguintes valores são válidos para este atributo: <br/> <br/>-Êxito  <br/>-Aviso  <br/>-Erro  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valores de atributo ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|**Sucesso** <br/> |Descreve uma solicitação que seja cumprida.  <br/> |
|**Warning** <br/> | Descreve uma solicitação que não foi processada. Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados. <br/><br/>Estes são exemplos de fontes de avisos de:  <br/><br/>-O armazenamento do Exchange está offline durante o lote.  <br/>-Active Directory Domain Services (AD DS) está offline.  <br/>-Caixas de correio são movidas.  <br/>-O banco de dados de mensagens (MDB) está offline.  <br/>-Uma senha expirou.  <br/>-Uma cota for excedida.  <br/> |
|**Erro** <br/> | Descreve uma solicitação que não puder ser atendida. <br/><br/>Estes são exemplos de fontes de erros:  <br/> <br/>-Inválido atributos e elementos  <br/>-Atributos ou elementos fora do intervalo  <br/>-Marca desconhecida  <br/>-Atributo ou elemento não é válido no contexto  <br/>-Tentativa de acesso não autorizado de qualquer cliente  <br/>-Falha server-side em resposta a uma chamada de cliente válida  <br/> <br/> Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |No momento não utilizados e está reservado para uso futuro. Ele contém um valor de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações de resposta de erro adicionais.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.  <br/> |
   
## <a name="remarks"></a>Coment�rios

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server com a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação SendItem](senditem-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

