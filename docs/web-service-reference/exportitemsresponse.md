---
title: ExportItemsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExportItemsResponse
api_type:
- schema
ms.assetid: ef44354b-fbdb-4f7c-b6bd-b27f56a1d018
description: O elemento ExportItemsResponse representa uma resposta a uma única solicitação ExportItems.
ms.openlocfilehash: a05a767032c32680cc269459b541446fcaa3d660
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526036"
---
# <a name="exportitemsresponse"></a>ExportItemsResponse

O elemento **ExportItemsResponse** representa uma resposta a uma única solicitação **ExportItems** . 
  
[ExportItemsResponse](exportitemsresponse.md)
  
```XML
<ExportItemsResponse>
   <ResponseMessages/>
</ExportItemsResponse>
```

 **ExportItemsResponseType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação ExportItems](exportitems-operation.md)
  
[Operação UploadItems](uploaditems-operation.md)

