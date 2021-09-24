---
title: Referência do serviço Web de Descoberta Automática SOAP para Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Encontre informações de referência para o serviço de Descoberta Automática SOAP Exchange.
ms.openlocfilehash: 488862f5797abfd71d33c916fa96970ab300a2c0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521351"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a>Referência do serviço Web de Descoberta Automática SOAP para Exchange

Encontre informações de referência para o serviço de Descoberta Automática SOAP Exchange.
  
O serviço descoberta automática fornece as informações de configuração que seu aplicativo usa para criar uma conexão com um Exchange servidor. Você pode usar o serviço soap Descoberta Automática para enviar mensagens entre o aplicativo cliente e o servidor Exchange para localizar as configurações que o aplicativo usará para se conectar ao Exchange. Ao contrário do serviço de Descoberta Automática da POX, o serviço de Descoberta Automática SOAP permite solicitações de Descoberta Automática em lote para configurações de muitos usuários e controle mais granular sobre quais configurações são retornadas na resposta. 
  
> [!NOTE]
> Para clientes que direcionam versões de Exchange a partir do Exchange Server 2010, recomendamos que você use o serviço de Descoberta Automática SOAP (em vez do serviço de Descoberta Automática POX). Os clientes destinados Exchange 2007 têm que usar o serviço de Descoberta Automática POX. Recomendamos que os clientes que usam o .NET Framework usem a API Gerenciada do EWS porque ela contém um cliente robusto e bem testado de Descoberta Automática SOAP. Para obter mais informações sobre a API Gerenciada do EWS, consulte [Get started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
Esta seção fornece informações sobre os elementos XML que são enviados entre o cliente e o servidor durante redirecionamentos de solicitação de Descoberta Automática SOAP e as configurações do usuário que são retornadas em uma resposta. A referência do elemento XML contém resumos do que os elementos representam e uma descrição das hierarquias de elemento potencial que contêm o elemento. 
  
Os artigos nesta seção descrevem as instâncias XML enviadas entre o cliente e o servidor. O esquema que descreve esses elementos pode ser encontrado no diretório virtual do servidor que hospeda o serviço de Descoberta Automática SOAP.
  
Os tópicos de operação WSDL nesta seção fornecem uma visão geral do que a operação faz e exemplos de solicitação e resposta de operação. Você pode usar as informações de versão fornecidas para determinar se os recursos que você deseja usar estão disponíveis na versão do produto que você está executando. Os exemplos nos tópicos de operação também ajudam você a entender a estrutura do XML incluído nas mensagens SOAP enviadas de e para o servidor.
  
Esta seção também fornece exemplos e descrições das mensagens usadas para recuperar informações de configuração de Descoberta Automática usando o serviço descoberta automática SOAP. 
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_InThisSection"> </a>

- [Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
    
- [Operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
    
- [Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)
    
- [Operação GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)
    
- [Elementos XML de Descoberta Automática SOAP para Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a>Confira também


- [Referência do serviço Web de Descoberta Automática para Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Descoberta Automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Usar a Descoberta Automática para localizar os pontos de conexão](https://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [Obter as configurações de usuário do Exchange usando a Descoberta Automática](https://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [Obter as configurações de domínio de um servidor do Exchange](https://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [Introdução ao uso dos serviços Web no Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

