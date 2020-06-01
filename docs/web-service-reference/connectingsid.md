---
title: ConnectingSID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectingSID
api_type:
- schema
ms.assetid: 56d6aa52-8fa6-4773-9046-44a6f4f5d97c
description: O elemento ConnectingSID representa uma conta para representar quando você estiver usando o cabeçalho SOAP ExchangeImpersonation.
ms.openlocfilehash: f4edf63f129fc769f4a2d710a505b40da4057fab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459276"
---
# <a name="connectingsid"></a>ConnectingSID

O elemento **ConnectingSID** representa uma conta para representar quando você estiver usando o cabeçalho SOAP ExchangeImpersonation. 
  
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
|[PrincipalName](principalname.md) <br/> |Representa o nome principal do usuário (UPN) da conta a ser usada para representação. Este deve ser o UPN para o domínio no qual a conta de usuário existe.  <br/> |
|[Identifica](sid.md) <br/> |Representa a forma SDDL (Security Descriptor Definition Language) do identificador de segurança (SID) da conta a ser usada para representação.  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Representa o endereço SMTP (Simple Mail Transfer Protocol) principal da conta a ser usada para a representação do Exchange. Se o endereço SMTP principal for fornecido, ele custará uma pesquisa adicional do serviço de diretório do Active Directory para obter o SID do usuário. Recomendamos que você use o SID ou o UPN se eles estiverem disponíveis.  <br/> |
|[SmtpAddress](smtpaddress.md) <br/> |Representa o endereço SMTP (Simple Mail Transfer Protocol) da conta a ser usada para a representação do Exchange. Se o endereço SMTP for fornecido, ele custará uma pesquisa do Active Directory extra para obter o SID do usuário. Recomendamos que você use o SID ou o UPN se eles estiverem disponíveis.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Usado no cabeçalho SOAP de uma solicitação. Quando esse elemento estiver presente, o chamador está tentando representar a conta que está contida no elemento **ExchangeImpersonation** .  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a>Comentários

A conta de chamada deve ter o direito **ms-Exch-Impersonation** no servidor de acesso para cliente e o **ms-exch-MayImpersonate** diretamente no banco de dados de caixa de correio que contém a caixa de correio para representar ou o objeto de contato ou usuário do Active Directory. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Autorização de servidor para servidor no EWS](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

