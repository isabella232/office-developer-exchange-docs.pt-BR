---
title: Definir a URL de serviço do EWS usando a API gerenciada de EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: cddf6525-1c04-484b-a911-56c2f0f1f7b6
description: Encontre informações sobre como definir a URL do serviço EWS no seu aplicativo do EWS Managed API.
ms.openlocfilehash: e1a414f7c6f13bd61a58403c9d2be546c0226a69
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750819"
---
# <a name="set-the-ews-service-url-by-using-the-ews-managed-api"></a>Definir a URL de serviço do EWS usando a API gerenciada de EWS

Encontre informações sobre como definir a URL do serviço EWS no seu aplicativo do EWS Managed API.
  
A URL do serviço é o endereço que o Exchange usa para se comunicar com o Exchange Web Services (EWS). Depois que seu aplicativo EWS Managed API tem esse endereço e tem o acesso apropriado para [se comunicar com o EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md), ele pode fazer chamadas para a [classe ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx). A URL do serviço para um servidor do Exchange local pode parecer com o seguinte. 
  
```HTML
https://computer.domain.contoso.com/EWS/Exchange.asmx
```

Você pode definir a URL do EWS em seu aplicativo em algumas maneiras. É recomendável que você usar o [serviço de descoberta automática](http://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx) para obter a URL, como em uma floresta grande de servidores, a URL pode ser alterado se a caixa de correio for transferida para outro servidor. No entanto, como chamar a descoberta automática pode levar algum tempo e pode diminuir seu aplicativo se você precisar fazer várias chamadas em um curto período de tempo, talvez você queira cache o valor URL você fazer a partir de descoberta automática e definir manualmente a URL do serviço do EWS com esse cache va Lue. Isso irá melhorar o desempenho do seu aplicativo; apenas certifique-se de que você usar descoberta automática para atualizar seu valor em cache periodicamente caso o valor é alterado no servidor. 
  
## <a name="set-the-ews-service-url-by-using-the-autodiscover-service"></a>Definir a URL de serviço do EWS usando o serviço de descoberta automática
<a name="bk_SetURLusingAutoDiscover"> </a>

O método [AutodiscoverUrl](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) usa o endereço de email para definir o ponto de extremidade [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e habilita o seu aplicativo para usar quaisquer métodos incluídos nas classes proxy **ExchangeService** . O exemplo a seguir mostra como usar o método **AutodiscoverURL** . 
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.AutodiscoverUrl("User1@contoso.com");

```

## <a name="set-the-exchange-service-url-manually"></a>Definir a URL do serviço Exchange manualmente
<a name="bk_SetURLmanually"> </a>

O exemplo a seguir mostra como definir a URL do serviço EWS utilizando-se um valor em cache. Antes de fazer isso, verifique se usar o serviço Descoberta automática para obter a URL do EWS.
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.Url = new Uri("https://computername.domain.contoso.com/EWS/Exchange.asmx");

```

## <a name="see-also"></a>Confira também

- [Introdução aos aplicativos de cliente API gerenciada de EWS](get-started-with-ews-managed-api-client-applications.md)   
- [Configurando o ambiente de desenvolvimento de aplicativos do Exchange](setting-up-your-exchange-application-development-environment.md)   
- [Controlar o acesso a EWS no Exchange](how-to-control-access-to-ews-in-exchange.md) 
- [Comunicar-se com o EWS usando a API gerenciada de EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)  
- [Usar descoberta automática para encontrar os pontos de conexão](how-to-use-autodiscover-to-find-connection-points.md)
    

