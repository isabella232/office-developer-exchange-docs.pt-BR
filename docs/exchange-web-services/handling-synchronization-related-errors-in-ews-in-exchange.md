---
title: Como lidar com erros relacionados à sincronização no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: a0807b90-645a-4ea6-aee1-96828df14be0
description: Descubra como lidar com erros relacionados à sincronização em aplicativos que você desenvolve usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: f62937ec444d64b0b358581371f1260f565215b3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455937"
---
# <a name="handling-synchronization-related-errors-in-ews-in-exchange"></a>Como lidar com erros relacionados à sincronização no EWS no Exchange

Descubra como lidar com erros relacionados à sincronização em aplicativos que você desenvolve usando a API gerenciada do EWS ou o EWS no Exchange.
  
Se o aplicativo sincronizar itens e pastas, talvez seja necessário lidar com erros relacionados à sincronização. Você pode manipular esses erros em tempo de execução ou enquanto desenvolve seu aplicativo do EWS. A maioria desses erros é definida pela enumeração [ResponseCodeType](https://msdn.microsoft.com/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) na API gerenciada do EWS e o elemento [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) nos serviços Web do Exchange (EWS). 
  
**Tabela 1. Erros relacionados à sincronização e como tratá-los**

|**Error**|**Ocorre quando você tenta...**|**Manipulá-lo pelo …**|
|:-----|:-----|:-----|
|ErrorInvalidSyncStateData  <br/> | Sincronizar itens ou pastas usando um valor de estado de sincronização inválido.  <br/>  Exclua uma pasta raiz na sua solicitação SyncFolderHierarchy inicial, quando sua solicitação subsequente incluir uma pasta raiz.  <br/>  Usar pastas raiz diferentes em solicitações subsequentes.  <br/> | Garantir que o valor de estado de sincronização que você está enviando corresponde ao valor de estado de sincronização retornado durante uma sincronização anterior.  <br/>  Garantir que você não esteja enviando o estado de sincronização para a hierarquia de pastas ao tentar sincronizar itens e vice-versa.  <br/>  Garantir que você esteja enviando o estado de sincronização para a pasta raiz correta.  <br/>  Garantir que a mesma pasta raiz seja especificada em cada solicitação.  <br/>  Garantir que a solicitação anterior não especificou uma pasta raiz de NULL, enquanto a solicitação atual inclui uma pasta raiz da raiz. NULL e root não são tratados da mesma.  <br/> |
|ErrorSyncFolderNotFound  <br/> |Sincronizar subpastas ou itens em uma pasta que não pode ser encontrado no servidor.  <br/> |Garantir que a ID da pasta especificada na solicitação corresponda a uma ID de pasta retornada do servidor em uma resposta de sincronização anterior.  <br/> |
|ErrorTimeoutExpired  <br/> |Enviar muitas solicitações.  <br/> |Limitar seus lotes a 10 itens por lote para evitar a [limitação](ews-throttling-in-exchange.md).  <br/> |
|[Naresponseexception](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) <br/> |Conecte-se ao EWS quando o servidor está offline ou há um problema com a conectividade.  <br/> |Verificar a conectividade com o servidor e repetir sua solicitação mais tarde. Isso provavelmente é um erro de serviço transitório ou um erro de rede.  <br/> |
   
## <a name="see-also"></a>Confira também


- [Sincronização de caixa de correio e EWS no Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    
- [Sincronizar pastas usando o EWS no Exchange](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [Sincronizar itens usando o EWS no Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)
    
- [Naresponseexception](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)
    

