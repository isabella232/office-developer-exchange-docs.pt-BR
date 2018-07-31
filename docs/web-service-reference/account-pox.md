---
title: Account (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: O elemento de conta Especifica as configurações da conta do usuário ou contém respostas de erro.
ms.openlocfilehash: 6cd87e678b3a524a69f6dca4d6999a3cff22fa57
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353340"
---
# <a name="account-pox"></a>Account (POX)

O elemento de **conta** Especifica as configurações da conta do usuário ou contém respostas de erro. 
  
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

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AccountType (POX)](accounttype-pox.md) <br/> |Representa o tipo de conta.  <br/> |
|[Action (POX)](action-pox.md) <br/> |Fornece informações que são usadas para determinar se outra solicitação de descoberta automática é necessária para retornar as informações de configuração do usuário.  <br/> |
|[MicrosoftOnline (POX)](microsoftonline-pox.md) <br/> |Contém um valor que indica se caixas de correio do usuário está hospedada no Exchange Online ou Exchange Online como parte do Office 365.  <br/> |
|[RedirectUrl (POX)](redirecturl-pox.md) <br/> |Contém a URL do computador que está executando o Exchange Server que possui a função de servidor do acesso para cliente instalada deve ser usada para obter as configurações de descoberta automática.  <br/> |
|[RedirectAddr (POX)](redirectaddr-pox.md) <br/> |Especifica o endereço de email que deve ser usado para uma solicitação de descoberta automática subsequente.  <br/> |
|[Image (POX)](image-pox.md) <br/> |Contém o caminho de uma imagem que é usado para marcar a experiência de configuração.  <br/> |
|[ServiceHome (POX)](servicehome-pox.md) <br/> |Contém a URL da home page do provedor de serviços de Internet (ISP).  <br/> |
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente para o servidor de acesso para cliente.  <br/> |
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |Contém informações que os clientes podem usar para enviar uma solicitação de descoberta automática para descobrir informações de pasta pública para o usuário.  <br/> |
|[Error (POX)](error-pox.md) <br/> |Contém uma resposta de erro de descoberta automática.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Response (POX)](response-pox.md) <br/> |Contém a resposta do serviço de descoberta automática.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

