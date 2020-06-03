---
title: Arquivamento no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78ae179b-ae4f-4f64-911a-e0c70e0fa314
description: Saiba mais sobre o arquivamento no EWS no Exchange.
ms.openlocfilehash: b433b9f88905ee255720e8b341d560fa0e464975
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456210"
---
# <a name="archiving-in-ews-in-exchange"></a>Arquivamento no EWS no Exchange

Saiba mais sobre o arquivamento no EWS no Exchange.
  
Caixas de correio de arquivo morto são caixas de correio secundárias associadas a um usuário. As caixas de correio de arquivo morto normalmente são usadas para gerenciar limites de armazenamento de email. Por exemplo, os itens de email mais antigos podem ser movidos periodicamente da caixa de entrada para a caixa de correio de arquivo morto. 
  
O Exchange Online, o Exchange Online como parte do Office 365 e o Exchange Server 2013 apresentam duas novas operações do EWS (serviços Web do Exchange) que você pode usar para arquivar um conjunto de itens de email de uma caixa de correio principal. O arquivamento de itens da caixa de entrada dessa forma preserva a hierarquia de pastas dos itens. Além disso, as caixas de correio de arquivo morto agora podem ser armazenadas localmente em um cliente ou remotamente, de modo mais opaco para um usuário, usando um caminho de pasta para apontar para o conteúdo do arquivo morto.
  
## <a name="archiving-operations-in-ews"></a>Operações de arquivamento no EWS

A tabela a seguir lista as operações de arquivamento que foram introduzidas no Exchange 2013. 
  
|**Nome da operação**|**Descrição**|
|:-----|:-----|
|[ArchiveItem](https://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |Move um item da caixa de correio principal para a caixa de correio de arquivo morto.  <br/> |
|[Createfolderpath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |Cria um URI que aponta para o local de armazenamento da caixa de correio de arquivo morto.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
    
- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)
    

