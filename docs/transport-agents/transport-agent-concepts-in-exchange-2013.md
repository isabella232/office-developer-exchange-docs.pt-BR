---
title: Conceitos de agente de transporte no Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0c700af8-2792-4d3f-8571-8860e0550d8e
description: Encontre informações sobre como o pipeline do agente de transporte e a arquitetura de função de servidor no Exchange 2013 afetam o desenvolvimento de agentes de transporte e as classes que você pode usar para desenvolver agentes de transporte.
ms.openlocfilehash: 9116c9b7811958a2479421a642052df3cee24e34
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537158"
---
# <a name="transport-agent-concepts-in-exchange-2013"></a>Conceitos de agente de transporte no Exchange 2013

Encontre informações sobre como o pipeline do agente de transporte e a arquitetura de função de servidor no Exchange 2013 afetam o desenvolvimento de agentes de transporte e as classes que você pode usar para desenvolver agentes de transporte. 
  
**Aplica-se a:** Exchange Server 2013 
  
Você pode usar a biblioteca de classes fornecida no Exchange Server 2013 para implementar agentes de transporte que se registram para eventos e realizar ações em mensagens à medida que passam pelo pipeline de transporte. Você também pode usar agentes de transporte para modificar mensagens e converter conteúdo. 
  
Este artigo fornece informações sobre agentes de transporte e a arquitetura do pipeline de transporte. É importante entender a arquitetura do pipeline de transporte para que você possa modificar o comportamento de transporte para atender às necessidades da sua organização. Este artigo também fornece informações sobre alterações na arquitetura Exchange 2013 que afetam os agentes de transporte e as classes que você pode usar para desenvolver agentes de transporte. 
  
## <a name="transport-agents-in-the-transport-pipeline"></a>Agentes de transporte no pipeline de transporte
<a name="Pipeline"> </a>

Os agentes de transporte são derivados de uma das três classes a seguir:
  
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
- [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx)
    
O pipeline de transporte refere-se ao fluxo de dados de mensagem dentro dos limites de uma organização Exchange 2013. O pipeline consiste nos serviços listados na tabela a seguir.
  
**Tabela 1. Serviços de pipeline de transporte**

|**Serviço**|**Descrição**|**Classes com suporte**|
|:-----|:-----|:-----|
|Transporte front-end  <br/> |É executado em todos os servidores de [Acesso](https://technet.microsoft.com/library/dd298114%28v=exchg.150%29.aspx) para Cliente e atua como um proxy sem estado para todo o tráfego SMTP externo de entrada e saída para a organização Exchange 2013. O serviço de Transporte de Front-End não inspeciona o conteúdo da mensagem ou enfilfila mensagens localmente. Ele se comunica com o serviço de Transporte em um servidor [de Caixa de Correio.](https://technet.microsoft.com/library/jj150491%28v=exchg.150%29.aspx)  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|Transport  <br/> |É executado em todos os servidores de Caixa de Correio e é semelhante à função de servidor [de Transporte](https://technet.microsoft.com/library/bb123494%28v=exchg.141%29.aspx) de Hub no Exchange Server 2010. O serviço de Transporte encaminha mensagens entre si e os serviços de Transporte de Caixa de Correio e Transporte de Front-End. Esse serviço não se comunica diretamente com bancos de dados de caixa de correio.  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) <br/> |
|Transporte de Caixa de Correio  <br/> |É executado em todos os servidores de Caixa de Correio e consiste em dois serviços separados: Envio de Transporte de Caixa de Correio e Entrega de Transporte de Caixa de Correio. A Entrega de Transporte de Caixa de Correio recebe mensagens SMTP do serviço de Transporte e se conecta ao banco de dados de caixa de correio usando Exchange chamada de procedimento remoto (RPC) para entregar a mensagem. O Envio de Transporte de Caixa de Correio se conecta ao banco de dados de caixa de correio usando o RPC para recuperar mensagens e envia as mensagens via SMTP para o serviço de Transporte.  <br/> |Nenhum.  <br/> |
   
### <a name="transport-events"></a>Eventos de transporte
<a name="Events"> </a>

Implemente os agentes de transporte primeiro registrando-se para um evento e, em seguida, fazendo uma ação quando esse evento é a ser a incêndio. Cada um dos três tipos de agente pode se registrar para um conjunto diferente de eventos.
  
A figura a seguir mostra onde os agentes de transporte do pipeline de transporte podem se registrar para eventos.
  
**Figura 1. Eventos de transporte**

![An image shows message flow through the transport pipeline and events for which each agent can register beginning with Smtp events for the SmtpReceivedAgent, then Categorizor events for the RoutingAgent, and finally deliver events for the DeliveryAgent.](media/TAConceptsFig1.png)
  
Quando uma mensagem entra no pipeline de transporte, um agente de transporte derivado da [classe SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) pode agir na mensagem durante qualquer um dos eventos SMTP que o agente registrou. Um agente derivado da classe [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) pode agir em qualquer um dos quatro eventos categorizados para os qual ele se registrou. Um agente derivado da [classe DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) pode agir em uma mensagem durante qualquer um dos eventos de entrega que ele registrou. 
  
## <a name="transport-agents-and-server-roles"></a>Agentes de transporte e funções de servidor
<a name="ServerRoles"> </a>

As alterações na arquitetura de função de servidor no Exchange 2013 afetam os agentes de transporte e o que seus agentes de transporte podem fazer. Exchange 2013 inclui as seguintes funções de servidor:
  
- Servidor de Caixa de Correio — inclui protocolos de Acesso para Cliente, o serviço de Transporte, bancos de dados de caixa de correio e componentes de Unificação de Mensagens. O servidor de Caixa de Correio se comunica diretamente com os Serviços de Domínio do Active Directory (AD DS), servidores de Acesso para Cliente e clientes de email, como Outlook.
    
- Servidor de Acesso para Cliente — fornece autenticação, redirecionamento limitado, serviços proxy e protocolos de acesso para cliente, como HTTP, POP, IMAP e SMTP.
    
- Servidor de Transporte de Borda — encaminha emails para dentro e para fora de uma organização. Os servidores de Transporte de Borda geralmente sentam no perímetro de uma topologia Exchange de borda.
    
Essa estrutura consolidada reduz o número de servidores que precisam ser implantados em um ambiente Exchange 2013. Os administradores não precisam mais implantar servidores de Transporte de Hub e Acesso para Cliente em todos os sites do Active Directory que incluam um servidor de Caixa de Correio e não precisam mais atualizar todas as funções de servidor para aproveitar a nova funcionalidade.
  
Essas alterações na arquitetura de função de servidor podem afetar potencialmente onde no pipeline seu agente pode responder a eventos. Se você criou agentes de transporte para versões do Exchange anteriores ao Exchange 2013, revise as alterações de arquitetura para determinar se você precisa fazer alterações em seus agentes.
  
A figura a seguir mostra como as alterações de arquitetura no Exchange 2013 resultam em um pipeline de transporte simplificado e consolidado. Nesta figura, os servidores de Acesso para Cliente são rotulados de CAS. E os servidores de Caixa de Correio são rotulados como MBX.
  
**Figura 2. Exchange de função de servidor 2013**

![An image shows client traffic through an external firewall and Edge Transport on the left that passes traffic through a layer 4 load balance to a consolidated CAS array and set of mailbox servers in a database accessibility group on the right.](media/Transport_Agent_Concepts_Fig_3.png)
  
A figura a seguir mostra as interações entre as funções de servidor Exchange 2013.
  
**Figura 3. Interações de servidor de Caixa de Correio e Acesso para Cliente**

![An image shows interactions starting with arrows from client traffic passing through a layer 4 load balance that has 4 targets in the CAS: IIS/HTTP Proxy, POP/IMAP, SMTP, and UM. The arrows pass to their complimentary targets in the mailbox store.](media/Transport_Agent_Concepts_Fig_4.png)
  
Para obter mais informações sobre as alterações na arquitetura de função de servidor Exchange 2013, consulte [Exchange arquitetura 2013](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx#BKMK_Arch) em [What's New in Exchange 2013](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx). 
  
## <a name="transport-agent-classes"></a>Classes de agente de transporte
<a name="Create"> </a>

A classe que seu agente de transporte deriva determina os eventos para os quais seu agente pode se registrar. Seu agente normalmente conterá uma classe de agente, uma fábrica de agentes, um ou mais manipuladores de eventos e o código que executa as ações que você deseja que seu agente execute.
  
A tabela a seguir lista as classes das quais derivar para cada tipo de agente.
  
**Tabela 2. Classes de agente**

||||
|:-----|:-----|:-----|
|Tipo de agente  <br/> |Classe base de fábrica  <br/> |Classe base do agente  <br/> |
|Recebimento SMTP  <br/> |[SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|Roteamento  <br/> |[RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) <br/> |[RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> |
|Entrega  <br/> |[DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) <br/> |[DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) <br/> |
   
Essas classes base de fábrica e agente fornecem propriedades e métodos que você pode usar para acessar eventos e mensagens de transporte. Implemente classes em seu agente que herdam dessas classes. Na classe derivada da fábrica do agente, substitua o **método CreateAgent** para que ele retorne uma nova instância da classe do agente. 
  
Argumentos passados para os eventos podem conter uma instância da [classe EmailMessage,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.EmailMessage.aspx) que você pode usar para alterar as propriedades e o conteúdo da mensagem subjacente. Nem todas as informações da mensagem estão disponíveis em cada evento. Você deve determinar qual agente e qual evento é o melhor para a tarefa que deseja realizar. 
  
Os namespaces a seguir contêm tipos que você pode usar para ler, gravar e modificar mensagens no pipeline de transporte:
  
- [Microsoft. Exchange. Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx)
    
- [Microsoft. Exchange. Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx)
    
- [Microsoft. Exchange. Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx)
    
- [Microsoft. Exchange. Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx)
    
- [Microsoft. Exchange. Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx)
    
Depois de gravar seu agente de transporte, instale [e gerencie seu](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx) agente usando o Shell de Gerenciamento Exchange gerenciamento. Para obter mais informações, consulte Criando agentes de transporte [para Exchange 2013](creating-transport-agents-for-exchange-2013.md). 
  
## <a name="see-also"></a>Confira também

- [Agentes de transporte no Exchange](transport-agents-in-exchange-2013.md)    
- [Referência do agente de transporte Exchange 2013](transport-agent-reference-for-exchange-2013.md)   
- [Leitura e modificação de mensagens no pipeline de transporte Exchange 2013](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)    
- [Novidades no Exchange 2013](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx)   
- [Exchange 2013 Server Role Architecture](https://blogs.technet.com/b/exchange/archive/2013/01/23/exchange-2013-server-role-architecture.aspx)    
- [Servidores de Caixa de Correio e Acesso para Cliente](https://technet.microsoft.com/library/jj150519%28v=exchg.150%29.aspx)   
- [Exchange Server 2013 Mail Flow](https://technet.microsoft.com/library/aa996349.aspx)
- [Exchange Server roteamento de email 2013](https://technet.microsoft.com/library/aa998825%28v=exchg.150%29.aspx)   
- [Exchange Server PowerShell (Exchange Shell de Gerenciamento)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
    

