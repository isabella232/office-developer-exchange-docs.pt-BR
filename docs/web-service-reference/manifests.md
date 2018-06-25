---
title: Manifestos
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 650d9fc0-1504-4db4-95d6-d3ba86df66ca
description: O elemento de manifestos contém uma coleção de manifestos de app codificado na base64 que estão instalados para a conta de email.
ms.openlocfilehash: 3877841c097e6b968d0af51ae5261e5b4336c7ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824362"
---
# <a name="manifests"></a>Manifestos

O elemento de **manifestos** contém uma coleção de manifestos de app codificado na base64 que estão instalados para a conta de email. 
  
```XML
<Manifests>
   <Manifest/>
</Manifests>
```

 **ArrayOfAppManifestsType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

[Manifesto](manifest.md)
  
### <a name="parent-elements"></a>Elementos pai

[GetAppManifestsResponse](getappmanifestsresponse.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

