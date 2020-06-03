---
title: Ferramentas e recursos para a solução de problemas de aplicativos do EWS para Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: ee7fcd05-35d7-47bf-bac4-e719c49c11fe
description: Encontre recursos para ajudá-lo a solucionar problemas de sua API gerenciada EWS ou aplicativo EWS.
localization_priority: Priority
ms.openlocfilehash: 7c7cbe8c93edec5ad99df079c6eb96286c1ba063
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463738"
---
# <a name="tools-and-resources-for-troubleshooting-ews-applications-for-exchange"></a>Ferramentas e recursos para a solução de problemas de aplicativos do EWS para Exchange

Encontre recursos para ajudá-lo a solucionar problemas de sua API gerenciada EWS ou aplicativo EWS.
  
As coisas nem sempre vão tão planejadas. Às vezes, as solicitações de EWS falham ou fornecem resultados inesperados. Isso pode ser frustrante, especialmente se a razão não é óbvia. Espero que isso nunca aconteça, mas se o fizer, este artigo fornecerá informações sobre ferramentas e recursos que você pode usar para ajudar a solucionar o problema.
  
> [!NOTE]
> Este artigo fornece orientações e fontes de solução de problemas gerais para a solução de problemas de informações. Infelizmente, não é possível fornecer etapas detalhadas de solução de problemas. Para obter ajuda para solucionar problemas de erro específico, consulte [próximas etapas](#bk_NextSteps). 
  
## <a name="examine-the-soap-requests-and-responses"></a>Examinar as solicitações e respostas SOAP

Quando as coisas não estão funcionando corretamente, ela realmente ajuda a ver o que está acontecendo. A primeira linha da consulta ao investigar um problema com o EWS ou a API gerenciada do EWS é examinar as solicitações que seu aplicativo está enviando pela rede e as respostas que o servidor está enviando de volta.
  
A API gerenciada do EWS torna fácil a análise de solicitações e respostas SOAP com sua [funcionalidade de rastreamento interna](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md). Se você estiver usando o EWS, talvez ou não tenha acesso a funcionalidades de rastreamento semelhantes, dependendo de qual plataforma ou classes você usa para enviar suas solicitações. No entanto, você sempre pode usar uma ferramenta de rastreamento de rede como o [Monitor de rede](https://www.microsoft.com/download/details.aspx?id=4865) ou o [Fiddler](http://www.telerik.com/fiddler) para examinar o tráfego de rede e exibir as cargas de solicitação e resposta. 
  
Além disso, você pode [instrumentar suas solicitações de cliente](instrumenting-client-requests-for-ews-and-rest-in-exchange.md) para aprimorar as informações disponíveis em solicitações e respostas. 
  
Após ter as solicitações e respostas, pergunte-se o seguinte: eles estão corretos? Os valores que seu aplicativo está enviando devem ser esperados? As respostas fazem sentido?
  
## <a name="examine-error-codes"></a>Examinar códigos de erro

Às vezes, o código de erro pode ser muito longo para indicar o problema, mesmo se a primeira vista não parecer fazer sentido. O erro indica que o cliente está sendo [limitado](ews-throttling-in-exchange.md)? Talvez uma chamada para a descoberta automática para [atualizar as informações de configuração](how-to-refresh-configuration-information-by-using-autodiscover.md) está em ordem? 
  
Para obter mais informações sobre como lidar com erros específicos, consulte os seguintes artigos:
  
- [Manipulação de mensagens de erro de Descoberta Automática](handling-autodiscover-error-messages.md)
    
- [Tratamento de erros relacionados à notificação no EWS no Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Como lidar com erros relacionados à sincronização no EWS no Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Tratamento de erros relacionados à exclusão no EWS no Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="verify-versions"></a>Verificar versões

Há vários componentes diferentes envolvidos nas operações do EWS, e as versões desses componentes podem influenciar os resultados.
  
**Tabela 1. Componentes com controle de versão que podem afetar processos EWS**

|**Componente**|**API gerenciada do EWS**|**EWS**|**Anotações**|
|:-----|:-----|:-----|:-----|
|Versão de servidor solicitada  <br/> |Propriedade [ExchangeServiceBase. RequestedServerVersion](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx)  <br/> |Elemento [RequestServerVersion](https://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx)  <br/> |Esse valor controla qual versão do esquema EWS é usada para processar a solicitação EWS. Verifique se a versão do esquema especificada aqui faz sentido para a solicitação que você está enviando. Algumas propriedades e operações não estão disponíveis em versões anteriores do esquema.  <br/> |
|A versão do servidor  <br/> |Propriedade [ExchangeServiceBase. ServerInfo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.serverinfo%28v=exchg.80%29.aspx)  <br/> |Elemento [ServerVersionInfo](https://msdn.microsoft.com/library/c04a6872-ca27-432b-aac2-36b023d0afc6%28Office.15%29.aspx)  <br/> |Esse valor é retornado pelo servidor nas respostas do EWS e indica a versão do servidor que processou a resposta. Certifique-se de que esse valor é o que você espera. Se possível, verifique se o servidor do Exchange está executando a atualização mais recente para sua versão principal do Exchange.  <br/> |
|A versão da API gerenciada do EWS  <br/> |A propriedade da versão do produto do arquivo Microsoft. Exchange. WebServices. dll.  <br/> |Não aplicável  <br/> |Se você estiver usando a API gerenciada do EWS, verifique se está usando [a versão mais recente](https://aka.ms/ews-managed-api-readme).  <br/> |
   
## <a name="verify-access"></a>Verificar o acesso

O EWS está habilitado por padrão, mas [os padrões podem ser alterados](how-to-control-access-to-ews-in-exchange.md). Use o cmdlet [Get-OrganizationConfig](https://technet.microsoft.com/library/bb124754.aspx) para certificar-se de que o EWS está habilitado no servidor e o cmdlet [Get-CASMailbox](https://technet.microsoft.com/library/aa997571.aspx) para garantir que o EWS esteja habilitado para a caixa de correio do usuário. Além disso, verifique as respostas de cmdlet de uma lista de permissões ou bloqueios do EWS e certifique-se de que o aplicativo não está bloqueado de usar o EWS. 
  
Você também deve verificar se as [configurações de autenticação padrão](https://technet.microsoft.com/library/gg247612%28v=exchg.150%29.aspx) no diretório virtual do EWS não foram modificadas. 
  
## <a name="try-another-ews-client"></a>Tente outro cliente do EWS

Às vezes, é útil tentar a mesma solicitação de outro cliente e comparar os resultados. Se outro cliente obtiver resultados diferentes, o que é diferente? Descobrir o que é diferente entre uma solicitação bem-sucedida e uma solicitação com falha pode ajudar a explicar por que uma solicitação específica está falhando.
  
Embora você possa, certamente, escrever outro cliente para testar, não é necessário! [EWSEditor](http://ewseditor.codeplex.com/) é um cliente de exemplo que usa a API gerenciada do EWS e o EWS. Você pode baixar o cliente (incluindo o código-fonte) e usá-lo para testar as mesmas solicitações que estão falhando em seu aplicativo. 
  
## <a name="examine-iis-logs"></a>Examinar os logs do IIS

Se você tiver acesso ao servidor Exchange, a funcionalidade de registro em log fornecida pelos serviços de informações da Internet (IIS) nos servidores de acesso para cliente poderá fornecer mais informações sobre falhas. No entanto, tenha em mente que os logs do IIS só serão úteis se você estiver recebendo um erro de HTTP.
  
O IIS fornece dois métodos de log diferentes: rastreamento de [log do IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis) e de [solicitações com falha](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis). Para trabalhar com os logs do IIS, você pode usar o [Log Parser Studio](https://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx), que inclui várias consultas do EWS internas.
  
## <a name="next-steps"></a>Próximas etapas
<a name="bk_NextSteps"> </a>

Agora que você aprendeu sobre as ferramentas e os recursos que você pode usar para solucionar problemas, talvez precise de ajuda para entender as informações fornecidas por essas ferramentas. Veja a seguir algumas opções para obter ajuda:
  
- [Fórum de desenvolvimento do Exchange Server no MSDN](https://social.msdn.microsoft.com/Forums/home?category=exchangeserver) — faça uma pergunta da comunidade de desenvolvimento do Exchange Server do MSDN. 
    
- [StackOverflow](http://stackoverflow.com/tags/ews) — faça uma pergunta sobre a Comunidade do stackoverflow. Certifique-se de marcar sua postagem com "EWS". 
    
- [Suporte da Microsoft](https://support.microsoft.com/ph/730/en-us) — entre em contato com um profissional de suporte da Microsoft para obter assistência. 
    
## <a name="see-also"></a>Confira também


Confira os seguintes artigos:
  
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Rastrear solicitações e respostas para solucionar problemas de aplicativos de API gerenciada do EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    
- [Instrumentação de solicitações de cliente para EWS e REST no Exchange](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
- [Limitação do EWS no Exchange](ews-throttling-in-exchange.md)
    
- [Atualizar as informações de configuração usando a Descoberta Automática](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [Manipulação de mensagens de erro de Descoberta Automática](handling-autodiscover-error-messages.md)
    
- [Tratamento de erros relacionados à notificação no EWS no Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Como lidar com erros relacionados à sincronização no EWS no Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Tratamento de erros relacionados à exclusão no EWS no Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
- [Configurando o registro em log no IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis)
    
- [Solucionando problemas de solicitações com falha usando o rastreamento no IIS 7](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)
    
- [Introdução: Log Parser Studio](https://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx)
    
- [Configurações padrão para diretórios virtuais do Exchange](https://technet.microsoft.com/library/gg247612%28v=exchg.150%29.aspx)
    
Baixe o seguinte:
  
- [Microsoft Network Monitor 3.4](https://www.microsoft.com/download/details.aspx?id=4865)
    
- [Fiddler](http://www.telerik.com/fiddler)
    
- [EWSEditor](http://ewseditor.codeplex.com/)
    
- [API gerenciada dos Serviços Web do Exchange](https://go.microsoft.com/fwlink/?LinkID=255472)
    

