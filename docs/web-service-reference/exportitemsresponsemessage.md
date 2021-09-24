---
title: ExportItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExportItemsResponseMessage
api_type:
- schema
ms.assetid: 830fb008-3c45-4988-9041-91a3da3fe689
description: O elemento ExportItemsResponseMessage contém o status e os resultados de uma solicitação para exportar um único item de caixa de correio.
ms.openlocfilehash: 72a7d1bb969e12b38a0caee294325bd2c7a72e4d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517081"
---
# <a name="exportitemsresponsemessage"></a>ExportItemsResponseMessage

O **elemento ExportItemsResponseMessage** contém o status e os resultados de uma solicitação para exportar um único item de caixa de correio. 
  
- [ExportItemsResponse](exportitemsresponse.md)  
- [ResponseMessages](responsemessages.md) 
- [ExportItemsResponseMessage](exportitemsresponsemessage.md)
  
```XML
<ExportItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ItemId/>
   <Data/>
</ExportItemsResponseMessage>
```

**ExportItemsResponseMessageType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ResponseClass** <br/> | Descreve o status da resposta.<br/><br/> Os seguintes valores são válidos para este atributo: <br/> <br/>- Sucesso  <br/>- Aviso  <br/>- Erro  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valores de atributo ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|**Success** <br/> |Descreve uma solicitação que é atendida.  <br/> |
|**Aviso** <br/> | Descreve uma solicitação que não foi processada. Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e os itens subsequentes não puderam ser processados.<br/><br/> Veja a seguir exemplos de fontes de avisos:  <br/><br/>- O Exchange store está offline durante o lote.  <br/>- Os Serviços de Domínio do Active Directory (AD DS) estão offline.  <br/>- As caixas de correio foram movidas.  <br/>- O banco de dados de mensagens (MDB) está offline.  <br/>- Uma senha expirou.  <br/>- Uma cota foi excedida.  <br/> |
|**Erro** <br/> | Descreve uma solicitação que não pode ser atendida. <br/><br/>Veja a seguir exemplos de fontes de erros:  <br/><br/>- Atributos ou elementos inválidos  <br/>- Atributos ou elementos que estão fora do intervalo  <br/>- Uma marca desconhecida  <br/>- Um atributo ou elemento que não é válido no contexto  <br/>- Uma tentativa de acesso não autorizada por qualquer cliente  <br/>- Uma falha no lado do servidor em resposta a uma chamada válida do lado do cliente  <br/><br/>  Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText.](messagetext.md)  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece um código de erro que identifica o erro específico encontrado pela solicitação.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Atualmente não usado e reservado para uso futuro. Esse elemento contém um valor 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta a erros.  <br/> |
|[ItemId](itemid.md) <br/> |Contém o identificador de item de um item exportado.  <br/> |
|[Data (base64Binary)](data-base64binary.md) <br/> |Contém o conteúdo de um item exportado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contém as mensagens de resposta para uma solicitação Exchange Web Services.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação ExportItems](exportitems-operation.md) 
- [Operação UploadItems](uploaditems-operation.md)

