---
title: CreateManagedFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateManagedFolderResponseMessage
api_type:
- schema
ms.assetid: a72eefc3-ef0b-4b44-a74b-e6907b5b5f68
description: O elemento CreateManagedFolderResponseMessage contém o status e o resultado de uma única solicitação de operação CreateManagedFolder.
ms.openlocfilehash: 5f98a056f34860161b69a250cf056e54d2b1f647
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536305"
---
# <a name="createmanagedfolderresponsemessage"></a>CreateManagedFolderResponseMessage

O **elemento CreateManagedFolderResponseMessage** contém o status e o resultado de uma única solicitação de operação [CreateManagedFolder.](createmanagedfolder-operation.md) 
  
- [CreateManagedFolderResponse](createmanagedfolderresponse.md)  
- [ResponseMessages](responsemessages.md) 
- [CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md)
  
```xml
<CreateManagedFolderResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CreateManagedFolderResponseMessage>
```

**FolderInfoResponseMessageType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ResponseClass** <br/> | Descreve o status de uma resposta de [operação CreateManagedFolder.](createmanagedfolder-operation.md)<br/><br/>Os seguintes valores são válidos para este atributo:<br/><br/>- Sucesso  <br/>- Aviso  <br/>- Erro  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valores de atributo ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|**Success** <br/> |Descreve uma solicitação que é atendida.  <br/> |
|**Aviso** <br/> | Descreve uma solicitação que não foi processada. Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e os itens subsequentes não puderam ser processados.<br/><br/>Veja a seguir exemplos de fontes de avisos:<br/><br/>- O Exchange store está offline durante o lote.  <br/>- Os Serviços de Domínio do Active Directory (AD DS) estão offline.  <br/>- As caixas de correio são movidas.  <br/>- O banco de dados de mensagens (MDB) está offline.  <br/>- Uma senha expirou.  <br/>- Uma cota é excedida.  <br/> |
|**Erro** <br/> | Descreve uma solicitação que não pode ser atendida.<br/><br/>Veja a seguir exemplos de fontes de erros:  <br/><br/>- Atributos ou elementos inválidos  <br/>- Atributos ou elementos fora do intervalo  <br/>- Marca desconhecida  <br/>- Atributo ou elemento não válido no contexto  <br/>- Tentativa de acesso não autorizada por qualquer cliente  <br/>- Falha do lado do servidor em resposta a uma chamada válida do lado do cliente<br/><br/>  Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText.](messagetext.md)  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece um código de erro que identifica o erro específico encontrado pela solicitação.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Atualmente não usado e reservado para uso futuro. Ele contém um valor 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta a erros.  <br/> |
|[Pastas](folders-ex15websvcsotherref.md) <br/> |Contém uma matriz de pastas gerenciadas criadas.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contém as mensagens de resposta para uma solicitação Exchange Web Services.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2010 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação CreateManagedFolder](createmanagedfolder-operation.md)
- [Referência do EWS para Exchange](ews-reference-for-exchange.md) 
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

