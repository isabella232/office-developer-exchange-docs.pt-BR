---
title: Account (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: O elemento Account especifica configurações de conta para o usuário ou contém respostas de erro.
ms.openlocfilehash: 89799ab62a2aa4945b0e8f3209ab1fbc7d2fa2e6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534050"
---
# <a name="account-pox"></a>Account (POX)

O **elemento Account** especifica configurações de conta para o usuário ou contém respostas de erro. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
- [Response (POX)](response-pox.md)
- [Account (POX)](account-pox.md)
  
```XML
<Account>
   <AccountType/>
   <Action/>
   <MicrosoftOnline/>
   <RedirectURL/>
   <RedirectAddr/>
   <Image/>
   <ServiceHome/>
   <Protocol/>
   <PublicFolderInformation/>
</Account>
```

<br/>

```XML
<Account> 
    <Error/> 
</Account>
```

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AccountType (POX)](accounttype-pox.md) <br/> |Representa o tipo de conta.  <br/> |
|[Action (POX)](action-pox.md) <br/> |Fornece informações usadas para determinar se outra solicitação de Descoberta Automática é necessária para retornar as informações de configuração do usuário.  <br/> |
|[MicrosoftOnline (POX)](microsoftonline-pox.md) <br/> |Contém um valor que indica se a caixa de correio do usuário está hospedada no Exchange Online ou Exchange Online como parte do Office 365.  <br/> |
|[RedirectUrl (POX)](redirecturl-pox.md) <br/> |Contém a URL do computador que está executando Exchange Server que tem a função de servidor de Acesso para Cliente instalada que deve ser usada para obter configurações de Descoberta Automática.  <br/> |
|[RedirectAddr (POX)](redirectaddr-pox.md) <br/> |Especifica o endereço de email que deve ser usado para uma solicitação de Descoberta Automática subsequente.  <br/> |
|[Image (POX)](image-pox.md) <br/> |Contém o caminho de uma imagem usada para identidade visual da experiência de configuração.  <br/> |
|[ServiceHome (POX)](servicehome-pox.md) <br/> |Contém a URL da home page do provedor de serviços da Internet (ISP).  <br/> |
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao servidor de Acesso para Cliente.  <br/> |
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |Contém informações que os clientes podem usar para enviar uma solicitação de Descoberta Automática para descobrir informações de pasta pública para o usuário.  <br/> |
|[Error (POX)](error-pox.md) <br/> |Contém uma resposta de erro de Descoberta Automática.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Response (POX)](response-pox.md) <br/> |Contém a resposta do serviço descoberta automática.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

