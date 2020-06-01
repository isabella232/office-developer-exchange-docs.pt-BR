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
ms.openlocfilehash: 12f32008dbbc603fca7adf26057f1f1904d3cfb2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455594"
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ResponseClass** <br/> | Descreve o status de uma resposta de [operação ResolveNames](resolvenames-operation.md) . <br/><br/>Os seguintes valores são válidos para este atributo:  <br/><br/>-Êxito  <br/>-Aviso  <br/>-Erro  <br/> |
   
#### <a name="responseclass-attribute"></a>Atributo ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|**Success** <br/> |Descreve uma solicitação que é atendida. Isso ocorre quando o nome solicitado é inambíguo e a resposta contém um único destinatário.  <br/> |
|**Aviso** <br/> | Descreve uma solicitação que não foi processada. Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes. <br/><br/>Veja a seguir um exemplo de fontes de avisos:  <br/><br/>– O repositório do Exchange fica offline durante o lote.  <br/>– O AD DS (serviços de domínio Active Directory) fica offline.  <br/>-As caixas de correio são movidas.  <br/>– O banco de dados de caixa de correio (MDB) fica offline.  <br/>-Uma senha expirou.  <br/>-Uma cota foi excedida.  <br/>-O nome solicitado é ambíguo e a resposta contém vários destinatários.  <br/> |
|**Error** <br/> | Descreve uma solicitação que não pode ser atendida. <br/><br/>A seguir estão exemplos de fontes de erros:  <br/><br/>-O nome solicitado não pôde ser resolvido.  <br/>-Os atributos ou elementos são inválidos.  <br/>-Os atributos ou elementos estão fora do intervalo.  <br/>-Uma marca é desconhecida.  <br/>-Um atributo ou elemento não é válido no contexto.  <br/>-Uma tentativa de acesso não autorizado por qualquer cliente ocorreu.  <br/>-Uma falha do servidor ocorreu em resposta a uma chamada válida do lado do cliente.  <br/>  <br/>As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece informações de erro sobre a solicitação.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Não utilizado no momento e está reservado para uso futuro. Ele contém um valor de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta de erro.  <br/> |
|[ResolutionSet](resolutionset.md) <br/> |Contém uma matriz de resoluções para um nome ambíguo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [ResolveNames](resolvenames.md)
- [ResolveNamesResponse](resolvenamesresponse.md)
- [Operação ResolveNames](resolvenames-operation.md)

