---
title: UserId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserId
api_type:
- schema
ms.assetid: 244af9e0-bf3c-46b4-8bfa-9719a1ed3107
description: O elemento UserId identifica um usuário delegado ou um usuário com permissões de acesso à pasta.
ms.openlocfilehash: 68075e335383835ddce9575d85ba5fa945ed305c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455538"
---
# <a name="userid"></a>UserId

O elemento **userid** identifica um usuário delegado ou um usuário com permissões de acesso à pasta. 
  
```xml
<UserId>
   <SID/>
   <PrimarySmtpAddress/>
   <DisplayName/>
   <DistinguishedUser/>
   <ExternalUserIdentity/>
</UserId>
```

 **UserIdtype**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Identifica](sid.md) <br/> |Representa a forma SDDL (Security Descriptor Definition Language) do identificador de segurança (SID).  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Representa o endereço SMTP (Simple Mail Transfer Protocol) principal de uma conta a ser usada para acesso de representante.  <br/> |
|[DisplayName (cadeia de caracteres)](displayname-string.md) <br/> |Define o nome de exibição de uma pasta, contato, lista de distribuição ou usuário delegado.  <br/> |
|[DistinguishedUser](distinguisheduser.md) <br/> |Identifica contas de usuário anônimas e padrão para acesso de representante.  <br/> |
|[ExternalUserIdentity](externaluseridentity.md) <br/> |Identifica um usuário delegado externo ou um usuário externo com permissões de acesso de pasta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DelegateUser](delegateuser.md) <br/> |Identifica um único representante para adicionar ou atualizar em uma caixa de correio.  <br/> |
|[Permissão](permission.md) <br/> |Define o acesso que um usuário tem a uma pasta.  <br/> |
|[CalendarPermission](calendarpermission.md) <br/> |Define o acesso que um usuário tem a uma pasta de calendário.  <br/> |
|[UserIds](userids.md) <br/> |Contém uma matriz de usuários delegados para obter ou remover da caixa de correio de uma entidade de segurança.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação AddDelegate](adddelegate-operation.md)
  
[Operação UpdateDelegate](updatedelegate-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Adicionar representantes](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

