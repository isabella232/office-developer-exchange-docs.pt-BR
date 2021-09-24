---
title: CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: cfdf01a9-0191-47c7-a7ad-5254d8bdee4a
description: O elemento CreateManagedFolder define uma solicitação para adicionar pastas personalizadas gerenciadas a uma caixa de correio.
ms.openlocfilehash: ca6850cfdc8a37bf0480db0c040b035591a59ce6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536370"
---
# <a name="createmanagedfolder"></a>CreateManagedFolder

O **elemento CreateManagedFolder** define uma solicitação para adicionar pastas personalizadas gerenciadas a uma caixa de correio. 
  
```xml
<CreateManagedFolder>
   <FolderNames/>
   <Mailbox/>
</CreateManagedFolder>
```

 **CreateManagedFolderRequestType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderNames](foldernames.md) <br/> |Contém uma matriz de pastas gerenciadas nomeadas para adicionar a uma caixa de correio.  <br/> |
|[Caixa de Correio](mailbox.md) <br/> |Identifica um objeto de serviço de diretório do Active Directory habilitado para email.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

A conta da pessoa que está fazendo a solicitação deve ter permissões FullAccess na caixa de correio onde as pastas gerenciadas são criadas. Você pode usar o parâmetro _ -AccessRights _ com o cmdlet Exchange **Add-MailboxPermission** do Shell de Gerenciamento para atribuir a permissão FullAccess. 
  
Embora você possa usar Exchange Web Services para adicionar pastas gerenciadas a uma caixa de correio, não é possível usar os Serviços Web Exchange para acessar a lista de pastas gerenciadas disponíveis. Para obter uma lista de pastas gerenciadas disponíveis, use o **cmdlet get-managedfolder** Exchange Shell de Gerenciamento. A lista retornada pelo **cmdlet get-managedfolder** conterá pastas personalizadas gerenciadas e pastas padrão gerenciadas. Você só pode adicionar pastas do tipo **managedcustomfolder** à caixa de correio usando a operação CreateManagedFolder. 
  
> [!NOTE]
> Você também pode obter uma lista de pastas gerenciadas usando a API DirectoryServices do Microsoft .NET Framework. 
  
Você pode usar a [operação FindFolder](findfolder-operation.md) para encontrar pastas gerenciadas em uma caixa de correio. As pastas gerenciadas podem ser distinguidas definindo o [elemento BaseShape](baseshape.md) como AllProperties na solicitação. A resposta conterá um [elemento ManagedFolderInformation](managedfolderinformation.md) para distinguir as pastas gerenciadas das pastas Exchange de armazenamento. Você pode excluir pastas gerenciadas da mesma maneira que exclui outros tipos de pasta. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação CreateManagedFolder](createmanagedfolder-operation.md)
  
[Operação FindFolder](findfolder-operation.md)


[Localizar Pastas](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Adicionando pastas gerenciadas](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

