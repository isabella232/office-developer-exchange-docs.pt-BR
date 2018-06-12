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
description: O elemento UserId identifica um usuário delegado ou um usuário que tem permissões de acesso de pasta.
ms.openlocfilehash: 8e9867f5a8cdd62dd2dae55fbf527595ac14f46d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837981"
---
# <a name="userid"></a>UserId

O elemento **UserId** identifica um usuário delegado ou um usuário que tem permissões de acesso de pasta. 
  
```xml
<UserId>
   <SID/>
   <PrimarySmtpAddress/>
   <DisplayName/>
   <DistinguishedUser/>
   <ExternalUserIdentity/>
</UserId>
```

 **UserIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SID](sid.md) <br/> |Representa o formulário de segurança descritor definition language (SDDL) do identificador de segurança (SID).  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Representa o endereço de Simple Mail Transfer Protocol (SMTP) principal de uma conta a ser usada para acesso de representante.  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |Define o nome de exibição de uma pasta, contatos, lista de distribuição ou usuário delegado.  <br/> |
|[DistinguishedUser](distinguisheduser.md) <br/> |Identifica as contas de usuário anônimo e padrão para acesso de representante.  <br/> |
|[ExternalUserIdentity](externaluseridentity.md) <br/> |Identifica um usuário delegado externo ou um usuário externo que tem permissões de acesso de pasta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DelegateUser](delegateuser.md) <br/> |Identifica um único representante para adicionar ou atualizar em uma caixa de correio.  <br/> |
|[Permissão](permission.md) <br/> |Define o que um usuário tem acesso a uma pasta.  <br/> |
|[CalendarPermission](calendarpermission.md) <br/> |Define o que um usuário tem acesso a uma pasta de calendário.  <br/> |
|[UserIds](userids.md) <br/> |Contém uma matriz de usuários do representante para obter ou remova a caixa de correio da entidade de segurança.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
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



[Operação AddDelegate](adddelegate-operation.md)
  
[Operação UpdateDelegate](updatedelegate-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Adicionando representantes](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

