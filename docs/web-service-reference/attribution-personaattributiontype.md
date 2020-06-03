---
title: Atribuição (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: O elemento de atribuição especifica uma instância em uma matriz de atributos para um elemento Personatype.
ms.openlocfilehash: 05b0d41c116f2ed7b8dbb3ac44108bb879256b5c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464172"
---
# <a name="attribution-personaattributiontype"></a>Atribuição (PersonaAttributionType)

O elemento de **atribuição** especifica uma instância em uma matriz de atributos para um elemento **personatype** . 
  
```XML
<Attribution>
    <Id></Id>
    <SourceId></SourceId>
    <DisplayName></DisplayName>
    <IsWritable></IsWritable>
    <IsQuickContact></IsQuickContact>
    <IsHidden></IsHidden>
    <FolderId></FolderId>
</Attribution>
```

 **PersonaAttributionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ID (cadeia de caracteres)](id-string.md) <br/> |Especifica uma cadeia de caracteres que identifica exclusivamente um aplicativo ou uma atribuição em uma pessoa.  <br/> |
|[SourceId](sourceid.md) <br/> |Especifica o identificador do contato ou destinatário do Active Directory.  <br/> |
|[DisplayName (cadeia de caracteres)](displayname-string.md) <br/> |Define o nome de exibição de uma pasta, contato, lista de distribuição, usuário delegado ou regra.  <br/> |
|[Iswritable](iswritable.md) <br/> |Especifica se o contato subjacente ou destinatário do Active Directory pode ser gravado.  <br/> |
|[IsQuickContact](isquickcontact.md) <br/> |Especifica um valor Boolean que indica se o contato subjacente ou o destinatário do Active Directory é um contato rápido.  <br/> |
|[IsHidden](ishidden.md) <br/> |Contém um valor booliano que indica se o contato subjacente ou o destinatário do Active Directory deve ser oculto ou exibido como parte do persona.  <br/> |
|[FolderId](folderid.md) <br/> |Contém o identificador e a chave de alteração de uma pasta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Atribuições (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md) <br/> |Especifica uma matriz de informações de atribuição para um ou mais destinatários de contatos ou do Active Directory (AD) agregados no persona associado.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

