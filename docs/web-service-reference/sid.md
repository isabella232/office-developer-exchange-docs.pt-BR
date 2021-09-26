---
title: SID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SID
api_type:
- schema
ms.assetid: 2f33b29b-163b-4106-a74d-6fb76ec38951
description: O elemento SID representa o formulário SDDL (linguagem de definição de descritor de segurança) do identificador de segurança (SID) para a conta a ser usada para representação ou acesso de representante.
ms.openlocfilehash: 436f284b59d5146b481a25b7b0986db4aeee67ce
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547054"
---
# <a name="sid"></a>SID

O **elemento SID** representa o formulário SDDL (linguagem de definição de descritor de segurança) do identificador de segurança (SID) para a conta a ser usada para representação ou acesso de representante. 
  
```xml
<SID/>
```

 **SIDType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |Representa uma conta para representar ao usar o header SOAP do ExchangeImpersonation.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[UserId](userid.md) <br/> |Identifica um usuário delegado ou um usuário com permissões de acesso a pastas.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto é uma representação de cadeia de caracteres de um SID.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Exchange Server com a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

