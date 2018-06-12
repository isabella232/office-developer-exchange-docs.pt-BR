---
title: Tratando erros relacionados a sincronização no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: a0807b90-645a-4ea6-aee1-96828df14be0
description: Descubra como lidar com erros relacionados a sincronização em aplicativos que você desenvolva usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 6de27d585e467d900941f34b2210877d17205502
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750662"
---
# <a name="handling-synchronization-related-errors-in-ews-in-exchange"></a>Tratando erros relacionados a sincronização no EWS no Exchange

Descubra como lidar com erros relacionados a sincronização em aplicativos que você desenvolva usando a API gerenciada de EWS ou EWS no Exchange.
  
Se seu aplicativo sincroniza os itens e pastas, você pode precisar manipular erros de sincronização. Você pode manipular esses erros em tempo de execução ou enquanto desenvolve seu aplicativo do EWS. A maioria desses erros é definida pela enumeração [ResponseCodeType](http://msdn.microsoft.com/en-us/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) na API gerenciada do EWS e o elemento [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) no serviços de Web do Exchange (EWS). 
  
**Tabela 1. Erros de sincronização e como lidar com elas**

|**Erro**|**Ocorre quando você tenta …**|**Manipulá-lo pelo …**|
|:-----|:-----|:-----|
|ErrorInvalidSyncStateData  <br/> | Sincronize itens ou pastas usando-se um valor de estado de sincronização inválidos.  <br/>  Exclua uma pasta raiz na sua solicitação SyncFolderHierarchy inicial, quando sua solicitação subsequente inclui uma pasta raiz.  <br/>  Use pastas raiz diferente em solicitações subsequentes.  <br/> | Garantir que o valor de estado de sincronização que estiver enviando correspondências o valor de estado de sincronização retornados durante uma sincronização anterior.  <br/>  Garantindo que você não está enviando o estado de sincronização para a hierarquia de pasta quando você tenta sincronizar itens e vice-versa.  <br/>  Garantir que você está enviando o estado de sincronização para a pasta raiz correta.  <br/>  Garantir que a mesma pasta raiz está especificada em cada solicitação.  <br/>  Garantir que a solicitação anterior não especificou uma pasta raiz de valor nulo, enquanto a solicitação atual inclui uma pasta raiz de autoridades de raiz. NULL e raiz não são tratados da mesma.  <br/> |
|ErrorSyncFolderNotFound  <br/> |Sincronize subpastas ou itens em uma pasta que não pode ser encontrado no servidor.  <br/> |Garantindo que a pasta especificado na solicitação de ID corresponde a uma ID de pasta retornada do servidor em uma resposta de sincronização anterior.  <br/> |
|ErrorTimeoutExpired  <br/> |Envie muitas solicitações.  <br/> |Limitando seus lotes de 10 itens por lote para evitar obter [limitadas](ews-throttling-in-exchange.md).  <br/> |
|[ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) <br/> |Conecte-se para o EWS quando o servidor está offline ou não há um problema com a conectividade.  <br/> |Verificando a conectividade com o servidor e repetindo a sua solicitação mais tarde. Provavelmente, esse é um erro de serviço transitórios ou erro de rede.  <br/> |
   
## <a name="see-also"></a>Confira também


- [Sincronização de caixa de correio e EWS no Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    
- [Sincronizar pastas usando o EWS no Exchange](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [Sincronizar itens usando o EWS no Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)
    
- [ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)
    

