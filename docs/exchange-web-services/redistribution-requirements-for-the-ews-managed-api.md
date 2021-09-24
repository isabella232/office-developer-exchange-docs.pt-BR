---
title: Requisitos de redistribuição para a API Gerenciada do EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: Descubra como você pode redistribuir os assemblies da API Gerenciada do EWS com seu aplicativo.
ms.openlocfilehash: f43156838c735cfc17106deb7860329d3da6c07a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531327"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a>Requisitos de redistribuição para a API Gerenciada do EWS

Descubra como você pode redistribuir os assemblies da API Gerenciada do EWS com seu aplicativo.
  
À medida que você projeta seu aplicativo de API Gerenciada do EWS, você também vai querer considerar como você o liberará para seus usuários. 
  
## <a name="redistributing-your-ews-managed-api-application"></a>Redistribuir seu aplicativo de API Gerenciada do EWS

A menos que seu aplicativo esteja localizado no servidor Exchange, você precisará redistribuir os assemblies da API Gerenciada do EWS. O download da API Gerenciada do EWS contém dois assemblies que você pode redistribuir: Microsoft.Exchange.WebServices.dll e Microsoft.Exchange.WebServices.Auth.dll. Lembre-se das seguintes informações ao projetar como liberará seu aplicativo de API Gerenciada do EWS:
  
- A API Gerenciada do EWS foi projetada para que você possa baixá-la e distribuí-la com seu aplicativo destinado a um Exchange servidor. Como alternativa, seu aplicativo pode baixar a API Gerenciada do EWS.
    
- Você pode usar a API Gerenciada do EWS para se comunicar com um servidor Exchange executando Exchange Online, Exchange Online como parte do Office 365 ou uma versão local do Exchange a partir do Exchange Server 2007.
    
- Em versões da API Gerenciada do EWS a partir da versão 2.1, você pode instalar a API no Cache de Assembly Global (GAC). O MSI adicionará automaticamente a DLL ao GAC e será acessível por computador, não por usuário.
    
Os termos de licença estão incluídos no download da API Gerenciada do EWS. Revise os termos das informações autoritativas sobre o que você pode fazer com a API Gerenciada do EWS.
  
## <a name="see-also"></a>Confira também


- [Visão geral de design do cliente EWS para o Exchange](ews-client-design-overview-for-exchange.md)
    
- [API Gerenciada do EWS (download)](https://aka.ms/ews-managed-api-readme)
    

