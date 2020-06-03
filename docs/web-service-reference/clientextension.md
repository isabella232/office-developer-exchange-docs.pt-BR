---
title: ClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3445ef2b-1bb1-43ea-bc93-85c72401e5b6
description: O elemento ClientExtension contém informações de usuário e configuração sobre um aplicativo.
ms.openlocfilehash: d3d9ce1d242a63f28da3464f0faff86abde502c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460194"
---
# <a name="clientextension"></a>ClientExtension

O elemento **ClientExtension** contém informações de usuário e configuração sobre um aplicativo. 
  
```XML
<ClientExtension IsAvailable=" true | false " IsMandatory=" true | false " IsEnabledByDefault=" true | false " Type="" Scope="" MarketplaceAssetId="" MarketplaceContentMarket="" AppStatus="" Etoken="">
    <SpecificUsers></SpecificUsers>
    <Manifest></Manifest>
</ClientExtension>
```

 **ClientExtensionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|IsAvailable  <br/> |Especifica se o aplicativo está disponível. Um valor de texto **true** para o atributo **IsAvailable** indica que o aplicativo está disponível. Um valor **false** indica que o aplicativo não está disponível. Esse atributo é opcional.  <br/> |
|IsMandatory  <br/> |Especifica se o aplicativo é obrigatório. Um valor de texto **true** para o atributo **IsMandatory** indica que o aplicativo é obrigatório para a caixa de correio. Um valor **false** indica que o aplicativo não é obrigatório. Esse atributo é opcional.  <br/> |
|IsEnabledByDefault  <br/> |Especifica se o aplicativo está habilitado por padrão. Um valor de texto **true** para o atributo **IsEnabledByDefault** indica que o aplicativo está habilitado por padrão. Um valor **false** indica que o aplicativo não está habilitado por padrão. Esse atributo é opcional.  <br/> |
|ProvidedTo  <br/> |Especifica para quem o aplicativo é fornecido. Esse atributo é opcional.  <br/> |
|Tipo  <br/> |Especifica o tipo do aplicativo.  <br/> |
|Escopo  <br/> |Especifica o escopo do aplicativo.  <br/> |
|MarketplaceAssetId  <br/> |Especifica o identificador de ativos do Marketplace do aplicativo.  <br/> |
|MarketplaceContentMarket  <br/> |Especifica o conteúdo do Marketplace que um usuário vê para obter detalhes e revisões sobre um aplicativo.  <br/> |
|AppStatus  <br/> |Especifica o código de status de um aplicativo de email em um estado inesperado.  <br/> |
|Etoken  <br/> |Especifica o token de licença para aplicativos de email pagos ou de avaliação.  <br/> |
   
#### <a name="type"></a>Tipo

|**Valor**|**Descrição**|
|:-----|:-----|
|Padrão  <br/> |Indica que o aplicativo está disponível por padrão.  <br/> |
|Private  <br/> |Indica que o aplicativo é privado.  <br/> |
|Competitivo  <br/> |Indica que o aplicativo é um aplicativo de Marketplace.  <br/> |
   
#### <a name="scope"></a>Escopo

|**Valor**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |Indica que o aplicativo não tem escopo.  <br/> |
|Usuário  <br/> |Indica que o aplicativo é por usuário.  <br/> |
|Organização  <br/> |Indica que o aplicativo é para uma organização.  <br/> |
|Padrão  <br/> |Indica que o aplicativo é um aplicativo padrão.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SpecificUsers](specificusers.md) <br/> |Especifica as contas de email que podem acessar o aplicativo.  <br/> |
|[Manifesto](manifest.md) <br/> |Contém o arquivo de manifesto de aplicativo codificado em base 64.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ClientExtensions](clientextensions.md) <br/> |Especifica uma matriz de elementos **ClientExtension** .  <br/> |
   
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

