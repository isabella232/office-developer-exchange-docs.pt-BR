---
title: SerializedSecurityContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SerializedSecurityContext
api_type:
- schema
ms.assetid: a02c4fc1-ed1a-40d9-a18e-6cfdae21a690
description: O elemento SerializedSecurityContext é usado no cabeçalho simples (SOAP Object Access Protocol) para serialização de token de autenticação de servidor-para-servidor. Serialização de token não é suportada.
ms.openlocfilehash: c5590551dc0780d918b05902e4f48fb9d1390b59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825363"
---
# <a name="serializedsecuritycontext"></a>SerializedSecurityContext

O elemento **SerializedSecurityContext** é usado no cabeçalho simples (SOAP Object Access Protocol) para serialização de token de autenticação de servidor-para-servidor. Serialização de token não é suportada. 
  
```xml
<SerializedSecurityContext>
   <UserSid/>
   <GroupSids/>
   <RestrictedGroupSids/>
   <PrimarySmtpAddress/>
</SerializedSecurityContext>
```

 **SerializedSecurityContextType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UserSid](usersid.md) <br/> |Representa o formato segurança descritor definition language (SDDL) o identificador de segurança do usuário em um cabeçalho SOAP de contexto de segurança serializados.  <br/> |
|[GroupSids](groupsids.md) <br/> |Representa uma coleção de identificadores de segurança do objeto de grupo do Active Directory directory service.  <br/> |
|[RestrictedGroupSids](restrictedgroupsids.md) <br/> |Representa o identificador de segurança de grupo e os atributos de um grupo restrito.  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Representa o endereço de Simple Mail Transfer Protocol (SMTP) principal de uma conta que serão usados para autorização de servidor-para-servidor.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor (CAS) de acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Autorização de servidor-para-servidor no EWS](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

