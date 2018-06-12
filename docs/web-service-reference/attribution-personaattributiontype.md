---
title: Atribuição (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: O elemento de atribuição Especifica uma instância em uma matriz de atributos de um elemento PersonaType.
ms.openlocfilehash: 0e800c92c75bf0c475d4bffd33d6ab49f9ad9a9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751233"
---
# <a name="attribution-personaattributiontype"></a>Atribuição (PersonaAttributionType)

O elemento de **atribuição** Especifica uma instância em uma matriz de atributos de um elemento **PersonaType** . 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ID (String)](id-string.md) <br/> |Especifica uma cadeia de caracteres que identifica exclusivamente uma atribuição de uma pessoa ou de um aplicativo.  <br/> |
|[SourceId](sourceid.md) <br/> |Especifica o identificador do contato ou destinatário do Active Directory.  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |Define o nome de exibição de uma pasta, o contato, a lista de distribuição, o usuário delegado ou a regra.  <br/> |
|[IsWritable](iswritable.md) <br/> |Especifica se o contato subjacente ou o destinatário do Active Directory pode ser gravado em.  <br/> |
|[IsQuickContact](isquickcontact.md) <br/> |Especifica um valor Boolean que indica se o contato subjacente ou o destinatário do Active Directory é um contato rápido.  <br/> |
|[IsHidden](ishidden.md) <br/> |Contém um valor Boolean que indica se o destinatário do Active Directory ou o contato subjacente deve ser oculto ou exibido como parte da pessoa.  <br/> |
|[FolderId](folderid.md) <br/> |Contém o identificador e alterar a chave de uma pasta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Atribuições (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md) <br/> |Especifica uma matriz das informações de atribuição para uma ou mais contatos ou destinatários do active directory (AD) agregados em que a pessoa associada.  <br/> |
   
## <a name="remarks"></a>Coment�rios

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

