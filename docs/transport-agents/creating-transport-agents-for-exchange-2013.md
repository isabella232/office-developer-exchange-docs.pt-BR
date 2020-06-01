---
title: Criando agentes de transporte para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d291ab78-7cdd-4dbe-a5f4-9dc8e9650a33
description: Encontre informações sobre como criar agentes de transporte personalizados para o Exchange 2013 e os requisitos de sistema para a criação de um agente personalizado.
ms.openlocfilehash: cb1cd180817524fe29a100a48d90444c75a77510
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462371"
---
# <a name="creating-transport-agents-for-exchange-2013"></a>Criando agentes de transporte para o Exchange 2013

Encontre informações sobre como criar agentes de transporte personalizados para o Exchange 2013 e os requisitos de sistema para a criação de um agente personalizado.
  
**Aplica-se a:** Exchange Server 2013
  
O Exchange Server 2013 inclui vários agentes de transporte que você pode usar para processar mensagens. Usando os assemblies que acompanham o Exchange, você pode criar seus próprios agentes personalizados para executar tarefas específicas de acordo com as necessidades da sua organização. Por exemplo, você pode usar um agente de transporte SmtpReceiveAgent para interceptar mensagens recebidas por meio do protocolo SMTP e processar a mensagem para converter o formato do corpo para conter texto pré-formatado. Você pode usar um agente de transporte RoutingAgent para registrar as mensagens que passam pelo servidor na rota para outro servidor. Você também pode criar recursos mais complexos que fazem uso de mais de um tipo de agente. Por exemplo, para criar um agente antivírus, é possível implementar um SmtpReceiveAgent e um agente do RoutingAgent. Se você tiver um componente em sua rede que não ofereça suporte ao protocolo SMTP, poderá usar um agente de transporte do DeliveryAgent para lidar com a comunicação entre o servidor do Exchange e o componente externo. 
  
Este artigo fornece informações sobre os pré-requisitos e as tarefas envolvidas na criação de seu próprio agente de transporte. Para obter informações sobre como criar agentes de transporte específicos, consulte [criar um agente de transporte RoutingAgent para o exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [criar um agente de transporte SmtpReceiveAgent para o Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)e [criar um agente de transporte DeliveryAgent para o Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).
  
## <a name="prerequisites-for-creating-a-transport-agent"></a>Pré-requisitos para a criação de um agente de transporte
<a name="bk_prerequisites"> </a>

Estes são os pré-requisitos de que você precisa para implementar um agente de transporte:
  
- Um computador executando o Exchange 2013 que está executando o serviço de transporte de front end em um servidor de transporte de borda ou acesso para cliente, ou o serviço de transporte em um servidor de caixa de correio. Para obter informações sobre a arquitetura de função de servidor no Exchange 2013, consulte [Transport Agent Concepts in exchange 2013](transport-agent-concepts-in-exchange-2013.md).
    
- Os seguintes assemblies para as classes de agente de transporte:
    
  - Microsoft. Exchange. Data. dll
    
  - Microsoft. Exchange. Data. Common. dll
    
  - Microsoft. Exchange. Transport. dll
    
- O .NET Framework 4,5
    
Também é recomendável instalar o Visual Studio 2012. Você pode implementar agentes de transporte usando o Visual Basic .NET ou C#.
  
## <a name="referencing-the-assemblies"></a>Fazendo referência aos assemblies
<a name="bk_ReferenceAssemblies"> </a>

O Exchange 2013 fornece uma biblioteca de classes que dão suporte à extensão do comportamento de transporte do Exchange. Essas classes exigem o .NET Framework 4,5. Você pode implementar agentes de transporte com base nessas classes usando o Visual Studio 2012.
  
O instalador do Exchange 2013 instala assemblies que são usados para o desenvolvimento do agente de transporte e os registra no cache de assembly global (GAC). Para começar a implementar um agente de transporte, crie uma referência ao assembly Microsoft. Exchange. Data. Transport em um projeto de biblioteca de classes.
  
## <a name="implementing-a-transport-agent"></a>Implementar um agente de transporte
<a name="bk_implementationExample"> </a>

O exemplo a seguir mostra uma implementação mínima de classes que derivam das classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) e [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) . 
  
> [!CAUTION]
> Se vários agentes de transporte estiverem instalados e registrados para o mesmo evento, todos os agentes serão invocados, mesmo que um agente remova todos os destinatários de um item de email. > para evitar erros não tratados ou comportamento imprevisível, seu agente de transporte deve lidar com casos em que a contagem de destinatários em um item de email é igual a zero. 
  
```cs
using System;
using System.Collections.Generic;
using System.Text;
using Microsoft.Exchange.Data.Transport;
using Microsoft.Exchange.Data.Transport.Smtp;
namespace MyAgents
{
    public sealed class MyAgentFactory : SmtpReceiveAgentFactory
    {
        public override SmtpReceiveAgent CreateAgent(SmtpServer server)
        {
            return new MyAgent();
        }
    }
    public class MyAgent : SmtpReceiveAgent
    {
        public MyAgent()
        {
            this.OnEndOfData += new EndOfDataEventHandler(MyEndOfDataHandler);
        }
        private void MyEndOfDataHandler (ReceiveMessageEventSource source, EndOfDataEventArgs e)
        {
            // The following line appends text to the subject of the message that caused the event.
            e.MailItem.Message.Subject += " - this text appended by MyAgent";
        }
    }
}
```

```vb
Imports System
Imports System.Collections.Generic
Imports System.Text
Imports Microsoft.Exchange.Data.Transport
Imports Microsoft.Exchange.Data.Transport.Smtp
Namespace MyAgents
    NotInheritable Class MyAgentFactory
        Inherits SmtpReceiveAgentFactory
        Public Overrides Function CreateAgent(ByVal server as SmtpServer) As SmtpReceiveAgent
            Return New MyAgent
        End Function
    End Class
    Public Class MyAgent
        Inherits SmtpReceiveAgent
        Private Sub MyEndOfDataHandler(ByVal source As ReceiveMessageEventSource, ByVal e As EndOfDataEventArgs) Handles Me.OnEndOfData
            ' The following line appends text to the subject of the message that caused the event.
            e.MailItem.Message.Subject &amp;= e.MailItem.Message.Subject + " - this text appended by MyAgent"
        End Sub
    End Class
End Namespace
```

## <a name="installing-and-enabling-an-agent"></a>Instalando e habilitando um agente
<a name="bk_InstallEnable"> </a>

Depois de compilar o seu agente para uma DLL, você deve instalar e habilitar o agente no seu servidor do Exchange de desenvolvimento. No Shell de gerenciamento do Exchange, use o cmdlet [Install-TransportAgent](https://technet.microsoft.com/library/aa997998.aspx) para instalar o seu agente e o cmdlet [Enable-TransportAgent](https://technet.microsoft.com/library/bb124921.aspx) para habilitar o seu agente. Para obter informações sobre como usar o Shell de gerenciamento do Exchange, consulte [Exchange Server PowerShell (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).
  
> [!CAUTION]
> Os agentes de transporte têm acesso total a todas as mensagens de email que encontrarem. O Exchange 2013 não restringe o comportamento de um agente de transporte. Os agentes de transporte instáveis ou que contêm falhas de segurança podem afetar a estabilidade e a segurança do Exchange 2013. Portanto, você deve instalar somente agentes de transporte com confiança total e que foram totalmente testados. 
  
Quando você usa o cmdlet **Install-TransportAgent** para instalar um agente, o Shell de gerenciamento do Exchange mantém um bloqueio no assembly. Para liberar o bloqueio no assembly, você deve fechar a instância do Shell de gerenciamento do Exchange que você usou para instalar o agente. Você não poderá atualizar o assembly até que você libere o bloqueio. 
  
O exemplo a seguir mostra como usar o Shell de gerenciamento do Exchange para instalar e habilitar um agente chamado myagent usando uma classe derivada de [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) chamada myagents. MyAgentFactory. 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
Este exemplo nomeia o agente MyCustomAgent no servidor no qual o agente está instalado. O exemplo a seguir mostra como habilitar o agente chamado MyCustomAgent.
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
Para gerenciar um agente de transporte no serviço de transporte de front-end em um servidor de acesso para cliente, adicione o seguinte valor ao comando: `-TransportService FrontEnd` . Por exemplo, para exibir os agentes de transporte no serviço de transporte de front-end, execute o comando a seguir.
  
 `Get-TransportAgent -TransportService FrontEnd`
  
Para obter mais informações sobre como instalar, habilitar e gerenciar o seu agente, consulte [Manage Transport Agents](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx).
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Criar um agente de transporte RoutingAgent para o Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [Criar um agente de transporte SmtpReceiveAgent para o Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [Criar um agente de transporte DeliveryAgent para o Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a>Também consulte

- [Conceitos de agente de transporte no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)   
- [Referência do agente de transporte para o Exchange 2013](transport-agent-reference-for-exchange-2013.md)
    

