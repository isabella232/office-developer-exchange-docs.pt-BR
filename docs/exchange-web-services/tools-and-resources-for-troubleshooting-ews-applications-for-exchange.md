---
title: Ferramentas e recursos para solucionar problemas de aplicativos do EWS do Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ee7fcd05-35d7-47bf-bac4-e719c49c11fe
description: Encontre recursos para ajudá-lo a solucionar problemas de seu aplicativo de EWS ou a API gerenciada de EWS.
ms.openlocfilehash: d8d8ea736ca3b896642ad06f5987caeba8d8d059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750957"
---
# <a name="tools-and-resources-for-troubleshooting-ews-applications-for-exchange"></a>Ferramentas e recursos para solucionar problemas de aplicativos do EWS do Exchange

Encontre recursos para ajudá-lo a solucionar problemas de seu aplicativo de EWS ou a API gerenciada de EWS.
  
Nem sempre tudo conforme o planejado. Em alguns casos, EWS solicita fail ou fornecer resultados inesperados. Isso pode ser frustrante, especialmente se o motivo pelo qual não são óbvio. Espera-se que isso nunca ocorra com você, mas se contiver, este artigo fornece informações sobre ferramentas e recursos que você pode usar para ajudar a solucionar o problema.
  
> [!NOTE]
> Este artigo fornece conselhos de solução de problemas geral e fontes para obter informações de solução de problemas. Infelizmente não é possível dar as etapas detalhadas de solução de problemas. Para obter assistência seu erro específico de solução de problemas, consulte as [próximas etapas](#bk_NextSteps). 
  
## <a name="examine-the-soap-requests-and-responses"></a>Examinar o SOAP solicitações e respostas

Quando as coisas não estão funcionando corretamente, realmente Ajuda poderão ver o que está acontecendo. A primeira linha de consulta ao investigar um problema com EWS ou a API gerenciada de EWS é examinar as solicitações de seu aplicativo está enviando pela rede e as respostas que o servidor está enviando novamente.
  
A API gerenciada de EWS torna fácil com suas [criadas em termos de funcionalidade de rastreamento](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)examinando SOAP solicitações e respostas. Se você estiver usando o EWS, você talvez ou pode não ter acesso à funcionalidade semelhante de rastreamento, dependendo de qual plataforma ou classes que você usa para enviar suas solicitações. No entanto, você sempre pode usar uma ferramenta de rastreamento de rede como [Monitor de rede](http://www.microsoft.com/en-us/download/details.aspx?id=4865) ou o [Fiddler](http://www.telerik.com/fiddler) para examinar o tráfego de rede e visualizar as cargas de solicitação e a resposta. 
  
Além disso, você pode [instrumento suas solicitações de cliente](instrumenting-client-requests-for-ews-and-rest-in-exchange.md) para aprimorar as informações disponíveis em solicitações e respostas. 
  
Depois que as solicitações e respostas, pergunte a mesmo o seguinte: que elas parecem corretas? São os valores que seu aplicativo está enviando esperado? As respostas faz sentido?
  
## <a name="examine-error-codes"></a>Examinar os códigos de erro

Em alguns casos, o código de erro pode passar um longo caminho para identificar o problema, mesmo se a princípio ele não parece faz sentido. O erro indica que seu cliente está sendo [acelerado](ews-throttling-in-exchange.md)? Talvez uma chamada a descoberta automática para [atualizar as informações de configuração](how-to-refresh-configuration-information-by-using-autodiscover.md) está na ordem? 
  
Para obter mais informações sobre o tratamento de erros específicos, consulte os seguintes artigos:
  
- [Manipulação de mensagens de erro de descoberta automática](handling-autodiscover-error-messages.md)
    
- [Tratando erros relacionados a notificação no EWS no Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Tratando erros relacionados a sincronização no EWS no Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Tratando erros relacionados a exclusão no EWS no Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="verify-versions"></a>Verifique se as versões

Há um número de diferentes componentes envolvidos nas operações de EWS e as versões desses componentes podem influenciar os resultados.
  
**Tabela 1. Versionado componentes que podem afetar os processos EWS**

|**Componente**|**API gerenciada do EWS**|**EWS**|**Notes**|
|:-----|:-----|:-----|:-----|
|Versão de servidor solicitado  <br/> |Propriedade [ExchangeServiceBase.RequestedServerVersion](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx)  <br/> |Elemento [RequestServerVersion](http://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx)  <br/> |Esse valor controla qual versão do esquema do EWS é usado para processar a solicitação do EWS. Certifique-se de que a versão do esquema especificada aqui faz sentido para a solicitação que você está enviando. Algumas operações e propriedades não estão disponíveis em versões anteriores do esquema.  <br/> |
|A versão do servidor  <br/> |Propriedade [ExchangeServiceBase.ServerInfo](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservicebase.serverinfo%28v=exchg.80%29.aspx)  <br/> |Elemento [ServerVersionInfo](http://msdn.microsoft.com/library/c04a6872-ca27-432b-aac2-36b023d0afc6%28Office.15%29.aspx)  <br/> |Esse valor será retornado pelo servidor em respostas do EWS e indica a versão do servidor que processaram a resposta. Verifique se que esse valor é o que você espera. Se possível, certifique-se de que o servidor do Exchange está executando a atualização mais recente para a sua versão principal do Exchange.  <br/> |
|A versão de API gerenciada de EWS  <br/> |A propriedade da versão de produto do arquivo Microsoft.Exchange.WebServices.dll.  <br/> |Não aplicável  <br/> |Se você estiver usando a API gerenciada de EWS, certifique-se de que você está usando [a versão mais recente](http://aka.ms/ews-managed-api-readme).  <br/> |
   
## <a name="verify-access"></a>Verificar o acesso

EWS é habilitado por padrão, mas [podem ser alterados padrões](how-to-control-access-to-ews-in-exchange.md). Use o cmdlet [Get-OrganizationConfig](http://technet.microsoft.com/en-us/library/bb124754.aspx) para certificar-se de que o EWS está habilitado no servidor e o cmdlet [Get-CASMailbox](http://technet.microsoft.com/en-us/library/aa997571.aspx) para certificar-se de que o EWS é habilitado para caixa de correio do usuário. Verifique também as duas respostas de cmdlet para um EWS permitem ou bloqueiam lista e certifique-se de que o seu aplicativo não está bloqueado para usando o EWS. 
  
Você também deve verificar se as [configurações de autenticação padrão](http://technet.microsoft.com/en-us/library/gg247612%28v=exchg.150%29.aspx) no diretório virtual EWS não foi modificado. 
  
## <a name="try-another-ews-client"></a>Tente outro cliente do EWS

Em alguns casos, é útil tentar a mesma solicitação de outro cliente e a comparação de resultados. Se outro cliente obtém resultados diferentes, o que é diferente? Para saber qual é a diferença entre uma solicitação bem-sucedida e uma solicitação com falha pode ajudar a explicam por que uma solicitação específica está falhando.
  
Embora certamente você pode escrever outro cliente para testar com, você não precisa! [EWSEditor](http://ewseditor.codeplex.com/) é um cliente de exemplo que usa a API gerenciada de EWS e EWS. Você pode baixar o cliente (incluindo o código-fonte) e usá-lo para testar as solicitações de mesmas que estão falhando em seu aplicativo. 
  
## <a name="examine-iis-logs"></a>Examine os logs do IIS

Se você tiver acesso ao Exchange server, a funcionalidade de log fornecida pelos serviços de informações da Internet (IIS) nos servidores de acesso para cliente pode fornecer mais informações sobre falhas. No entanto, tenha em mente que o IIS registra somente será útil se você está recebendo um erro HTTP.
  
O IIS fornece dois métodos diferentes de log: [log de IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis) e [falhas nas solicitações de rastreamento](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis). Para trabalhar com os logs do IIS, você pode usar o [Log Parser Studio](http://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx), que inclui um número de consultas do EWS internas.
  
## <a name="next-steps"></a>Próximas etapas
<a name="bk_NextSteps"> </a>

Agora que você aprendeu sobre as ferramentas e recursos que você pode usar para solucionar problemas, talvez seja necessário ajuda a entender as informações fornecidas por essas ferramentas. A seguir estão algumas opções para obtenção de Ajuda:
  
- [Fórum de desenvolvimento do Exchange Server no MSDN](http://social.msdn.microsoft.com/Forums/en-US/home?category=exchangeserver) — faça uma pergunta da comunidade de desenvolvimento do MSDN Exchange Server. 
    
- [StackOverflow](http://stackoverflow.com/tags/ews) — faça uma pergunta da comunidade do StackOverflow. Certifique-se de marcar sua postagem com "ews". 
    
- [Suporte da Microsoft](http://support.microsoft.com/ph/730/en-us) — contate um profissional de suporte da Microsoft para obter assistência. 
    
## <a name="see-also"></a>Confira também


Consulte os seguintes artigos:
  
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Solicitações e respostas para solucionar problemas de aplicativos do EWS Managed API de rastreamento](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    
- [Instrumentação solicitações de clientes para o EWS e REST no Exchange](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
- [EWS limitação no Exchange](ews-throttling-in-exchange.md)
    
- [Atualizar informações de configuração usando a descoberta automática](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [Manipulação de mensagens de erro de descoberta automática](handling-autodiscover-error-messages.md)
    
- [Tratando erros relacionados a notificação no EWS no Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Tratando erros relacionados a sincronização no EWS no Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Tratando erros relacionados a exclusão no EWS no Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
- [Configurando o log no IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis)
    
- [Solucionando problemas de falha solicitações usando o rastreamento no IIS 7](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)
    
- [Introdução: O Log Parser Studio](http://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx)
    
- [Configurações padrão para os diretórios virtuais do Exchange](http://technet.microsoft.com/en-us/library/gg247612%28v=exchg.150%29.aspx)
    
Baixe o seguinte:
  
- [Microsoft Network Monitor 3.4](http://www.microsoft.com/en-us/download/details.aspx?id=4865)
    
- [Fiddler](http://www.telerik.com/fiddler)
    
- [EWSEditor](http://ewseditor.codeplex.com/)
    
- [API gerenciada de serviços Web do Exchange](http://go.microsoft.com/fwlink/?LinkID=255472)
    

