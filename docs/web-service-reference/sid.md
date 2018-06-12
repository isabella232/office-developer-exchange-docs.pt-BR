---
title: SID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SID
api_type:
- schema
ms.assetid: 2f33b29b-163b-4106-a74d-6fb76ec38951
description: O elemento SID representa um formulário de segurança descritor definition language (SDDL) do identificador de segurança (SID) para a conta usada para representação ou acesso de representante.
ms.openlocfilehash: efcea42c12ec1d26ea31fdb8de337c37a2338a96
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825492"
---
# <a name="sid"></a>SID

O elemento **SID** representa um formulário de segurança descritor definition language (SDDL) do identificador de segurança (SID) para a conta usada para representação ou acesso de representante. 
  
```xml
<SID/>
```

 **SIDType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |Representa uma conta para representar ao usar o cabeçalho SOAP ExchangeImpersonation.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[UserId](userid.md) <br/> |Identifica um usuário delegado ou um usuário com permissões de acesso de pasta.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto é uma representação de cadeia de caracteres de um SID.
  
## <a name="remarks"></a>Coment�rios

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server com a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

