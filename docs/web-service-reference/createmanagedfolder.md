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
description: O elemento CreateManagedFolder define uma solicitação para adicionar pastas personalizadas gerenciadas a uma caixa de correio.
ms.openlocfilehash: 01fe8b7341c38ad33089c56271434ad3f9a4e5f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458359"
---
# <a name="createmanagedfolder"></a>CreateManagedFolder

O elemento **CreateManagedFolder** define uma solicitação para adicionar pastas personalizadas gerenciadas a uma caixa de correio. 
  
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

Nenhum
  
## <a name="remarks"></a>Comentários

A conta da pessoa que está fazendo a solicitação deve ter permissões FullAccess na caixa de correio onde as pastas gerenciadas são criadas. Você pode usar o parâmetro _-AccessRights _ com o cmdlet **Add-MailboxPermission** do Shell de gerenciamento do Exchange para atribuir a permissão FullAccess. 
  
Embora você possa usar os serviços Web do Exchange para adicionar pastas gerenciadas a uma caixa de correio, não é possível usar os serviços Web do Exchange para acessar a lista de pastas gerenciadas que estão disponíveis. Para obter uma lista de pastas gerenciadas disponíveis, use o cmdlet **Get-ManagedFolder** do Shell de gerenciamento do Exchange. A lista retornada pelo **cmdlet Get-ManagedFolder** conterá pastas personalizadas gerenciadas e pastas padrão gerenciadas. Você só pode adicionar pastas do tipo **ManagedCustomFolder** à caixa de correio usando a operação CreateManagedFolder. 
  
> [!NOTE]
> Você também pode obter uma lista de pastas gerenciadas usando a API DirectoryServices do Microsoft .NET Framework. 
  
Você pode usar a [operação FindFolder](findfolder-operation.md) para localizar pastas gerenciadas em uma caixa de correio. Pastas gerenciadas podem ser distinguidas Configurando o elemento [BaseShape](baseshape.md) para myproperties na solicitação. A resposta conterá um elemento [ManagedFolderInformation](managedfolderinformation.md) para distinguir as pastas gerenciadas das pastas do repositório do Exchange. Você pode excluir pastas gerenciadas da mesma maneira que exclui outros tipos de pasta. 
  
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


[Localizando pastas](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Adicionando pastas gerenciadas](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

