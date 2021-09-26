---
title: SearchFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SearchFolder
api_type:
- schema
ms.assetid: 1a7d408b-2e98-4391-8834-085ed6d5757c
description: O elemento SearchFolder representa uma pasta de pesquisa que está contida em uma caixa de correio.
ms.openlocfilehash: 44f19dad83e8cd18045901bc7e3e48e31508b3db
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544000"
---
# <a name="searchfolder"></a>SearchFolder

O **elemento SearchFolder** representa uma pasta de pesquisa que está contida em uma caixa de correio. 
  
```xml
<SearchFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <UnreadCount/>
   <SearchParameters/>
   <PermissionSet/>
      <EffectiveRights/>
</SearchFolder>
```

 **SearchFolderType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador e a chave de alteração de uma pasta.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai que contém a pasta.  <br/> |
|[FolderClass](folderclass.md) <br/> |Representa a classe folder de uma determinada pasta.  <br/> |
|[DisplayName (cadeia de caracteres)](displayname-string.md) <br/> |Contém o nome de exibição de uma pasta.  <br/> |
|[TotalCount](totalcount.md) <br/> |Representa a contagem total de itens em uma determinada pasta.  <br/> |
|[ChildFolderCount](childfoldercount.md) <br/> |Representa o número de pastas filho contidas em uma pasta. Essa propriedade é somente leitura.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifica propriedades estendidas em pastas.  <br/> |
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Contém informações sobre uma pasta gerenciada.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Representa a contagem de itens não lidos em uma determinada pasta.  <br/> |
|[SearchParameters](searchparameters.md) <br/> |Contém os parâmetros que definem uma pasta de pesquisa.  <br/> |
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |Contém todas as permissões configuradas para uma pasta. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contém os direitos do cliente com base nas configurações de permissão do item ou pasta. Esse elemento é somente leitura. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |Especifica dados a ser anexados a uma propriedade de pasta durante uma [operação UpdateFolder.](updatefolder-operation.md)  <br/> |
|[Create (FolderSync)](create-foldersync.md) <br/> |Identifica uma única pasta a ser criado no armazenamento do cliente local.  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Representa uma atualização para uma única propriedade em uma pasta em uma [operação UpdateFolder](updatefolder-operation.md).  <br/> |
|[Update (FolderSync)](update-foldersync.md) <br/> |Identifica uma única pasta a ser atualizada no armazenamento cliente local.  <br/> |
|[Pastas](folders-ex15websvcsotherref.md) <br/> |Contém uma matriz de pastas usadas em operações de pasta.  <br/> |
   
## <a name="remarks"></a>Comentários

 **SearchFolder** é usado para pastas de pesquisa regulares e MicrosoftOfficeOutlook e Outlook de pesquisa visíveis do Web Access. Para que uma pasta de pesquisa seja visível Outlook e Outlook Web Access, a pasta deve ser criada sob a pasta distinta SearchFolders. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

