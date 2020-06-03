---
title: Referência de serviço Web de descoberta automática do SOAP para Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Encontre informações de referência para o serviço de descoberta automática do SOAP no Exchange.
ms.openlocfilehash: bfca8e8e260a6262d12542bd6834894a2375453f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468422"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a>Referência de serviço Web de descoberta automática do SOAP para Exchange

Encontre informações de referência para o serviço de descoberta automática do SOAP no Exchange.
  
O serviço de descoberta automática fornece as informações de configuração que o aplicativo usa para criar uma conexão com um servidor Exchange. Você pode usar o serviço de descoberta automática do SOAP para enviar mensagens entre o aplicativo cliente e o servidor do Exchange para localizar as configurações que o aplicativo usará para se conectar ao Exchange. Ao contrário do serviço de descoberta automática do POX, o serviço de descoberta automática do SOAP permite solicitações de descoberta automática em lote para muitas configurações de usuários e um controle mais granular sobre quais configurações são retornadas na resposta. 
  
> [!NOTE]
> Para clientes que direcionam versões do Exchange a partir do Exchange Server 2010, recomendamos que você use o serviço de descoberta automática do SOAP (em vez do serviço de descoberta automática do POX). Os clientes que direcionam o Exchange 2007 precisam usar o serviço de descoberta automática do POX. Recomendamos que os clientes que usam o .NET Framework usem a API gerenciada do EWS, já que contenha um cliente de descoberta automática do SOAP robusto e bem testado. Para obter mais informações sobre a API gerenciada do EWS, confira [introdução aos aplicativos clientes de API gerenciada do EWS](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
Esta seção fornece informações sobre os elementos XML que são enviados entre o cliente e o servidor durante as redirecionamentos de solicitação de descoberta automática de SOAP e as configurações de usuário retornadas em uma resposta. A referência do elemento XML contém resumos dos elementos que representam e uma descrição das possíveis hierarquias de elemento que contêm o elemento. 
  
Os artigos desta seção descrevem as instâncias XML que são enviadas entre o cliente e o servidor. O esquema que descreve esses elementos pode ser encontrado no diretório virtual do servidor que hospeda o serviço de descoberta automática do SOAP.
  
Os tópicos de operação WSDL nesta seção fornecem uma visão geral do que a operação faz e dos exemplos de resposta e solicitação de operação. Você pode usar as informações de versão fornecidas para determinar se os recursos que você deseja usar estão disponíveis na versão do produto que você está executando. Os exemplos nos tópicos de operação também ajudam a entender a estrutura do XML que está incluída nas mensagens SOAP que são enviadas para e do servidor.
  
Esta seção também fornece exemplos e descrições das mensagens usadas para recuperar as informações de configuração da descoberta automática usando o serviço de descoberta automática SOAP. 
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_InThisSection"> </a>

- [Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
    
- [Operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
    
- [Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)
    
- [Operação GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)
    
- [Elementos XML de descoberta automática SOAP para o Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a>Confira também


- [Referência do serviço Web de descoberta automática do Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Descoberta Automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Usar a Descoberta Automática para localizar os pontos de conexão](https://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [Obter as configurações de usuário do Exchange usando a Descoberta Automática](https://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [Obter as configurações de domínio de um servidor do Exchange](https://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [Introdução ao uso dos serviços Web no Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

