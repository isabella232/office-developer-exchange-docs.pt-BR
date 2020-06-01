---
title: ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: c85207e1-1315-443b-94ec-2b58f405076b
description: O elemento ResolveNames define uma solicitação para resolver nomes ambíguos.
ms.openlocfilehash: 9c36a5f84451f91e90a8e7148cf384b5cacd7f29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467946"
---
# <a name="resolvenames"></a>ResolveNames

O elemento **ResolveNames** define uma solicitação para resolver nomes ambíguos. 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 **ResolveNamesType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ReturnFullContactData** <br/> |Descreve se os detalhes do contato completo para contatos públicos para um nome resolvido são retornados na resposta. Este atributo é necessário para contatos públicos. Esse valor não afeta contatos privados e listas de distribuição privada, para os quais o [ItemId](itemid.md) sempre é retornado.  <br/> |
|**SearchScope** <br/> |Identifica a ordem e o escopo de uma pesquisa ResolveNames.  <br/> |
|ContactDataShape  <br/> |Identifica o conjunto de propriedades retornado para os contatos. Este atributo foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a>Valores de atributo ReturnFullContactData

|**Valor**|**Descrição**|
|:-----|:-----|
|True  <br/> |Detalhes de contato completo para contatos públicos são retornados.  <br/> |
|Falso  <br/> |Detalhes de contato completo para contatos públicos não são retornados.  <br/> |
   
#### <a name="searchscope-attribute-values"></a>Valores de atributo SearchScope

|**Valor**|**Descrição**|
|:-----|:-----|
|ActiveDirectory  <br/> |Somente o serviço de diretório do Active Directory é pesquisado.  <br/> |
|ActiveDirectoryContacts  <br/> |O Active Directory é pesquisado primeiro e, em seguida, as pastas de contatos especificadas na propriedade [ParentFolderIds](parentfolderids.md) são pesquisadas.  <br/> |
|Contatos  <br/> |Somente as pastas de contatos identificadas pela propriedade [ParentFolderIds](parentfolderids.md) são pesquisadas.  <br/> |
|ContactsActiveDirectory  <br/> |As pastas de contatos identificadas pela propriedade [ParentFolderIds](parentfolderids.md) são pesquisadas primeiro e, em seguida, o Active Directory é pesquisado.  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a>Valores de atributo ContactDataShape

|**Valor**|**Descrição**|
|:-----|:-----|
|IdOnly  <br/> |A propriedade de identificador de item de contato é retornada.  <br/> |
|Padrão  <br/> |O conjunto padrão de propriedades de item de contato é retornado. Para obter mais informações, consulte [as formas de resposta no EWS](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).  <br/> |
|Propriedades  <br/> |O conjunto de propriedades de item de contato Propriedades é retornado. Para obter mais informações, consulte [as formas de resposta no EWS](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ParentFolderIds](parentfolderids.md) <br/> |Contém uma matriz de identificadores de pasta de contato que seriam pesquisados se o atributo **SearchScope** estiver definido como ActiveDirectoryContacts, contatos ou ContactsActiveDirectory. A matriz ParentFolderIds só pode conter um único identificador de pasta de contato. Se o elemento **ParentFolderIds** não estiver presente, a pasta de contatos padrão será pesquisada.  <br/> O identificador de pasta pode ser usado para acesso de representante.  <br/> As pesquisas do Active Directory são realizadas usando ACLs (listas de controle de acesso). Alguns usuários podem não ter os direitos para ver alguns objetos do Active Directory.  <br/> Este elemento é opcional.  <br/> |
|[UnresolvedEntry](unresolvedentry.md) <br/> |Contém o nome de um contato ou de uma lista de distribuição a ser resolvido.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação ResolveNames](resolvenames-operation.md)
  
[ResolveNamesType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[ResolveNamesSearchScopeType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Usando a resolução de nome](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

