---
title: Attribution (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: O elemento Attribution especifica uma instância em uma matriz de atributos para um elemento PersonaType.
ms.openlocfilehash: eb2fe66042b6c7f52732be20195f0f4b94ab867c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524375"
---
# <a name="attribution-personaattributiontype"></a>Attribution (PersonaAttributionType)

O **elemento Attribution** especifica uma instância em uma matriz de atributos para um **elemento PersonaType.** 
  
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
|[ID (String)](id-string.md) <br/> |Especifica uma cadeia de caracteres que identifica exclusivamente um aplicativo ou uma atribuição em uma persona.  <br/> |
|[SourceId](sourceid.md) <br/> |Especifica o identificador do contato ou destinatário do Active Directory.  <br/> |
|[DisplayName (cadeia de caracteres)](displayname-string.md) <br/> |Define o nome de exibição de uma pasta, contato, lista de distribuição, usuário representante ou regra.  <br/> |
|[IsWritable](iswritable.md) <br/> |Especifica se o contato subjacente ou o destinatário do Active Directory pode ser gravado.  <br/> |
|[IsQuickContact](isquickcontact.md) <br/> |Especifica um valor Boolean que indica se o contato subjacente ou o destinatário do Active Directory é um contato rápido.  <br/> |
|[IsHidden](ishidden.md) <br/> |Contém um valor Boolean que indica se o contato subjacente ou o destinatário do Active Directory deve ser oculto ou exibido como parte da persona.  <br/> |
|[FolderId](folderid.md) <br/> |Contém o identificador e a chave de alteração de uma pasta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Attributions (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md) <br/> |Especifica uma matriz de informações de atribuição para um ou mais dos contatos ou destinatários do Active Directory (AD) agregados à persona associada.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Tipo de esquema  <br/> |
|Arquivo de validação  <br/> |types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

