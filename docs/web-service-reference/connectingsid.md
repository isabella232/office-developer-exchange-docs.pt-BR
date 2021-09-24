---
title: ConnectingSID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConnectingSID
api_type:
- schema
ms.assetid: 56d6aa52-8fa6-4773-9046-44a6f4f5d97c
description: O elemento ConnectingSID representa uma conta para representar quando você está usando o header SOAP do ExchangeImpersonation.
ms.openlocfilehash: 21cfcfc3590ea5a8b8ca5b53dfdb403e108e37f7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515968"
---
# <a name="connectingsid"></a>ConnectingSID

O **elemento ConnectingSID** representa uma conta para representar quando você está usando o header SOAP do ExchangeImpersonation. 
  
- [ExchangeImpersonation](exchangeimpersonation.md) 
- [ConnectingSID](connectingsid.md)
  
```xml
<ConnectingSID>
   <PrincipalName/>
</ConnectingSID>
```

```xml
<ConnectingSID>
   <SmtpAddress/>
</ConnectingSID>
```

```xml
<ConnectingSID>
    <SID/> 
</ConnectingSID>
```

```xml
<ConnectingSID>
   <PrimarySmtpAddress/>
</ConnectingSID>
```

**ConnectingSIDType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PrincipalName](principalname.md) <br/> |Representa o nome principal do usuário (UPN) da conta a ser usada para representação. Esse deve ser o UPN para o domínio onde a conta de usuário existe.  <br/> |
|[SID](sid.md) <br/> |Representa o formulário SDDL (linguagem de definição de descritor de segurança) do identificador de segurança (SID) para a conta a ser usada para representação.  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Representa o endereço SMTP (Simple Mail Transfer Protocol) principal da conta a ser usado para Exchange representação. Se o endereço SMTP principal for fornecido, ele custará uma busca extra de serviço de diretório do Active Directory para obter o SID do usuário. Recomendamos que você use o SID ou UPN se eles estão disponíveis.  <br/> |
|[SmtpAddress](smtpaddress.md) <br/> |Representa o endereço SMTP (Simple Mail Transfer Protocol) da conta a ser usada para Exchange Representação. Se o endereço SMTP for fornecido, ele custará uma busca extra do Active Directory para obter o SID do usuário. Recomendamos que você use o SID ou UPN se eles estão disponíveis.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Usado no header SOAP de uma solicitação. Quando esse elemento está presente, o chamador está tentando representar a conta contida no **elemento ExchangeImpersonation.**  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a>Comentários

A conta de chamada deve ter a **ms-exch-impersonation** direita no servidor de Acesso para Cliente e o **ms-exch-MayImpersonate** direito no banco de dados de caixa de correio que contém a caixa de correio para representar ou o usuário ou objeto de contato do Active Directory. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Autorização de servidor para servidor no EWS](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

