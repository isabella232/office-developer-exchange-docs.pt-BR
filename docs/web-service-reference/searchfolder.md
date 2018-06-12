---
title: SearchFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchFolder
api_type:
- schema
ms.assetid: 1a7d408b-2e98-4391-8834-085ed6d5757c
description: O elemento SearchFolder representa uma pasta de pesquisa que está contida em uma caixa de correio.
ms.openlocfilehash: d842c54dab7950c68e26804b676834c2d95debad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825302"
---
# <a name="searchfolder"></a>SearchFolder

O elemento **SearchFolder** representa uma pasta de pesquisa que está contida em uma caixa de correio. 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador e alterar a chave de uma pasta.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai que contém a pasta.  <br/> |
|[FolderClass](folderclass.md) <br/> |Representa a classe de pasta para uma determinada pasta.  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |Contém o nome de exibição de uma pasta.  <br/> |
|[TotalCount](totalcount.md) <br/> |Representa a contagem total de itens dentro de uma determinada pasta.  <br/> |
|[ChildFolderCount](childfoldercount.md) <br/> |Representa o número de pastas filho contida em uma pasta. Esta propriedade é somente leitura.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifica as propriedades estendidas de pastas.  <br/> |
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Contém informações sobre uma pasta gerenciada.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Representa a contagem de itens não lidos dentro de uma determinada pasta.  <br/> |
|[SearchParameters](searchparameters.md) <br/> |Contém os parâmetros que definem a uma pasta de pesquisa.  <br/> |
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |Contém todas as permissões configuradas para uma pasta. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta. Este elemento é somente leitura. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |Especifica os dados a serem acrescentados a uma propriedade de pasta durante uma [operação UpdateFolder](updatefolder-operation.md).  <br/> |
|[Criar (FolderSync)](create-foldersync.md) <br/> |Identifica uma única pasta para criar no repositório de cliente local.  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Representa uma atualização para uma única propriedade em uma pasta em uma [operação UpdateFolder](updatefolder-operation.md).  <br/> |
|[Atualização (FolderSync)](update-foldersync.md) <br/> |Identifica uma única pasta ao atualizar no repositório de cliente local.  <br/> |
|[Pastas](folders-ex15websvcsotherref.md) <br/> |Contém uma matriz de pastas usados nas operações da pasta.  <br/> |
   
## <a name="remarks"></a>Coment�rios

 **SearchFolder** é usado para as pastas de pesquisa comum e MicrosoftOfficeOutlook e Outlook Web Access visível pastas de pesquisa. Para uma pasta de pesquisa fiquem visíveis para o Outlook e Outlook Web Access, a pasta deve ser criada na pasta diferenciada SearchFolders. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

