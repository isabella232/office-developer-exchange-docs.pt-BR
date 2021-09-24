---
title: Lidar com erros relacionados à sincronização no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: a0807b90-645a-4ea6-aee1-96828df14be0
description: Saiba como lidar com erros relacionados à sincronização em aplicativos que você desenvolve usando a API Gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: fd52b54413c6fc791132fb01b47bc9077d0266b2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513245"
---
# <a name="handling-synchronization-related-errors-in-ews-in-exchange"></a>Lidar com erros relacionados à sincronização no EWS no Exchange

Saiba como lidar com erros relacionados à sincronização em aplicativos que você desenvolve usando a API Gerenciada do EWS ou o EWS no Exchange.
  
Se o aplicativo sincronizar itens e pastas, talvez seja preciso lidar com erros relacionados à sincronização. Você pode manipular esses erros em tempo de execução ou enquanto desenvolve seu aplicativo do EWS. A maioria desses erros é definida pela enumeração [ResponseCodeType](https://msdn.microsoft.com/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) na API Gerenciada do EWS e pelo elemento [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) no Exchange Web Services (EWS). 
  
**Tabela 1. Erros relacionados à sincronização e como lidar com eles**

|**Erro**|**Ocorre quando você tenta...**|**Manipulá-lo pelo …**|
|:-----|:-----|:-----|
|ErrorInvalidSyncStateData  <br/> | Sincronizar itens ou pastas usando um valor de estado de sincronização inválido.  <br/>  Exclua uma pasta raiz em sua solicitação syncFolderHierarchy inicial, quando sua solicitação subsequente incluir uma pasta raiz.  <br/>  Use pastas raiz diferentes em solicitações subsequentes.  <br/> | Garantir que o valor do estado de sincronização que você está enviando corresponde ao valor de estado de sincronização retornado durante uma sincronização anterior.  <br/>  Garantindo que você não está enviando o estado de sincronização para a hierarquia de pastas ao tentar sincronizar itens e vice-versa.  <br/>  Garantindo que você está enviando o estado de sincronização para a pasta raiz correta.  <br/>  Garantindo que a mesma pasta raiz seja especificada em cada solicitação.  <br/>  Garantindo que a solicitação anterior não especifique uma pasta raiz de null, enquanto a solicitação atual inclui uma pasta raiz de raiz. Null e root não são tratados da mesma forma.  <br/> |
|ErrorSyncFolderNotFound  <br/> |Sincronizar subpastas ou itens em uma pasta que não pode ser encontrada no servidor.  <br/> |Garantindo que a ID da pasta especificada na solicitação corresponde a uma ID de pasta retornada do servidor em uma resposta de sincronização anterior.  <br/> |
|ErrorTimeoutExpired  <br/> |Envie muitas solicitações.  <br/> |Limitar seus lotes a 10 itens por lote para evitar ser [limitado.](ews-throttling-in-exchange.md)  <br/> |
|[ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) <br/> |Conexão para o EWS quando o servidor estiver offline ou houver um problema com a conectividade.  <br/> |Verificando a conectividade com o servidor e tentando novamente sua solicitação posteriormente. É provável que seja um erro de serviço transitório ou um erro de rede.  <br/> |
   
## <a name="see-also"></a>Confira também


- [Sincronização de caixa de correio e EWS no Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    
- [Sincronizar pastas usando o EWS em Exchange](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [Sincronizar itens usando o EWS no Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)
    
- [ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)
    

