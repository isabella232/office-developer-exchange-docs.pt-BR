---
title: Atualizar as informações de configuração usando a Descoberta Automática
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c2f3c6a5-e8ea-4375-b41a-686a6f238d33
description: Saiba como e quando atualizar as informações de configuração para sua conexão do Exchange usando a descoberta automática.
ms.openlocfilehash: b9a4264d150d09b0e143e0bf7365af351bb2ef44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527751"
---
# <a name="refresh-configuration-information-by-using-autodiscover"></a>Atualizar as informações de configuração usando a Descoberta Automática

Saiba como e quando atualizar as informações de configuração para sua conexão do Exchange usando a descoberta automática.
  
Quando o aplicativo EWS é executado pela primeira vez, a descoberta automática oferece uma ótima maneira de coletar as informações necessárias para se conectar à caixa de correio do Exchange do usuário. Mas a descoberta automática não é apenas para uso pela primeira vez. O uso da descoberta automática em uma base regular pode ajudar a manter seu aplicativo conectado, permitindo que ele responda às alterações na implantação do Exchange.
  
## <a name="cache-autodiscover-endpoint-and-ews-settings"></a>Configurações de ponto de extremidade de descoberta automática de cache e EWS
<a name="bk_CacheSettings"> </a>

Embora seja recomendável que você use a descoberta automática regularmente, o quão regularmente você usa isso requer alguma consideração. O ideal é que você Equilibre a resposta rapidamente às alterações no ambiente em relação à geração de tráfego de rede muito desnecessário. Quando o aplicativo recebe uma resposta de descoberta automática bem-sucedida pela primeira vez, você deve salvar as seguintes informações para não precisar repetir o processo de descoberta automática sempre que enviar uma solicitação do EWS.
  
**Tabela 1. Informações para armazenar em cache as solicitações de descoberta automática**

|**Configuração para cache**|**Válido para...**|**Detalhes**|
|:-----|:-----|:-----|
|Ponto de extremidade de descoberta automática  <br/> |Contanto que funcione  <br/> |Quando você salva o ponto de extremidade de descoberta automática que retornou uma resposta bem-sucedida, não é necessário repetir o processo de [geração de uma lista de pontos de extremidade de descoberta automática](how-to-generate-a-list-of-autodiscover-endpoints.md) e experimentá-los até obter uma resposta bem-sucedida.<br/><br/> **Observação**: a API gerenciada do EWS não dá suporte ao armazenamento em cache do ponto de extremidade de descoberta automática.           |
|URL do EWS e quaisquer outras configurações recuperadas da resposta de descoberta automática  <br/> |Uma semana  <br/> |Ao salvar a URL do EWS e outras configurações relacionadas, não é necessário [Enviar uma nova solicitação de descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) para cada solicitação do EWS ou se o aplicativo for reiniciado. No entanto, mesmo que uma URL do EWS funcione para o seu usuário, pode haver um servidor disponível que seja mais adequado.<br/><br/> Por exemplo, a caixa de correio do usuário pode ter sido movida para um novo servidor de caixa de correio, resultando em um novo ponto de extremidade do EWS preferencial. Recomendamos que você atualize suas configurações de usuário enviando uma nova solicitação de descoberta automática depois que uma semana tiver passado desde a última solicitação de descoberta automática. Esse tempo pode ser ajustado para atender aos requisitos do seu aplicativo.  <br/> |
   
## <a name="refresh-cached-configuration-information"></a>Atualizar informações de configuração armazenadas em cache
<a name="bk_RefreshConfig"> </a>

Agora que você tem as informações armazenadas em cache, vamos examinar como você pode manter o cache atualizado. Recomendamos que você atualize suas informações armazenadas em cache quando:
  
- O período de validade das informações expira.
    
- Ocorre um [erro relacionado à conexão](#bk_ConnectionErrors) , e suas informações em cache foram atualizadas pela última vez em uma hora atrás.
    
Para atualizar suas informações armazenadas em cache, envie uma solicitação de descoberta automática para um ponto de extremidade de descoberta automática em cache e faça o seguinte:
  
- Se a solicitação for bem-sucedida, compare o ponto de extremidade do EWS na resposta com o ponto de extremidade do EWS armazenado em cache e faça o seguinte:
    
  - Se forem diferentes, use o ponto de extremidade novo EWS. Se você estiver atualizando para se recuperar de um erro, repita a solicitação com falha com o novo ponto de extremidade.
    
  - Se forem iguais, continue a usar o ponto de extremidade do EWS original. Se você estiver atualizando para se recuperar de um erro, manipule o erro conforme apropriado.
    
- Se a solicitação falhar, inicie o [processo de descoberta automática](autodiscover-for-exchange.md) desde o início. Após obter uma resposta bem-sucedida, substitua o ponto de extremidade de descoberta automática em cache pelo ponto de extremidade de descoberta automática com êxito e continue a usar o novo ponto de extremidade do EWS. Se você não receber uma resposta bem-sucedida, continue a usar o ponto de extremidade de descoberta automática e o ponto de extremidade do EWS originais. Se você estiver atualizando para se recuperar de um erro, manipule o erro conforme apropriado. 
    
A figura a seguir fornece uma representação visual desse processo.
  
**Figura 1. Processo de atualização de informações de configuração usando a descoberta automática**

![Diagrama esquemático mostrando como a Descoberta Automática atualiza informações de configuração.](media/Ex15_Autodiscover_Refresh_Flowchart.png)
  
### <a name="connection-related-errors"></a>Erros relacionados à conexão
<a name="bk_ConnectionErrors"> </a>

A atualização de suas informações de configuração em cache pode ajudar com alguns erros, mas não todos. 
  
**Tabela 2. Erros resolvidos pela atualização do cache**

|**Error**|**Implementação da API gerenciada do EWS**|**Anotações**|
|:-----|:-----|:-----|
|Erros de DNS ou de falha de rede<br/><br/> Exemplo: não foi possível encontrar o nome do host.  <br/> |[Onremoteexception](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.serviceremoteexception?view=exchange-ews-api) <br/> |Qualquer erro que indique que o servidor não pôde ser encontrado ou não pôde ser alcançado pode ser resolvido tentando a descoberta automática. <br/><br/> O ponto de extremidade do EWS em cache pode não ser mais válido e a descoberta automática pode ser capaz de apontar para o novo servidor.  <br/> |
|Erros de status HTTP<br/><br/> Exemplo: serviço 503 indisponível  <br/> |[Onremoteexception](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.serviceremoteexception?view=exchange-ews-api) <br/> |Os erros de status HTTP podem ocorrer por vários motivos diferentes.<br/><br/> No entanto, é uma boa ideia tentar a descoberta automática para ver se um novo ponto de extremidade do EWS está disponível para o usuário.  <br/> |
|Códigos de erro do EWS <br/><br/> Exemplo: ErrorConnectionFailed <br/> |[ResponseCodeType](../web-service-reference/responsecode.md) <br/> | A maioria dos códigos de erro do EWS não garante a atualização de suas informações de configuração.<br/><br/> No entanto, o seguinte indica especificamente que as informações de configuração precisam ser atualizadas:<br/>- **ErrorConnectionFailed** <br/>- **ErrorMailboxMoveInProgress** <br/> |
   
## <a name="see-also"></a>Confira também

- [Descoberta Automática do Exchange](autodiscover-for-exchange.md)  
- [Gerar uma lista de pontos de extremidade de Descoberta Automática](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [Obter as configurações de usuário do Exchange usando a Descoberta Automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    

