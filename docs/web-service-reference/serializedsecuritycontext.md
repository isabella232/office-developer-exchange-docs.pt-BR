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
description: O elemento SerializedSecurityContext é usado no cabeçalho SOAP (Simple Object Access Protocol) para serialização de token em autenticação de servidor para servidor. Não há suporte para serialização de token.
ms.openlocfilehash: 58fea1c7f613315d59e81935561f92f318afc769
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462049"
---
# <a name="serializedsecuritycontext"></a>SerializedSecurityContext

O elemento **SerializedSecurityContext** é usado no cabeçalho SOAP (Simple Object Access Protocol) para serialização de token em autenticação de servidor para servidor. Não há suporte para serialização de token. 
  
```xml
<SerializedSecurityContext>
   <UserSid/>
   <GroupSids/>
   <RestrictedGroupSids/>
   <PrimarySmtpAddress/>
</SerializedSecurityContext>
```

 **SerializedSecurityContextType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Userid](usersid.md) <br/> |Representa a forma SDDL (Security Descriptor Definition Language) do identificador de segurança do usuário em um cabeçalho SOAP de contexto de segurança serializado.  <br/> |
|[GroupSids](groupsids.md) <br/> |Representa uma coleção de identificadores de segurança do objeto do grupo de serviços de diretório do Active Directory.  <br/> |
|[RestrictedGroupSids](restrictedgroupsids.md) <br/> |Representa o identificador de segurança do grupo e os atributos de um grupo restrito.  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Representa o endereço SMTP (Simple Mail Transfer Protocol) principal de uma conta a ser usada para a autorização de servidor para servidor.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para cliente (CAS) instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Autorização de servidor para servidor no EWS](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

