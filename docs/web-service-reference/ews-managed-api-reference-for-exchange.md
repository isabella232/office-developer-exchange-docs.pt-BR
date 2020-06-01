---
title: Referência da API gerenciada do EWS (Serviços Web do Exchange)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
api_type:
- schema
ms.assetid: c6ca36f4-a67c-4e3c-aae7-9ead7b704e15
description: Saiba mais sobre os namespaces incluídos na API gerenciada do EWS.
localization_priority: Priority
ms.openlocfilehash: aa5dd71bf1e9962611a8ea8471aca0c60aa232e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466749"
---
# <a name="ews-managed-api-reference"></a>Referência de API gerenciada do EWS

**Aplica-se à**: API gerenciada do EWS | Exchange Online | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 | Office 365

A API gerenciada do EWS (Serviços Web do Exchange) inclui duas APIs: Microsoft.Exchange.WebServices.dll e Microsoft.Exchange.WebServices.Auth.dll.

## <a name="ews-managed-api-namespaces"></a>Namespaces da API gerenciada do EWS

|Namespace |Descrição |
|:---------|:-----------|
|[Microsoft.Exchange.WebServices.Auth.Validation](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.auth.validation?view=exchange-ews-api) |Contém tipos e métodos usados para validar tokens de identidade do usuário enviados de um servidor Exchange. O namespace Microsoft.Exchange.WebServices.Auth.Validation se aplica a clientes que direcionam o Exchange Online e versões do Exchange a partir do Exchange Server 2013. Esse namespace está incluído na API Microsoft.Exchange.WebServices.Auth.dll.|
|[Microsoft.Exchange.WebServices.Autodiscover](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.autodiscover?view=exchange-ews-api)|Contém tipos usados para se comunicar com o serviço Descoberta Automática hospedado por um Exchange Server. Esse namespace também é usado para procurar objetos de ponto de conexão do serviço no AD DS (Active Directory Domain Services). Os serviços Descoberta Automática fornecem informações de configuração para clientes do EWS. Isso permite que os clientes direcionem a URL do serviço apropriado.<br/><br/>A funcionalidade namespace pode ser usada para direcionar o serviço Descoberta Automática POX introduzido no Microsoft Exchange Server 2007, a pesquisa de objeto de ponto de conexão do serviço se o cliente ingressou no domínio ou o ponto de extremidade SOAP de Descoberta Automática introduzido no Exchange Server 2010. O tipo principal nesse namespace é a classe [AutodiscoverService](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.autodiscover.autodiscoverservice?view=exchange-ews-api). Esse namespace está incluído na API Microsoft.Exchange.WebServices.dll.|
|[Microsoft.Exchange.WebServices.Data](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data?view=exchange-ews-api)| Contém tipos usados para se comunicar com o servidor Exchange por meio do EWS. Esse namespace fornece a principal funcionalidade da API gerenciada do EWS. O tipo principal nesse namespace é a classe [ExchangeService](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.exchangeservice?view=exchange-ews-api).|

## <a name="see-also"></a>Confira também

- [Referência de serviço Web do Exchange](web-services-reference-for-exchange.md)
- [Explorar os recursos da API gerenciada por EWS, EWS e serviços Web no Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Novidades no EWS e outros serviços Web no Exchange](../exchange-web-services/whats-new-in-ews-and-other-web-services-in-exchange.md)
- [Introdução ao uso dos serviços Web no Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Develop web service clients for Exchange](../exchange-web-services/develop-web-service-clients-for-exchange.md)

