---
title: Atualizar informações de configuração usando a Descoberta Automática
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: c2f3c6a5-e8ea-4375-b41a-686a6f238d33
description: Saiba como e quando atualizar informações de configuração para sua conexão Exchange usando a Descoberta Automática.
ms.openlocfilehash: 0ec6910fcd8ab66085de2414f02a4f78419ec78b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513112"
---
# <a name="refresh-configuration-information-by-using-autodiscover"></a>Atualizar informações de configuração usando a Descoberta Automática

Saiba como e quando atualizar informações de configuração para sua conexão Exchange usando a Descoberta Automática.
  
Quando seu aplicativo EWS é executado pela primeira vez, a Descoberta Automática fornece uma ótima maneira de coletar as informações necessárias para se conectar à caixa de correio de Exchange do usuário. Mas a Descoberta Automática não é apenas para uso pela primeira vez. Usar a Descoberta Automática regularmente pode ajudar a manter seu aplicativo conectado, permitindo que ele responda a alterações na implantação Exchange.
  
## <a name="cache-autodiscover-endpoint-and-ews-settings"></a>Cache Autodiscover endpoint and EWS settings
<a name="bk_CacheSettings"> </a>

Embora seja recomendável que você use a Descoberta Automática regularmente, a forma como a usa regularmente exige alguma consideração. O ideal é equilibrar a resposta rápida às alterações no ambiente em relação à geração de tráfego de rede desnecessário. Quando seu aplicativo obtém uma resposta de Descoberta Automática bem-sucedida pela primeira vez, você deve salvar as informações a seguir para que não seja preciso repetir o processo de Descoberta Automática sempre que enviar uma solicitação do EWS.
  
**Tabela 1. Informações para armazenar em cache as solicitações de Descoberta Automática**

|**Configuração para cache**|**Válido para...**|**Detalhes**|
|:-----|:-----|:-----|
|Ponto de extremidade de Descoberta Automática  <br/> |Contanto que funcione  <br/> |Quando você salva o ponto de extremidade descoberta automática que retornou uma [](how-to-generate-a-list-of-autodiscover-endpoints.md) resposta bem-sucedida, não é preciso repetir o processo de gerar uma lista de pontos de extremidade de Descoberta Automática e tentar até obter uma resposta bem-sucedida.<br/><br/> **OBSERVAÇÃO**: A API Gerenciada do EWS não dá suporte ao armazenamento em cache do ponto de extremidade de Descoberta Automática.           |
|URL do EWS e quaisquer outras configurações recuperadas da resposta descoberta automática  <br/> |Uma semana  <br/> |Ao salvar [a](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) URL do EWS e outras configurações relacionadas, você não precisa enviar uma nova solicitação de Descoberta Automática para cada solicitação do EWS ou se o aplicativo for reiniciado. No entanto, mesmo que uma URL do EWS funcione para o seu usuário, um servidor pode estar disponível que seja mais ideal.<br/><br/> Por exemplo, a caixa de correio do usuário pode ter se movido para um novo servidor de caixa de correio, resultando em um novo ponto de extremidade EWS preferencial. Recomendamos que você atualize suas configurações de usuário enviando uma nova solicitação de Descoberta Automática após uma semana ter passado desde sua última solicitação de Descoberta Automática. Esse tempo pode ser ajustado para atender aos requisitos do seu aplicativo.  <br/> |
   
## <a name="refresh-cached-configuration-information"></a>Atualizar informações de configuração em cache
<a name="bk_RefreshConfig"> </a>

Agora que você tem as informações armazenadas em cache, vamos examinar como você pode manter esse cache atualizado. Recomendamos que você atualize suas informações armazenadas em cache quando:
  
- O período de validade das informações expira.
    
- Ocorre [um erro relacionado a conexão](#bk_ConnectionErrors) E suas informações armazenadas em cache foram atualizadas pela última vez há mais de uma hora.
    
Para atualizar suas informações armazenadas em cache, envie uma solicitação de Descoberta Automática para um ponto de extremidade de Descoberta Automática em cache e faça o seguinte:
  
- Se a solicitação for bem-sucedida, compare o ponto de extremidade EWS na resposta com o ponto de extremidade EWS armazenado em cache e faça o seguinte:
    
  - Se eles são diferentes, use o novo ponto de extremidade EWS. Se você estiver atualize para se recuperar de um erro, repetir a solicitação com falha com o novo ponto de extremidade.
    
  - Se eles são iguais, continue a usar o ponto de extremidade EWS original. Se você estiver atualize para se recuperar de um erro, manipulará o erro conforme apropriado.
    
- Se a solicitação falhar, inicie [o processo de Descoberta Automática](autodiscover-for-exchange.md) desde o início. Depois de obter uma resposta bem-sucedida, substitua o ponto de extremidade de Descoberta Automática em cache pelo ponto de extremidade descoberta automática que foi bem-sucedido e continue a usar o novo ponto de extremidade do EWS. Se você não receber uma resposta bem-sucedida, continue a usar o ponto de extremidade de Descoberta Automática original e o ponto de extremidade EWS. Se você estiver atualize para se recuperar de um erro, manipulará o erro conforme apropriado. 
    
A figura a seguir fornece uma representação visual desse processo.
  
**Figura 1. Processo para atualizar informações de configuração usando a Descoberta Automática**

![Diagrama esquemático mostrando como a Descoberta Automática atualiza informações de configuração.](media/Ex15_Autodiscover_Refresh_Flowchart.png)
  
### <a name="connection-related-errors"></a>Erros relacionados à conexão
<a name="bk_ConnectionErrors"> </a>

Atualizar suas informações de configuração em cache pode ajudar com alguns erros, mas não todos. 
  
**Tabela 2. Erros abordados atualizendo seu cache**

|**Erro**|**Implementação da API Gerenciada do EWS**|**Observações**|
|:-----|:-----|:-----|
|Erros de falha de REDE ou DNS<br/><br/> Exemplo: não foi possível encontrar o nome do host.  <br/> |[ServiceRemoteException](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.serviceremoteexception?view=exchange-ews-api) <br/> |Qualquer erro que indique que o servidor não pôde ser encontrado ou não pôde ser atingido pode ser resolvido ao tentar a Descoberta Automática. <br/><br/> Seu ponto de extremidade EWS armazenado em cache pode não ser mais válido, e a Descoberta Automática pode ser capaz de apontar você para o novo servidor.  <br/> |
|Erros de status HTTP<br/><br/> Exemplo: 503 Serviço Indisponível  <br/> |[ServiceRemoteException](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.serviceremoteexception?view=exchange-ews-api) <br/> |Erros de status HTTP podem acontecer por vários motivos diferentes.<br/><br/> No entanto, é uma boa ideia tentar a Descoberta Automática para ver se um novo ponto de extremidade EWS está disponível para o usuário.  <br/> |
|Códigos de erro do EWS <br/><br/> Exemplo: ErrorConnectionFailed <br/> |[ResponseCodeType](../web-service-reference/responsecode.md) <br/> | A maioria dos códigos de erro do EWS não garante a atualização das informações de configuração.<br/><br/> No entanto, o seguinte indica especificamente que as informações de configuração precisam ser atualizadas:<br/>- **ErrorConnectionFailed** <br/>- **ErrorMailboxMoveInProgress** <br/> |
   
## <a name="see-also"></a>Confira também

- [Descoberta Automática do Exchange](autodiscover-for-exchange.md)  
- [Gerar uma lista de pontos de extremidade de Descoberta Automática](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [Obter as configurações de usuário do Exchange usando a Descoberta Automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    

