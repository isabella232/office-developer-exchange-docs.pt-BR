---
title: PrincipalName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PrincipalName
api_type:
- schema
ms.assetid: 88c142d4-0bc7-43ea-a997-d7200664d900
description: O elemento PrincipalName representa o nome principal do usuário (UPN) da conta a ser usada para Exchange representação.
ms.openlocfilehash: f3cc23b1cab69e166b59d7c358f663772e71ea09
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543013"
---
# <a name="principalname"></a>PrincipalName

O **elemento PrincipalName** representa o nome principal do usuário (UPN) da conta a ser usada para Exchange representação. 
  
```xml
<PrincipalName/>
```

 **PrincipalNameType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |Representa uma conta para representar quando você está usando o header SOAP do ExchangeImpersonation.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa a UPN de um usuário. Esse valor existe no objeto do usuário no serviço de diretório do Active Directory. Isso contém o nome de logon do usuário e um nome de domínio que identifica o domínio no qual a conta de usuário está localizada, no seguinte formato:  `someone@example.com` .
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2010 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Autorização de servidor para servidor no EWS](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

