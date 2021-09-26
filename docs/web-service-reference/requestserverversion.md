---
title: RequestServerVersion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RequestServerVersion
api_type:
- schema
ms.assetid: af4032d5-42b3-463e-9d0a-8236d78e5b75
description: O elemento RequestServerVersion contém as informações de versão que identificam a versão do esquema a ser direcionada para uma solicitação.
ms.openlocfilehash: 4f01d5fcc2a2e08d426efc8d1f0a193d6139a038
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541872"
---
# <a name="requestserverversion"></a>RequestServerVersion

O **elemento RequestServerVersion** contém as informações de versão que identificam a versão do esquema a ser direcionada para uma solicitação. 
  
```XML
<RequestServerVersion Version=""/>
```

 **ExchangeVersionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Versão  <br/> |Descreve a versão a ser direcionada para a solicitação. Esse atributo é necessário quando a versão do servidor de destino é uma versão do Exchange começando com Exchange Server 2010.  <br/> |
   
#### <a name="version-attribute-values"></a>Valores de atributo version

|**Valor**|**Descrição**|
|:-----|:-----|
|Exchange2007  <br/> |Direcionar os arquivos de esquema para a versão inicial do Exchange 2007.  <br/> |
|Exchange2007_SP1  <br/> |Direcionar os arquivos de esquema para Exchange 2007 Service Pack 1 (SP1), Exchange 2007 Service Pack 2 (SP2) e Exchange 2007 Service Pack 3 (SP3).  <br/> |
|Exchange2010  <br/> |Direcionar os arquivos de esquema para Exchange 2010.  <br/> |
|Exchange2010_SP1  <br/> |Direcionar os arquivos de esquema para Exchange 2010 Service Pack 1 (SP1).  <br/> |
|Exchange2010_SP2  <br/> |Direcionar os arquivos de esquema para Exchange 2010 Service Pack 2 (SP2) e Exchange 2010 Service Pack 3 (SP3).  <br/> |
|Exchange2013  <br/> |Direcionar os arquivos de esquema para Exchange 2013.  <br/> |
|Exchange2013_SP1  <br/> |Direcionar os arquivos de esquema para Exchange 2013 Service Pack 1 (SP1).  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

O **elemento RequestServerVersion** está localizado no header SOAP. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Solicitações de versão](https://msdn.microsoft.com/library/76877b0a-d2e5-4c74-9295-7b445a41d46a%28Office.15%29.aspx)

