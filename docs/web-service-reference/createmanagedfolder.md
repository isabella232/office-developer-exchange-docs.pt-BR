---
title: CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: cfdf01a9-0191-47c7-a7ad-5254d8bdee4a
description: O elemento de CreateManagedFolder define uma solicitação para adicionar pastas personalizadas gerenciadas para uma caixa de correio.
ms.openlocfilehash: 4acc931de2a8665db092c3b309d914f0a3c67558
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751618"
---
# <a name="createmanagedfolder"></a>CreateManagedFolder

O elemento de **CreateManagedFolder** define uma solicitação para adicionar pastas personalizadas gerenciadas para uma caixa de correio. 
  
```xml
<CreateManagedFolder>
   <FolderNames/>
   <Mailbox/>
</CreateManagedFolder>
```

 **CreateManagedFolderRequestType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Nomes de pastas](foldernames.md) <br/> |Contém uma matriz de nomeada pastas gerenciadas para adicionar uma caixa de correio.  <br/> |
|[Caixa de correio](mailbox.md) <br/> |Identifica um objeto de serviço de diretório do Active Directory habilitado para email.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

A conta da pessoa que está fazendo a solicitação deve ter permissões de FullAccess na caixa de correio onde as pastas gerenciadas são criadas. Você pode usar o parâmetro de _ _ - AccessRights com o cmdlet do Shell de gerenciamento do Exchange **Add-MailboxPermission** para atribuir a permissão FullAccess. 
  
Embora você possa usar os serviços Web do Exchange para adicionar pastas gerenciadas para uma caixa de correio, você não pode usar os serviços Web do Exchange para acessar a lista de pastas gerenciadas que estão disponíveis. Para obter uma lista de pastas gerenciadas disponíveis, use o cmdlet do Shell de gerenciamento do Exchange de **get-managedfolder** . A lista retornada pelo **cmdlet get-managedfolder** conterá pastas personalizadas gerenciadas e a pastas padrão gerenciadas. Você somente pode adicionar pastas do tipo **managedcustomfolder** à caixa de correio usando a operação CreateManagedFolder. 
  
> [!NOTE]
> Você também pode obter uma lista de pastas gerenciadas usando a API DirectoryServices do Microsoft .NET Framework. 
  
Você pode usar a [operação FindFolder](findfolder-operation.md) para localizar pastas gerenciadas em uma caixa de correio. Pastas gerenciadas podem ser diferenciadas, definindo o elemento [BaseShape](baseshape.md) para AllProperties na solicitação. A resposta conterá um elemento [ManagedFolderInformation](managedfolderinformation.md) para distinguir as pastas gerenciadas a partir das pastas de repositório do Exchange. Você pode excluir pastas gerenciadas da mesma maneira que você exclua outros tipos de pasta. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação CreateManagedFolder](createmanagedfolder-operation.md)
  
[Operação FindFolder](findfolder-operation.md)


[Localizando pastas](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Adicionando pastas gerenciadas](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

