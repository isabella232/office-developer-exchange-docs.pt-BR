---
title: Requisitos de redistribuição para a API gerenciada de EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: Descubra como você pode redistribuir os assemblies de API gerenciada de EWS com seu aplicativo.
ms.openlocfilehash: d8fc57c4a2b3ed7d6218aeeed0fe88c2d3e0fbe0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750946"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a>Requisitos de redistribuição para a API gerenciada de EWS

Descubra como você pode redistribuir os assemblies de API gerenciada de EWS com seu aplicativo.
  
Como criar seu aplicativo EWS Managed API, também desejará considerar como você irá liberá-la para seus usuários. 
  
## <a name="redistributing-your-ews-managed-api-application"></a>Redistribuir seu aplicativo API gerenciada de EWS

A menos que o aplicativo está localizado no servidor do Exchange, você precisará redistribuir os assemblies de API gerenciada de EWS. O download do EWS Managed API contém dois assemblies que você pode redistribuir: Microsoft.Exchange.WebServices.dll e Microsoft.Exchange.WebServices.Auth.dll. Lembre-se das seguintes informações ao criar como lançará seu aplicativo API gerenciada de EWS:
  
- A API gerenciada de EWS foi projetada, de forma que você pode baixá-lo e distribuí-lo com o seu aplicativo que tem como destino um servidor Exchange. Como alternativa, seu aplicativo pode baixar o EWS Managed API.
    
- Você pode usar a API gerenciada de EWS para se comunicar com um servidor do Exchange executando o Exchange Online, Exchange Online como parte do Office 365 ou uma versão local do Exchange, começando com o Exchange Server 2007.
    
- Nas versões do EWS Managed API começando com a versão 2.1, você pode instalar a API no Cache de Assembly Global (GAC). O MSI adicionará automaticamente a DLL no GAC e será acessível no computador por computador, não em uma base por usuário.
    
Os termos de licença são incluídos no download do EWS Managed API. Analise os termos para obter as informações autoritativas sobre o que você pode fazer com a API gerenciada de EWS.
  
## <a name="see-also"></a>Confira também


- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md)
    
- [API gerenciada de EWS (download)](http://aka.ms/ews-managed-api-readme)
    

