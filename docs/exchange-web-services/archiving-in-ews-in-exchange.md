---
title: Arquivamento no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78ae179b-ae4f-4f64-911a-e0c70e0fa314
description: Saiba mais sobre o arquivamento no EWS no Exchange.
ms.openlocfilehash: bc282a7774bb74e57550bc663512987839324b83
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750639"
---
# <a name="archiving-in-ews-in-exchange"></a>Arquivamento no EWS no Exchange

Saiba mais sobre o arquivamento no EWS no Exchange.
  
Caixas de correio de arquivo morto são secundárias caixas de correio que estão associadas um usuário. Caixas de correio de arquivo morto são geralmente usadas para gerenciar os limites de armazenamento de email. Por exemplo, itens de email mais antigos periodicamente talvez seja movidos de caixa de entrada para a caixa de correio de arquivo morto. 
  
O Exchange Online, Exchange Online como parte do Office 365 e Exchange Server 2013 introduz duas novas operações de serviços Web do Exchange (EWS) que você pode usar para arquivar um conjunto de itens de email de uma caixa de correio principal. Arquivamento de itens de caixa de entrada dessa maneira preserva a hierarquia de pastas dos itens. Além disso, as caixas de correio de arquivo morto agora podem ser armazenadas localmente em um cliente, ou remotamente, de forma que é opaca a um usuário, principalmente por meio de um caminho de pasta para apontar para o conteúdo do arquivamento.
  
## <a name="archiving-operations-in-ews"></a>Operações de arquivamento no EWS

A tabela a seguir lista as operações de arquivamento que foram introduzidas no Exchange 2013. 
  
|**Nome da operação**|**Descrição**|
|:-----|:-----|
|[ArchiveItem](http://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |Move um item da caixa de correio principal para a caixa de correio de arquivo morto.  <br/> |
|[CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |Cria um URI que aponta para o local de armazenamento para a caixa de correio de arquivo morto.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Start using web services in Exchange](start-using-web-services-in-exchange.md)
    
- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md)
    

