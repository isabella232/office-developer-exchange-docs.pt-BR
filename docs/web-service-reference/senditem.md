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
description: O elemento SendItem é o elemento raiz em uma solicitação para enviar um item no armazenamento do Exchange.
ms.openlocfilehash: c5ce52ee4643219aa31ae59e8b7d40d7a904c8ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825340"
---
# <a name="senditem"></a>SendItem

O elemento **SendItem** é o elemento raiz em uma solicitação para enviar um item no armazenamento do Exchange. 
  
```xml
<SendItem SaveItemToFolder="">
   <ItemIds/>
   <SavedItemFolderId/>
</SendItem>
```

 **SendItemType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**SaveItemToFolder** <br/> |Identifica se uma cópia do item enviado é salva. Salvar ação depende do valor de **SaveItemToFolder** e se um elemento [SavedItemFolderId](saveditemfolderid.md) está presente na solicitação. Este elemento é obrigatório.  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a>Atributo SaveItemToFolder

|**Valor**|**Descrição**|
|:-----|:-----|
|**True** <br/> |Se o elemento [SavedItemFolderId](saveditemfolderid.md) não estiver presente, o item é salvo na pasta Itens enviados. Se o elemento [SavedItemFolderId](saveditemfolderid.md) estiver presente, o item é salvo na pasta especificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
|**False** <br/> |Se o elemento [SavedItemFolderId](saveditemfolderid.md) não estiver presente, o item não é salvo. Se o elemento [SavedItemFolderId](saveditemfolderid.md) estiver presente, uma resposta de erro será retornada com um elemento [ResponseCode](responsecode.md) que contém o valor de **ErrorInvalidSendItemSaveSettings** .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemIds](itemids.md) <br/> |Contém as identidades exclusivas dos itens, itens de ocorrência e itens recorrentes de mestres que são usados para excluir, enviar, obter, mover ou copiar itens no armazenamento do Exchange.  <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Identifica a pasta de destino para operações de atualização, enviar e crie itens no armazenamento do Exchange.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

Se um item na pasta Itens enviados é enviado, o item enviado será excluído e uma cópia dele é colocada na pasta Itens enviados.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação SendItem](senditem-operation.md)

