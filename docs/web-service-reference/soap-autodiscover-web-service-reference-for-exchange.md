---
title: SOAP referência de serviço web de descoberta automática do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Encontre informações de referência para o serviço de descoberta automática do SOAP no Exchange.
ms.openlocfilehash: 1cb24a8667c71028f3dead78d9fa533dc9547a64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825514"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a>SOAP referência de serviço web de descoberta automática do Exchange

Encontre informações de referência para o serviço de descoberta automática do SOAP no Exchange.
  
O serviço de descoberta automática fornece as informações de configuração que o aplicativo usa para criar uma conexão a um servidor Exchange. Você pode usar o serviço Descoberta automática do SOAP para enviar mensagens entre o aplicativo cliente e o servidor do Exchange para localizar as configurações que o aplicativo usará para se conectar ao Exchange. Ao contrário do serviço de descoberta automática de POX, o serviço Descoberta automática do SOAP permite solicitações de descoberta automática em lote para configurações de muitos usuários e controle mais específico sobre quais configurações são retornadas na resposta. 
  
> [!NOTE]
> Para clientes que têm como alvo versões do Exchange, começando com o Exchange Server 2010, recomendamos que você use o serviço de descoberta automática de SOAP (em vez do serviço de descoberta automática de POX). Clientes que visam o Exchange 2007 tem que usar o serviço Descoberta automática de POX. É recomendável que os clientes que usam o .NET Framework usam a API gerenciada de EWS, porque ele contém um cliente de descoberta automática do SOAP robusto e bem testado. Para obter mais informações sobre a API gerenciada de EWS, consulte [Introdução ao aplicativos cliente do EWS Managed API](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
Esta seção fornece informações sobre os elementos XML que são enviados entre o cliente e o servidor durante os redirecionamentos de solicitação de descoberta automática do SOAP e as configurações de usuário que são retornadas em uma resposta. A referência do elemento XML contém resumos dos quais representam os elementos e uma descrição das hierarquias de elemento potenciais que contenham o elemento. 
  
Os artigos nesta seção descrevem as instâncias XML que são enviadas entre o cliente e servidor. O esquema que descreve esses elementos pode ser encontrado no diretório virtual do servidor que hospeda o serviço Descoberta automática do SOAP.
  
A operação WSDL tópicos nesta seção fornecem que uma visão geral dos qual a operação e exemplos de solicitação e a resposta de operação. Você pode usar as informações de versão fornecidas para determinar se os recursos que você deseja usar estão disponíveis no qual você está executando a versão do produto. Os exemplos nos tópicos a operação também ajudarão-lo a compreender a estrutura do XML que está incluído nas mensagens SOAP que são enviadas para e do servidor.
  
Esta seção também fornece exemplos e descrições das mensagens que são usadas para recuperar informações de configuração de descoberta automática usando o serviço de descoberta automática do SOAP. 
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_InThisSection"> </a>

- [Operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
    
- [Operação de GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
    
- [Operação de GetUserSettings (SOAP)](getusersettings-operation-soap.md)
    
- [Operação de GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)
    
- [Elementos de Autodiscover XML SOAP para o Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a>Confira também


- [Referência de web service de descoberta automática do Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Descoberta Automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Usar descoberta automática para encontrar os pontos de conexão](http://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [Obter configurações de usuário do Exchange usando a descoberta automática](http://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [Fazer configurações de domínio a partir de um servidor do Exchange](http://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [Start using web services in Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

