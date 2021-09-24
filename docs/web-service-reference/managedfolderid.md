---
title: ManagedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ManagedFolderId
api_type:
- schema
ms.assetid: 3efb7abb-0e91-4d8a-9fa2-3dec8bd17c30
description: O elemento ManagedFolderId contém a ID da pasta gerenciada.
ms.openlocfilehash: 85564ecb8e88b5f03dd74f167b26d065b9f00e0d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524802"
---
# <a name="managedfolderid"></a>ManagedFolderId

O **elemento ManagedFolderId** contém a ID da pasta gerenciada. 
  
```xml
<ManagedFolderId/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Contém informações sobre uma pasta gerenciada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário para esse elemento.
  
## <a name="remarks"></a>Comentários

O valor do identificador **ManagedFolderId** é o equivalente à **propriedade Guid** recuperada pelo `Get-ManagedFolder` comando microsoft Windows Powershell. Também é o valor do atributo **objectGUID** para a pasta gerenciada no serviço de diretório do Active Directory. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação CreateManagedFolder](createmanagedfolder-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Excluir Pastas](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)
  
[Adicionando pastas gerenciadas](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

