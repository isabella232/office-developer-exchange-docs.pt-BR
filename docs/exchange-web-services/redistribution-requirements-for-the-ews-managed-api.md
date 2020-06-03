---
title: Requisitos de redistribuição para a API gerenciada do EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: Descubra como você pode redistribuir os assemblies da API gerenciada do EWS com seu aplicativo.
ms.openlocfilehash: e64b4cdb8938caa819ba30621112a25946ef0424
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463822"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a>Requisitos de redistribuição para a API gerenciada do EWS

Descubra como você pode redistribuir os assemblies da API gerenciada do EWS com seu aplicativo.
  
À medida que você projeta seu aplicativo de API gerenciada do EWS, você também deve considerar como você irá liberá-lo para seus usuários. 
  
## <a name="redistributing-your-ews-managed-api-application"></a>Redistribuindo seu aplicativo de API gerenciada do EWS

A menos que seu aplicativo esteja localizado no servidor Exchange, será necessário redistribuir os assemblies da API gerenciada do EWS. O download da API gerenciada do EWS contém dois assemblies que você pode redistribuir: Microsoft. Exchange. WebServices. dll e Microsoft. Exchange. WebServices. auth. dll. Tenha em mente as seguintes informações ao projetar como você vai liberar seu aplicativo de API gerenciada do EWS:
  
- A API gerenciada do EWS foi projetada para que você possa baixá-lo e distribuí-lo com o aplicativo que tem como alvo um servidor Exchange. Como alternativa, seu aplicativo pode baixar a API gerenciada do EWS.
    
- Você pode usar a API gerenciada do EWS para se comunicar com um servidor Exchange executando o Exchange Online, o Exchange Online como parte do Office 365 ou uma versão local do Exchange a partir do Exchange Server 2007.
    
- Nas versões da API gerenciada do EWS que começam com a versão 2,1, você pode instalar a API no cache de assembly global (GAC). O MSI adicionará automaticamente a DLL ao GAC e estará acessível em cada computador, e não em uma base por usuário.
    
Os termos de licença estão incluídos no download da API gerenciada do EWS. Revise os termos das informações autoritativas sobre o que você pode fazer com a API gerenciada do EWS.
  
## <a name="see-also"></a>Confira também


- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)
    
- [API gerenciada do EWS (download)](https://aka.ms/ews-managed-api-readme)
    

