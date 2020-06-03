---
title: Definir a URL do serviço EWS usando a API gerenciada do EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: cddf6525-1c04-484b-a911-56c2f0f1f7b6
description: Encontre informações sobre como definir a URL do serviço do EWS em seu aplicativo de API gerenciada do EWS.
localization_priority: Priority
ms.openlocfilehash: 5ba79b48d4eb4fec62110448c5924de16b67ce10
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456716"
---
# <a name="set-the-ews-service-url-by-using-the-ews-managed-api"></a>Definir a URL do serviço EWS usando a API gerenciada do EWS

Encontre informações sobre como definir a URL do serviço do EWS em seu aplicativo de API gerenciada do EWS.
  
A URL do serviço é o endereço que o Exchange usa para se comunicar com os serviços Web do Exchange (EWS). Após o aplicativo da API gerenciada do EWS ter esse endereço e ter acesso apropriado para [se comunicar com o EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md), ele pode fazer chamadas para a [classe ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx). A URL de serviço de um servidor Exchange local pode ter a aparência a seguir. 
  
```HTML
https://computer.domain.contoso.com/EWS/Exchange.asmx
```

Você pode definir a URL do EWS em seu aplicativo de algumas maneiras. Recomendamos que você use o [serviço de descoberta automática](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx) para obter a URL porque, em uma grande floresta de servidores, a URL poderá ser alterada se a caixa de correio for migrada para outro servidor. No entanto, como chamar a descoberta automática pode levar algum tempo e reduzir o aplicativo se você precisar fazer várias chamadas em um curto período de tempo, talvez queira armazenar em cache o valor da URL obtido da descoberta automática e definir manualmente a URL do serviço do EWS com esse valor em cache. Isso melhorará o desempenho do seu aplicativo; Apenas certifique-se de usar a descoberta automática para atualizar o valor em cache periodicamente, caso o valor mude no servidor. 
  
## <a name="set-the-ews-service-url-by-using-the-autodiscover-service"></a>Definir a URL do serviço do EWS usando o serviço de descoberta automática
<a name="bk_SetURLusingAutoDiscover"> </a>

O método [AutodiscoverUrl](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) usa o endereço de email para definir o ponto de extremidade [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e permite que seu aplicativo use qualquer método incluído nas classes de proxy do **ExchangeService** . O exemplo a seguir mostra como usar o método **AutodiscoverURL** . 
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.AutodiscoverUrl("User1@contoso.com");

```

## <a name="set-the-exchange-service-url-manually"></a>Definir a URL do serviço do Exchange manualmente
<a name="bk_SetURLmanually"> </a>

O exemplo a seguir mostra como definir a URL do serviço do EWS usando um valor em cache. Antes de fazer isso, certifique-se de usar o serviço de descoberta automática para obter a URL do EWS.
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.Url = new Uri("https://computername.domain.contoso.com/EWS/Exchange.asmx");

```

## <a name="see-also"></a>Confira também

- [Introdução aos aplicativos clientes de API gerenciada por EWS](get-started-with-ews-managed-api-client-applications.md)   
- [Configurando seu ambiente de desenvolvimento de aplicativos do Exchange](setting-up-your-exchange-application-development-environment.md)   
- [Controlar o acesso ao EWS no Exchange](how-to-control-access-to-ews-in-exchange.md) 
- [Comunicar-se com o EWS usando a API gerenciada do EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)  
- [Usar a Descoberta Automática para localizar os pontos de conexão](how-to-use-autodiscover-to-find-connection-points.md)
    

