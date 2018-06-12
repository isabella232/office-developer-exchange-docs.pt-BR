---
title: RequestServerVersion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestServerVersion
api_type:
- schema
ms.assetid: af4032d5-42b3-463e-9d0a-8236d78e5b75
description: O elemento RequestServerVersion contém as informações de controle de versão que identifica a versão do esquema de destino para uma solicitação.
ms.openlocfilehash: 0092d90a5fc479363f6d774b793c7148ad29f21c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825143"
---
# <a name="requestserverversion"></a>RequestServerVersion

O elemento **RequestServerVersion** contém as informações de controle de versão que identifica a versão do esquema de destino para uma solicitação. 
  
```XML
<RequestServerVersion Version=""/>
```

 **ExchangeVersionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|Versão  <br/> |Descreve a versão de destino para a solicitação. Este atributo é necessário quando a versão do servidor de destino for uma versão do Exchange, começando com o Exchange Server 2010.  <br/> |
   
#### <a name="version-attribute-values"></a>Valores de atributos de versão

|**Valor**|**Descrição**|
|:-----|:-----|
|Exchange2007  <br/> |Direcione os arquivos de esquema para a versão de lançamento inicial do Exchange 2007.  <br/> |
|Exchange2007_SP1  <br/> |Direcione os arquivos de esquema para o Exchange 2007 Service Pack 1 (SP1) do Exchange 2007 Service Pack 2 (SP2) e Exchange 2007 Service Pack 3 (SP3).  <br/> |
|Exchange2010  <br/> |Direcione os arquivos de esquema para o Exchange 2010.  <br/> |
|Exchange2010_SP1  <br/> |Direcione os arquivos de esquema para o Exchange 2010 Service Pack 1 (SP1).  <br/> |
|Exchange2010_SP2  <br/> |Direcione os arquivos de esquema para o Exchange 2010 Service Pack 2 (SP2) e Exchange 2010 Service Pack 3 (SP3).  <br/> |
|Exchange2013  <br/> |Direcione os arquivos de esquema para o Exchange 2013.  <br/> |
|Exchange2013_SP1  <br/> |Direcione os arquivos de esquema para o Exchange 2013 Service Pack 1 (SP1).  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

O elemento **RequestServerVersion** está localizado no cabeçalho SOAP. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Solicitações de controle de versão](http://msdn.microsoft.com/library/76877b0a-d2e5-4c74-9295-7b445a41d46a%28Office.15%29.aspx)

