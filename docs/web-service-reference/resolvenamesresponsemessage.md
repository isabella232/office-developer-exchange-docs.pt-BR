---
title: ResolveNamesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNamesResponseMessage
api_type:
- schema
ms.assetid: edcdaf58-ef63-412e-8c58-409213e6ab0d
description: O elemento ResolveNamesResponseMessage contém o status e o resultado de uma solicitação de operação ResolveNames.
ms.openlocfilehash: 953a1f0b19c078d969ffe175c22df02b58c5e939
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825170"
---
# <a name="resolvenamesresponsemessage"></a>ResolveNamesResponseMessage

O elemento **ResolveNamesResponseMessage** contém o status e o resultado de uma solicitação de [operação ResolveNames](resolvenames-operation.md) . 
  
- [ResolveNamesResponse](resolvenamesresponse.md) 
- [ResponseMessages](responsemessages.md)
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
  
```xml
<ResolveNamesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResolutionSet/>
</ResolveNamesResponseMessage>
```

 **ResolveNamesResponseMessageType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**ResponseClass** <br/> | Descreve o status de uma resposta [ResolveNames operação](resolvenames-operation.md) . <br/><br/>Os seguintes valores são válidos para este atributo:  <br/><br/>-Êxito  <br/>-Aviso  <br/>-Erro  <br/> |
   
#### <a name="responseclass-attribute"></a>Atributo ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|**Sucesso** <br/> |Descreve uma solicitação que seja cumprida. Esse problema ocorre quando o nome solicitado é inequívoco e a resposta conterá um único destinatário.  <br/> |
|**Warning** <br/> | Descreve uma solicitação que não foi processada. Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados. <br/><br/>Exemplo das fontes de avisos veja a seguir:  <br/><br/>-O armazenamento do Exchange fica offline durante o lote.  <br/>-Active Directory Domain Services (AD DS) ficará offline.  <br/>-Caixas de correio são movidas.  <br/>-O banco de dados de caixa de correio (MDB) ficará offline.  <br/>-Uma senha expirou.  <br/>-Uma cota for excedida.  <br/>-O nome solicitado é ambíguo e a resposta conterá vários destinatários.  <br/> |
|**Erro** <br/> | Descreve uma solicitação que não puder ser atendida. <br/><br/>Estes são exemplos de fontes de erros:  <br/><br/>-O nome solicitado não pôde ser resolvido.  <br/>-Atributos ou elementos são inválidos.  <br/>-Atributos ou elementos estão fora do intervalo.  <br/>-Uma marca é desconhecida.  <br/>-Um atributo ou elemento não é válido no contexto.  <br/>-Uma tentativa de acesso não autorizado por qualquer cliente ocorreu.  <br/>-Falha do servidor em resposta a uma chamada de cliente válida.  <br/>  <br/>Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece informações de erro sobre a solicitação.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |No momento não utilizados e está reservado para uso futuro. Ele contém um valor de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações de resposta de erro adicionais.  <br/> |
|[ResolutionSet](resolutionset.md) <br/> |Contém uma matriz de resoluções referentes a um nome ambíguo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [ResolveNames](resolvenames.md)
- [ResolveNamesResponse](resolvenamesresponse.md)
- [Operação ResolveNames](resolvenames-operation.md)

