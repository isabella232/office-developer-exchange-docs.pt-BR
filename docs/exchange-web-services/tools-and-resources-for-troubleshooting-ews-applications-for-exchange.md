---
title: Ferramentas e recursos para solucionar problemas de aplicativos EWS para Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: ee7fcd05-35d7-47bf-bac4-e719c49c11fe
description: Encontre recursos para ajudá-lo a solucionar problemas da API Gerenciada do EWS ou do aplicativo EWS.
localization_priority: Priority
ms.openlocfilehash: 8a65b06cf911cd033d7fe5fe1b4566a7496de784
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542579"
---
# <a name="tools-and-resources-for-troubleshooting-ews-applications-for-exchange"></a>Ferramentas e recursos para solucionar problemas de aplicativos EWS para Exchange

Encontre recursos para ajudá-lo a solucionar problemas da API Gerenciada do EWS ou do aplicativo EWS.
  
As coisas nem sempre são conforme o planejado. Às vezes, as solicitações EWS falham ou fornecem resultados inesperados. Isso pode ser frustrante, especialmente se o motivo não for óbvio. Esperamos que isso nunca aconteça com você, mas se isso acontecer, este artigo fornecerá informações sobre ferramentas e recursos que você pode usar para ajudar a solucionar o problema.
  
> [!NOTE]
> Este artigo fornece orientações gerais sobre solução de problemas e fontes para informações de solução de problemas. Infelizmente, não é possível fornecer etapas detalhadas de solução de problemas. Para obter assistência para solucionar o erro específico, consulte [Próximas etapas](#bk_NextSteps). 
  
## <a name="examine-the-soap-requests-and-responses"></a>Examinar as solicitações e respostas SOAP

Quando as coisas não estão funcionando corretamente, é realmente útil poder ver o que está acontecendo. A primeira linha de consulta ao investigar um problema com o EWS ou a API Gerenciada do EWS é examinar as solicitações que seu aplicativo está enviando pela rede e as respostas que o servidor está enviando de volta.
  
A API Gerenciada do EWS facilita o exame de solicitações e respostas SOAP com sua [funcionalidade de rastreamento](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md). Se você estiver usando o EWS, poderá ou não ter acesso à funcionalidade de rastreamento semelhante, dependendo da plataforma ou das classes usadas para enviar suas solicitações. No entanto, você sempre pode usar uma ferramenta de rastreamento de rede como [Monitor de Rede](https://www.microsoft.com/download/details.aspx?id=4865) ou [Fiddler](http://www.telerik.com/fiddler) para examinar o tráfego de rede e exibir os conteúdos de solicitação e resposta. 
  
Além disso, você pode [instrumentar as solicitações de seu cliente](instrumenting-client-requests-for-ews-and-rest-in-exchange.md) para aprimorar as informações disponíveis em solicitações e respostas. 
  
Depois que você tiver as solicitações e respostas, pergunte a si mesmo o seguinte: Elas parecem corretas? Os valores que seu aplicativo está enviando são esperados? As respostas fazem sentido?
  
## <a name="examine-error-codes"></a>Examinar códigos de erro

Às vezes, o código de erro pode facilitar muito na identificação do problema, mesmo que à primeira vista não pareça fazer sentido. O erro indica que o cliente está sendo [limitado](ews-throttling-in-exchange.md)? Talvez uma chamada à Descoberta Automática para [atualizar informações de configuração](how-to-refresh-configuration-information-by-using-autodiscover.md) é necessária? 
  
Para obter mais informações sobre como lidar com erros específicos, consulte os seguintes artigos:
  
- [Manipulação de mensagens de erro de Descoberta Automática](handling-autodiscover-error-messages.md)
    
- [Manipulação de erros relacionados a notificações no EWS no Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Manipulação de erros relacionados à sincronização no EWS no Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Manipulação de erros relacionados à exclusão no EWS no Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="verify-versions"></a>Verificar versões

Há vários componentes diferentes envolvidos em operações do EWS, e as versões desses componentes podem influenciar os resultados.
  
**Tabela 1. Componentes com controle de versão que podem afetar os processos do EWS**

|**Componente**|**API Gerenciada do EWS**|**EWS**|**Anotações**|
|:-----|:-----|:-----|:-----|
|Versão do servidor solicitada  <br/> |propriedade [ExchangeServiceBase.RequestedServerVersion](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx)  <br/> |elemento [RequestServerVersion](https://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx)  <br/> |Esse valor controla qual versão do esquema EWS é usada para processar a solicitação do EWS. Verifique se a versão do esquema especificada aqui faz sentido para a solicitação que você está enviando. Algumas propriedades e operações não estão disponíveis em versões anteriores do esquema.  <br/> |
|A versão do servidor  <br/> |propriedade [ExchangeServiceBase.ServerInfo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.serverinfo%28v=exchg.80%29.aspx)  <br/> |elemento [ServerVersionInfo](https://msdn.microsoft.com/library/c04a6872-ca27-432b-aac2-36b023d0afc6%28Office.15%29.aspx)  <br/> |Esse valor é retornado pelo servidor em respostas EWS e indica a versão do servidor que processou a resposta. Verifique se esse valor é o que você espera. Se possível, verifique se o servidor Exchange está executando a atualização mais recente para sua versão principal do Exchange.  <br/> |
|A versão da API Gerenciada do EWS  <br/> |A propriedade Product version do arquivo Microsoft.Exchange.WebServices.dll.  <br/> |Não aplicável  <br/> |Se você estiver usando a API Gerenciada do EWS, verifique se está usando [a versão mais recente](https://aka.ms/ews-managed-api-readme).  <br/> |
   
## <a name="verify-access"></a>Verificar o acesso

O EWS está habilitado por padrão, mas [padrões podem ser alterados](how-to-control-access-to-ews-in-exchange.md). Use o cmdlet [Get-OrganizationConfig](https://technet.microsoft.com/library/bb124754.aspx) para garantir que o EWS esteja habilitado no servidor, e o cmdlet [Get-CASMailbox](https://technet.microsoft.com/library/aa997571.aspx) para garantir que o EWS esteja habilitado para a caixa de correio do usuário. Verifique também as duas respostas de cmdlet para uma lista de permissões ou bloqueios do EWS e verifique se o aplicativo não está impedido de usar o EWS. 
  
Você também deve verificar se as [configurações de autenticação padrão](https://technet.microsoft.com/library/gg247612%28v=exchg.150%29.aspx) no diretório virtual do EWS não foram modificadas. 
  
## <a name="try-another-ews-client"></a>Tentar outro cliente EWS

Às vezes, é útil tentar a mesma solicitação de outro cliente e comparar os resultados. Se outro cliente obtiver resultados diferentes, o que será diferente? Descobrir o que é diferente entre uma solicitação bem-sucedida e uma solicitação com falha pode ajudar a explicar por que uma solicitação específica está falhando.
  
Embora você possa certamente escrever outro cliente com o qual testar, você não precisa fazer isso! [EWSEditor](http://ewseditor.codeplex.com/) é um cliente de exemplo que usa a API Gerenciada do EWS e o EWS. Você pode baixar o cliente (incluindo o código-fonte) e usá-lo para tentar as mesmas solicitações que estão falhando em seu aplicativo. 
  
## <a name="examine-iis-logs"></a>Examinar logs do IIS

Se você tiver acesso ao servidor Exchange, a funcionalidade de log fornecida pelo Serviços de Informações da Internet (IIS) nos servidores de Acesso para Cliente poderá fornecer mais informações sobre falhas. No entanto, tenha em mente que os logs do IIS só serão úteis se você estiver recebendo um erro HTTP.
  
O IIS fornece dois métodos de registro em log diferentes: [registro em log do IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis) e [rastreamento de solicitações com falha](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis). Para trabalhar com logs do IIS, você pode usar o [Log Parser Studio](https://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx), que inclui várias consultas EWS internas.
  
## <a name="next-steps"></a>Próximas etapas
<a name="bk_NextSteps"> </a>

Agora que você aprendeu sobre as ferramentas e os recursos que pode usar para solucionar problemas, talvez precise de ajuda para entender as informações fornecidas por essas ferramentas. A seguir estão algumas opções para obter ajuda:
  
- [Fórum de desenvolvimento do Exchange Server no MSDN](https://social.msdn.microsoft.com/Forums/home?category=exchangeserver) — Faça uma pergunta para a comunidade de desenvolvimento do MSDN Exchange Server. 
    
- [StackOverflow](http://stackoverflow.com/tags/ews)— faça uma pergunta para a comunidade stackOverflow. Certifique-se de marcar sua postagem com "ews". 
    
- [Suporte da Microsoft](https://support.microsoft.com/ph/730/en-us) — Entre em contato com um profissional de suporte da Microsoft para obter assistência. 
    
## <a name="see-also"></a>Confira também


Confira os seguintes artigos:
  
- [Desenvolver clientes de serviço Web para o Exchange](develop-web-service-clients-for-exchange.md)
    
- [Procure solicitações e respostas para solucionar problemas de aplicativos de API gerenciada do EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    
- [Instrumentando solicitações de cliente para EWS e REST no Exchange](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
- [Limitação do EWS no Exchange](ews-throttling-in-exchange.md)
    
- [Atualizar as informações de configuração usando a Descoberta Automática](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [Manipulação de mensagens de erro de Descoberta Automática](handling-autodiscover-error-messages.md)
    
- [Manipulação de erros relacionados a notificações no EWS no Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Manipulação de erros relacionados à sincronização no EWS no Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Manipulação de erros relacionados à exclusão no EWS no Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
- [Configurando o registro em log no IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis)
    
- [Solução de problemas de solicitações com falha usando o rastreamento no IIS 7](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)
    
- [Introdução: Log Parser Studio](https://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx)
    
- [Configurações Padrão para Diretórios Virtuais do Exchange](https://technet.microsoft.com/library/gg247612%28v=exchg.150%29.aspx)
    
Baixe o seguinte:
  
- [Monitor de Rede da Microsoft 3.4](https://www.microsoft.com/download/details.aspx?id=4865)
    
- [Fiddler](http://www.telerik.com/fiddler)
    
- [EWSEditor](http://ewseditor.codeplex.com/)
    
- [API Gerenciada dos Serviços Web do Exchange](https://www.nuget.org/packages/Microsoft.Exchange.WebServices/)
