---
title: Caixa de correio (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4ad59e5b-4047-4c34-a318-ca06c31d3de8
description: O elemento Mailbox contém o endereço de email do usuário a ser descoberto.
ms.openlocfilehash: e050cd9d3ca4a2d2450f315f1eedd3862328d096
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467281"
---
# <a name="mailbox-soap"></a>Caixa de correio (SOAP)

O elemento **Mailbox** contém o endereço de email do usuário a ser descoberto. 
  
```XML
<Mailbox/>
```

**cadeia de caracteres**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Usuário (SOAP)](user-soap.md) <br/> |Representa a identidade de um único usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **Mailbox** é o endereço de email do usuário a ser descoberto. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Também consulte

- [Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)

