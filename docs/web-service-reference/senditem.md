---
title: SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItem
api_type:
- schema
ms.assetid: a966da19-b05a-4504-ac98-91acc1667b9a
description: O elemento SendItem é o elemento raiz em uma solicitação para enviar um item no repositório do Exchange.
ms.openlocfilehash: 28f0d484dd079146c998cb7317bd2d80c6739e19
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530562"
---
# <a name="senditem"></a>SendItem

O elemento **SendItem** é o elemento raiz em uma solicitação para enviar um item no repositório do Exchange. 
  
```xml
<SendItem SaveItemToFolder="">
   <ItemIds/>
   <SavedItemFolderId/>
</SendItem>
```

 **SendItemType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**SaveItemToFolder** <br/> |Identifica se uma cópia do item enviado é salva. A ação salvar depende do valor de **SaveItemToFolder** e se um elemento [SavedItemFolderId](saveditemfolderid.md) está presente na solicitação. Este elemento é obrigatório.  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a>Atributo SaveItemToFolder

|**Valor**|**Descrição**|
|:-----|:-----|
|**verdadeiro** <br/> |Se o elemento [SavedItemFolderId](saveditemfolderid.md) não estiver presente, o item será salvo na pasta Itens enviados. Se o elemento [SavedItemFolderId](saveditemfolderid.md) estiver presente, o item será salvo na pasta especificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
|**false** <br/> |Se o elemento [SavedItemFolderId](saveditemfolderid.md) não estiver presente, o item não será salvo. Se o elemento [SavedItemFolderId](saveditemfolderid.md) estiver presente, uma resposta de erro será retornada com um elemento [ResponseCode](responsecode.md) que contém o valor de **ErrorInvalidSendItemSaveSettings** .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemIds](itemids.md) <br/> |Contém as identidades exclusivas de itens, itens de ocorrência e itens mestre recorrentes que são usados para excluir, enviar, obter, mover ou copiar itens no repositório do Exchange.  <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Identifica a pasta de destino para operações que atualizam, enviam e criam itens no repositório do Exchange.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

Se um item na pasta Itens enviados é enviado, o item enviado é excluído e uma cópia dele é colocada na pasta Itens enviados.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação SendItem](senditem-operation.md)

