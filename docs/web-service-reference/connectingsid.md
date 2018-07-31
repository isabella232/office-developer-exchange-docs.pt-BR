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
ms.openlocfilehash: a30f11721506989a84f52dd04c328974f4483956
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354334"
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

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PrincipalName](principalname.md) <br/> |Representa o nome de usuário principal (UPN) da conta a ser usada para a representação. Este deve ser o UPN para o domínio em que a conta de usuário existe.  <br/> |
|[SID](sid.md) <br/> |Representa o formulário de segurança descritor definition language (SDDL) do identificador de segurança (SID) para a conta a ser usada para representação.  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Representa o endereço de Simple Mail Transfer Protocol (SMTP) principal da conta a ser usada para a representação do Exchange. Se o endereço SMTP principal for fornecido, ele será custo uma pesquisa de serviço de diretório do Active Directory extra para obter o SID do usuário. Recomendamos que você use o UPN ou SID se eles estiverem disponíveis.  <br/> |
|[SmtpAddress](smtpaddress.md) <br/> |Representa o endereço de Simple Mail Transfer Protocol (SMTP) da conta a ser usada para a representação do Exchange. Se o endereço SMTP for fornecido, ele será custo uma pesquisa do Active Directory extra para obter o SID do usuário. Recomendamos que você use o UPN ou SID se eles estiverem disponíveis.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Usado no cabeçalho de uma solicitação SOAP. Quando esse elemento estiver presente, o chamador está tentando representar a conta que está contida no elemento **ExchangeImpersonation** .  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a>Comentários

A chamada conta deve ter o **ms-exch-impersonation** direto no servidor de acesso para cliente e o **ms-exch-MayImpersonate** direito em ou o banco de dados de caixa de correio que contém a caixa de correio para representar ou o usuário do Active Directory ou um contato objeto. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Autorização de servidor-para-servidor no EWS](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

