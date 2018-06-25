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
description: O elemento de ResolveNames define uma solicitação para resolver nomes de ambíguos.
ms.openlocfilehash: e97b6e78d99cf8ffa3d680907916882d40963f59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825172"
---
# <a name="resolvenames"></a>ResolveNames

O elemento de **ResolveNames** define uma solicitação para resolver nomes de ambíguos. 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 **ResolveNamesType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**ReturnFullContactData** <br/> |Descreve se os detalhes de contato completo para Contatos públicos para um nome resolvido são retornados na resposta. Este atributo é necessário para Contatos públicos. Este valor não afeta privados contatos e listas de distribuição privada, para o qual [ItemId](itemid.md) sempre será retornado.  <br/> |
|**SearchScope** <br/> |Identifica o escopo para uma pesquisa ResolveNames e ordem.  <br/> |
|ContactDataShape  <br/> |Identifica a propriedade definida retornada para contatos. Este atributo foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a>Valores de atributo ReturnFullContactData

|**Valor**|**Descrição**|
|:-----|:-----|
|True  <br/> |Detalhes do contato completa para Contatos públicos são retornadas.  <br/> |
|False  <br/> |Detalhes do contato completa para Contatos públicos não são retornados.  <br/> |
   
#### <a name="searchscope-attribute-values"></a>Valores de atributo SearchScope

|**Valor**|**Descrição**|
|:-----|:-----|
|ActiveDirectory  <br/> |O serviço de diretório do Active Directory é pesquisado.  <br/> |
|ActiveDirectoryContacts  <br/> |Active Directory é pesquisado primeiro e, em seguida, as pastas de contato que são especificadas na propriedade [ParentFolderIds](parentfolderids.md) são pesquisadas.  <br/> |
|Contatos  <br/> |Somente as pastas de contato que são identificadas pela propriedade [ParentFolderIds](parentfolderids.md) são pesquisadas.  <br/> |
|ContactsActiveDirectory  <br/> |Pastas de contatos são identificadas pela propriedade [ParentFolderIds](parentfolderids.md) são pesquisadas primeiro e, em seguida, o Active Directory é pesquisado.  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a>Valores de atributo ContactDataShape

|**Valor**|**Descrição**|
|:-----|:-----|
|IdOnly  <br/> |A propriedade do identificador de item de contato é retornada.  <br/> |
|Default  <br/> |O conjunto de propriedades de item de contato padrão será retornado. Para obter mais informações, consulte [as formas de resposta no EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).  <br/> |
|AllProperties  <br/> |O conjunto de AllProperties de propriedades de item de contato são retornadas. Para obter mais informações, consulte [as formas de resposta no EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ParentFolderIds](parentfolderids.md) <br/> |Contém uma matriz de identificadores de pasta de contato que seria ser pesquisada se o atributo **SearchScope** estiver definido como ActiveDirectoryContacts, contatos ou ContactsActiveDirectory. A matriz ParentFolderIds só pode conter um identificador único de pasta de contato. Se o elemento **ParentFolderIds** não estiver presente, a pasta padrão Contatos é pesquisada.  <br/> O identificador de pasta pode ser usado para acesso de representante.  <br/> Pesquisas do Active Directory são realizadas usando listas de controle de acesso (ACLs). Alguns usuários talvez não tenha os direitos para ver alguns objetos do Active Directory.  <br/> Esse elemento é opcional.  <br/> |
|[UnresolvedEntry](unresolvedentry.md) <br/> |Contém o nome de uma lista de contatos ou de distribuição para resolver.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação ResolveNames](resolvenames-operation.md)
  
[ResolveNamesType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[ResolveNamesSearchScopeType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Usando a resolução de nome](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

