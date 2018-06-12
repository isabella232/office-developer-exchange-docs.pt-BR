---
title: ClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3445ef2b-1bb1-43ea-bc93-85c72401e5b6
description: O elemento ClientExtension contém informações de usuário e de configuração sobre um aplicativo.
ms.openlocfilehash: 5051248a2c8e664d82666bd7b42ee3c3046f43fe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751394"
---
# <a name="clientextension"></a>ClientExtension

O elemento **ClientExtension** contém informações de usuário e de configuração sobre um aplicativo. 
  
```XML
<ClientExtension IsAvailable=" true | false " IsMandatory=" true | false " IsEnabledByDefault=" true | false " Type="" Scope="" MarketplaceAssetId="" MarketplaceContentMarket="" AppStatus="" Etoken="">
    <SpecificUsers></SpecificUsers>
    <Manifest></Manifest>
</ClientExtension>
```

 **ClientExtensionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|IsAvailable  <br/> |Especifica se o aplicativo está disponível. Um valor de **true** para o atributo **IsAvailable** text indica que o aplicativo está disponível. Um valor **false** indica que o aplicativo não está disponível. Este atributo é opcional.  <br/> |
|IsMandatory  <br/> |Especifica se o aplicativo é obrigatório. Um valor de texto de **true** para o atributo **IsMandatory** indica que o aplicativo é obrigatório para a caixa de correio. Um valor **false** indica que o aplicativo não é obrigatório. Este atributo é opcional.  <br/> |
|IsEnabledByDefault  <br/> |Especifica se o aplicativo está habilitado por padrão. Um valor de texto de **true** para o atributo **IsEnabledByDefault** indica que o aplicativo está habilitado por padrão. Um valor **false** indica que o aplicativo não está ativado por padrão. Este atributo é opcional.  <br/> |
|ProvidedTo  <br/> |Especifica a qual o aplicativo é fornecido. Este atributo é opcional.  <br/> |
|Tipo  <br/> |Especifica o tipo do aplicativo.  <br/> |
|Escopo  <br/> |Especifica o escopo do aplicativo.  <br/> |
|MarketplaceAssetId  <br/> |Especifica o identificador de ativos do marketplace do aplicativo.  <br/> |
|MarketplaceContentMarket  <br/> |Especifica o conteúdo do marketplace que um usuário vê para obter detalhes e analisa sobre um aplicativo.  <br/> |
|AppStatus  <br/> |Especifica o código de status de um aplicativo de email em um estado inesperado.  <br/> |
|Etoken  <br/> |Especifica o token de licença para aplicativos de email paga ou de avaliação.  <br/> |
   
#### <a name="type"></a>Tipo

|**Valor**|**Descrição**|
|:-----|:-----|
|Default  <br/> |Indica que o aplicativo está disponível por padrão.  <br/> |
|Particular  <br/> |Indica que o aplicativo é privado.  <br/> |
|MarketPlace  <br/> |Indica que o aplicativo é um aplicativo do marketplace.  <br/> |
   
#### <a name="scope"></a>Escopo

|**Valor**|**Descrição**|
|:-----|:-----|
|None  <br/> |Indica que o aplicativo não tem nenhum escopo.  <br/> |
|Usuário  <br/> |Indica que o aplicativo é por usuário.  <br/> |
|Organização  <br/> |Indica que o aplicativo é para uma organização.  <br/> |
|Default  <br/> |Indica que o aplicativo é um aplicativo padrão.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SpecificUsers](specificusers.md) <br/> |Especifica as contas de email que podem acessar o aplicativo.  <br/> |
|[Manifesto](manifest.md) <br/> |Contém o arquivo de manifesto do aplicativo codificada de base 64.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ClientExtensions](clientextensions.md) <br/> |Especifica uma matriz de elementos de **ClientExtension** .  <br/> |
   
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

