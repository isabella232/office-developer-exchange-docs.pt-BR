---
title: Conceitos de agente de transporte no Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0c700af8-2792-4d3f-8571-8860e0550d8e
description: Encontre informações sobre como o pipeline do agente de transporte e a arquitetura de função de servidor no Exchange 2013 afetam o desenvolvimento do agente de transporte e as classes que você pode usar para desenvolver agentes de transporte.
ms.openlocfilehash: b9552ea4398ac8135a11b48eb7e7bdf5ec81985e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527555"
---
# <a name="transport-agent-concepts-in-exchange-2013"></a>Conceitos de agente de transporte no Exchange 2013

Encontre informações sobre como o pipeline do agente de transporte e a arquitetura de função de servidor no Exchange 2013 afetam o desenvolvimento do agente de transporte e as classes que você pode usar para desenvolver agentes de transporte. 
  
**Aplica-se a:** Exchange Server 2013 
  
Você pode usar a biblioteca de classes fornecida no Exchange Server 2013 para implementar agentes de transporte que se registram em eventos e realizar ações em mensagens à medida que elas passam pelo pipeline de transporte. Você também pode usar agentes de transporte para modificar mensagens e converter conteúdo. 
  
Este artigo fornece informações sobre agentes de transporte e a arquitetura de pipeline de transporte. É importante entender a arquitetura do pipeline de transporte para que você possa modificar o comportamento de transporte para atender às necessidades da sua organização. Este artigo também fornece informações sobre alterações na arquitetura do Exchange 2013 que afetam agentes de transporte e as classes que você pode usar para desenvolver agentes de transporte. 
  
## <a name="transport-agents-in-the-transport-pipeline"></a>Agentes de transporte no pipeline de transporte
<a name="Pipeline"> </a>

Os agentes de transporte são derivados de uma das seguintes três classes:
  
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
- [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx)
    
O pipeline de transporte se refere ao fluxo de dados da mensagem dentro dos limites de uma organização do Exchange 2013. O pipeline consiste nos serviços listados na tabela a seguir.
  
**Tabela 1. Serviços de pipeline de transporte**

|**Serviço**|**Descrição**|**Classes suportadas**|
|:-----|:-----|:-----|
|Transporte de front-end  <br/> |É executado em todos os [servidores de acesso para cliente](https://technet.microsoft.com/library/dd298114%28v=exchg.150%29.aspx) e atua como um proxy sem estado para todo o tráfego SMTP externo de entrada e saída para a organização do Exchange 2013. O serviço de transporte de front-end não inspeciona o conteúdo da mensagem ou enfileira qualquer mensagem localmente. Ele se comunica com o serviço de transporte em um [servidor de caixa de correio](https://technet.microsoft.com/library/jj150491%28v=exchg.150%29.aspx).  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|Transport  <br/> |É executado em todos os servidores de caixa de correio e é semelhante à função de [servidor Transporte de Hub](https://technet.microsoft.com/library/bb123494%28v=exchg.141%29.aspx) no Exchange Server 2010. O serviço de transporte roteia mensagens entre si e o transporte de caixa de correio e os serviços de transporte de front-end. Este serviço não se comunica diretamente com bancos de dados de caixa de correio.  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) <br/> |
|Transporte de caixa de correio  <br/> |Executa em todos os servidores de caixa de correio e consiste em dois serviços separados: envio de transporte de caixa de correio e entrega de transporte de caixa de correio A entrega de transporte de caixa de correio recebe mensagens SMTP do serviço de transporte e se conecta ao banco de dados de caixa de correio usando uma RPC (chamada de procedimento remoto) do Exchange para entregar a mensagem. O envio de transporte de caixa de correio conecta-se ao banco de dados de caixa de correio usando RPC para recuperar mensagens e envia as mensagens por SMTP para o serviço de transporte.  <br/> |Nenhum  <br/> |
   
### <a name="transport-events"></a>Eventos de transporte
<a name="Events"> </a>

Você implementa agentes de transporte, registrando primeiro um evento e, em seguida, realizando uma ação quando esse evento é acionado. Cada um dos três tipos de agentes pode se registrar em um conjunto diferente de eventos.
  
A figura a seguir mostra onde os agentes de transporte de pipeline de transporte podem se registrar em eventos.
  
**Figura 1. Eventos de transporte**

![An image shows message flow through the transport pipeline and events for which each agent can register beginning with Smtp events for the SmtpReceivedAgent, then Categorizor events for the RoutingAgent, and finally deliver events for the DeliveryAgent.](media/TAConceptsFig1.png)
  
Quando uma mensagem entra no pipeline de transporte, um agente de transporte derivado da classe [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) pode atuar na mensagem durante qualquer evento SMTP que o agente está registrado. Um agente derivado da classe [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) pode atuar em qualquer um dos quatro eventos categorizadores que ele registrou para o. Um agente derivado da classe [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) pode agir em uma mensagem durante qualquer um dos eventos de entrega registrados. 
  
## <a name="transport-agents-and-server-roles"></a>Agentes de transporte e funções de servidor
<a name="ServerRoles"> </a>

As alterações na arquitetura da função de servidor no Exchange 2013 afetam agentes de transporte e o que seus agentes de transporte podem fazer. O Exchange 2013 inclui as seguintes funções de servidor:
  
- Servidor de caixa de correio — inclui protocolos de acesso para cliente, serviço de transporte, bancos de dados de caixa de correio e componentes de Unificação de mensagens. O servidor de caixa de correio se comunica diretamente com os serviços de domínio do Active Directory (AD DS), servidores de acesso para cliente e clientes de email, como o Outlook.
    
- Servidor de acesso para cliente — fornece autenticação, redirecionamento limitado, serviços de proxy e protocolos de acesso para cliente, como HTTP, POP, IMAP e SMTP.
    
- Servidor de transporte de Borda — roteia o email para dentro e para fora de uma organização. Os servidores de transporte de borda normalmente ficam no perímetro de uma topologia do Exchange.
    
Essa estrutura consolidada reduz o número de servidores que precisam ser implantados em um ambiente do Exchange 2013. Os administradores não precisam mais implantar servidores de transporte de Hub e de acesso para cliente em todos os sites do Active Directory que incluem um servidor de caixa de correio e não precisam mais atualizar todas as funções de servidor para aproveitar a nova funcionalidade.
  
Essas alterações na arquitetura da função de servidor podem afetar potencialmente o local no pipeline que seu agente pode responder a eventos. Se você tiver criado agentes de transporte para versões do Exchange anteriores ao Exchange 2013, revise as alterações arquitetônicas para determinar se precisa fazer qualquer alteração nos seus agentes.
  
A figura a seguir mostra como as alterações arquitetônicas no Exchange 2013 resultam em um pipeline de transporte consolidado e simplificado. Nesta figura, os servidores de acesso para cliente são identificados como CAS. E servidores de caixa de correio são rotulados MBX.
  
**Figura 2. Arquitetura de função de servidor do Exchange 2013**

![An image shows client traffic through an external firewall and Edge Transport on the left that passes traffic through a layer 4 load balance to a consolidated CAS array and set of mailbox servers in a database accessibility group on the right.](media/Transport_Agent_Concepts_Fig_3.png)
  
A figura a seguir mostra as interações entre as funções de servidor do Exchange 2013.
  
**Figura 3. Interações de servidor de acesso para cliente e caixa de correio**

![An image shows interactions starting with arrows from client traffic passing through a layer 4 load balance that has 4 targets in the CAS: IIS/HTTP Proxy, POP/IMAP, SMTP, and UM. The arrows pass to their complimentary targets in the mailbox store.](media/Transport_Agent_Concepts_Fig_4.png)
  
Para obter mais informações sobre alterações na arquitetura de função de servidor do Exchange 2013, consulte [exchange 2013 Architecture](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx#BKMK_Arch) em [What ' s New in Exchange 2013](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx). 
  
## <a name="transport-agent-classes"></a>Classes de agente de transporte
<a name="Create"> </a>

A classe que seu agente de transporte deriva determina os eventos para os quais o seu agente pode se registrar. O seu agente normalmente conterá uma classe de agente, uma fábrica de agentes, um ou mais manipuladores de eventos e o código que executará as ações que você deseja que seu agente realize.
  
A tabela a seguir lista as classes nas quais derivar cada tipo de agente.
  
**Tabela 2. Classes de agentes**

||||
|:-----|:-----|:-----|
|Tipo de agente  <br/> |Classe base de fábrica  <br/> |Classe base do agente  <br/> |
|Recebimento SMTP  <br/> |[SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|Caminhar  <br/> |[RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) <br/> |[RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> |
|Entrega  <br/> |[DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) <br/> |[DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) <br/> |
   
Essas classes de fábrica e de agentes fornecem propriedades e métodos que você pode usar para acessar eventos e mensagens de transporte. Implementar classes no seu agente que herdam dessas classes. Na classe derivada de Factory de agentes, substitua o método **CreateAgent** para que ele retorne uma nova instância da classe de agente. 
  
Os argumentos passados para os eventos podem conter uma instância da classe [EmailMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.EmailMessage.aspx) , que você pode usar para alterar as propriedades e o conteúdo da mensagem subjacente. Nem todas as informações de mensagem estão disponíveis em cada evento. Você deve determinar qual agente e qual evento é melhor para a tarefa que você deseja realizar. 
  
Os namespaces a seguir contêm tipos que podem ser usados para ler, gravar e modificar mensagens no pipeline de transporte:
  
- [Microsoft. Exchange. Data. MIME. decodificadores](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx)
    
- [Microsoft. Exchange. Data. ContentTypes. iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx)
    
- [Microsoft. Exchange. Data. MIME](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx)
    
- [Microsoft. Exchange. Data. ContentTypes. TNEF](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx)
    
- [Microsoft. Exchange. Data. ContentTypes. vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx)
    
Depois de escrever o agente de transporte, você [instala e gerencia seu agente](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx) usando o Shell de gerenciamento do Exchange. Para obter mais informações, consulte [Creating Transport Agents for Exchange 2013](creating-transport-agents-for-exchange-2013.md). 
  
## <a name="see-also"></a>Confira também

- [Agentes de transporte no Exchange](transport-agents-in-exchange-2013.md)    
- [Referência do agente de transporte para o Exchange 2013](transport-agent-reference-for-exchange-2013.md)   
- [Leitura e modificação de mensagens no pipeline de transporte do Exchange 2013](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)    
- [O que há de novo no Exchange 2013](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx)   
- [Arquitetura de função de servidor do Exchange 2013](https://blogs.technet.com/b/exchange/archive/2013/01/23/exchange-2013-server-role-architecture.aspx)    
- [Servidores de caixa de correio e acesso para cliente](https://technet.microsoft.com/library/jj150519%28v=exchg.150%29.aspx)   
- [Fluxo de email do Exchange Server 2013](https://technet.microsoft.com/library/aa996349.aspx)
- [Roteamento de email do Exchange Server 2013](https://technet.microsoft.com/library/aa998825%28v=exchg.150%29.aspx)   
- [PowerShell do Exchange Server (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
    

