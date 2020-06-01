---
title: Conta (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: O elemento Account especifica as configurações de conta do usuário ou contém respostas de erro.
ms.openlocfilehash: ffd8ebe4b7bd9d4b3f6a9b42fc557ac6189a068d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462315"
---
# <a name="account-pox"></a>Conta (POX)

O elemento **Account** especifica as configurações de conta do usuário ou contém respostas de erro. 
  
- [Descoberta automática (POX)](autodiscover-pox.md)
- [Resposta (POX)](response-pox.md)
- [Conta (POX)](account-pox.md)
  
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
|[Ação (POX)](action-pox.md) <br/> |Fornece informações que são usadas para determinar se outra solicitação de descoberta automática é necessária para retornar as informações de configuração do usuário.  <br/> |
|[MicrosoftOnline (POX)](microsoftonline-pox.md) <br/> |Contém um valor que indica se a caixa de correio do usuário está hospedada no Exchange Online ou no Exchange Online como parte do Office 365.  <br/> |
|[RedirectUrl (POX)](redirecturl-pox.md) <br/> |Contém a URL do computador que está executando o Exchange Server que tem a função de servidor de acesso para Cliente instalada que deve ser usada para obter as configurações de descoberta automática.  <br/> |
|[RedirectAddr (POX)](redirectaddr-pox.md) <br/> |Especifica o endereço de email que deve ser usado para uma solicitação de descoberta automática subsequente.  <br/> |
|[Imagem (POX)](image-pox.md) <br/> |Contém o caminho de uma imagem usada para marcar a experiência de configuração.  <br/> |
|[Onhome (POX)](servicehome-pox.md) <br/> |Contém a URL da home page do provedor de serviços de Internet (ISP).  <br/> |
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao servidor de acesso para cliente.  <br/> |
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |Contém informações que os clientes podem usar para enviar uma solicitação de descoberta automática para descobrir informações de pasta pública para o usuário.  <br/> |
|[Erro (POX)](error-pox.md) <br/> |Contém uma resposta de erro de descoberta automática.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Resposta (POX)](response-pox.md) <br/> |Contém a resposta do serviço de descoberta automática.  <br/> |
   
## <a name="see-also"></a>Também consulte

- [Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

