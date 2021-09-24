---
title: Arquivamento no EWS em Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 78ae179b-ae4f-4f64-911a-e0c70e0fa314
description: Saiba mais sobre arquivamento no EWS Exchange.
ms.openlocfilehash: f2ca4cc783556b089b732c75d166b77c0dcd891c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520224"
---
# <a name="archiving-in-ews-in-exchange"></a>Arquivamento no EWS em Exchange

Saiba mais sobre arquivamento no EWS Exchange.
  
As caixas de correio de arquivo morto são caixas de correio secundárias associadas a um usuário. As caixas de correio de arquivo morto geralmente são usadas para gerenciar limites de armazenamento de email. Por exemplo, itens de email mais antigos podem ser movidos periodicamente da Caixa de Entrada para a caixa de correio de arquivo morto. 
  
Exchange Online, Exchange Online como parte do Office 365 e o Exchange Server 2013 introduzem duas novas operações do Exchange Web Services (EWS) que você pode usar para arquivar um conjunto de itens de email de uma caixa de correio principal. Arquivando itens de Caixa de Entrada dessa forma preserva a hierarquia de pastas dos itens. Além disso, as caixas de correio de arquivo morto agora podem ser armazenadas localmente em um cliente ou remotamente, de forma que seja principalmente opaca para um usuário, usando um caminho de pasta para apontar para o conteúdo do arquivo morto.
  
## <a name="archiving-operations-in-ews"></a>Operações de arquivamento no EWS

A tabela a seguir lista as operações de arquivamento introduzidas no Exchange 2013. 
  
|**Nome da operação**|**Descrição**|
|:-----|:-----|
|[ArchiveItem](https://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |Move um item da caixa de correio principal para a caixa de correio de arquivo morto.  <br/> |
|[CreateFolderPath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |Cria um URI que aponta para o local de armazenamento da caixa de correio de arquivo morto.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Desenvolver clientes do serviço Web para o Exchange](develop-web-service-clients-for-exchange.md)
    
- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
    
- [Visão geral de design do cliente EWS para o Exchange](ews-client-design-overview-for-exchange.md)
    

