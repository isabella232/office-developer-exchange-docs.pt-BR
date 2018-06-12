---
title: Criando os agentes de transporte do Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d291ab78-7cdd-4dbe-a5f4-9dc8e9650a33
description: Encontre informações sobre como criar os agentes de transporte personalizado para o Exchange 2013 e os requisitos de sistema para a criação de um agente personalizado.
ms.openlocfilehash: 6146e37c44441bed1d30d08f71ede255dba26440
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751003"
---
# <a name="creating-transport-agents-for-exchange-2013"></a>Criando os agentes de transporte do Exchange 2013

Encontre informações sobre como criar os agentes de transporte personalizado para o Exchange 2013 e os requisitos de sistema para a criação de um agente personalizado.
  
**Aplica-se a:** Exchange Server 2013
  
Exchange Server 2013 inclui vários agentes de transporte que podem ser usados para processar mensagens. Usando os assemblies que vêm com o Exchange, você pode criar seus próprios agentes personalizados para executar tarefas específicas de acordo com as necessidades da sua organização. Por exemplo, você pode usar um agente de transporte SmtpReceiveAgent a intercepção mensagens que são recebidos por meio do protocolo SMTP e o processo a mensagem para converter o formato do corpo para conter texto pré-formatado. Você pode usar um agente de transporte RoutingAgent para efetuar as mensagens que passam pelo servidor em rota para outro servidor. Você também pode criar mais complexos recursos que tornam o usam das mais de um tipo de agente. Por exemplo, para criar um agente de antivírus, você pode implementar um SmtpReceiveAgent e um agente de RoutingAgent. Se você tiver um componente da rede que não suporta o protocolo SMTP, você pode usar um agente de transporte DeliveryAgent para lidar com a comunicação entre o seu servidor do Exchange e seu componente externo. 
  
Este artigo fornece informações sobre os pré-requisitos para e as tarefas envolvidas na criação de seu próprio agente de transporte. Para obter informações sobre a criação de agentes de transporte específica, consulte [criar um agente de transporte do Exchange 2013 RoutingAgent](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [criar um agente de transporte SmtpReceiveAgent para o Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)e [criar um agente de transporte DeliveryAgent para Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).
  
## <a name="prerequisites-for-creating-a-transport-agent"></a>Pré-requisitos para a criação de um agente de transporte
<a name="bk_prerequisites"> </a>

Estes são os pré-requisitos necessários para implementar um agente de transporte:
  
- Um computador executando o Exchange 2013 que está executando o serviço Front End Transport em um servidor de acesso para cliente ou de transporte de borda, ou o serviço de transporte em um servidor de caixa de correio. Para obter informações sobre a arquitetura da função de servidor no Exchange 2013, consulte [Transporte conceitos de agente no Exchange 2013](transport-agent-concepts-in-exchange-2013.md).
    
- Os assemblies a seguir para as classes de agente de transporte:
    
  - Microsoft.Exchange.Data.dll
    
  - Microsoft.Exchange.Data.Common.dll
    
  - Microsoft.Exchange.Transport.dll
    
- O .NET Framework 4.5
    
Também recomendamos que você instale o Visual Studio 2012. Você pode implementar agentes de transporte usando o Visual Basic .NET ou c#.
  
## <a name="referencing-the-assemblies"></a>Referenciando os assemblies
<a name="bk_ReferenceAssemblies"> </a>

Exchange 2013 fornece uma biblioteca de classes que oferecem suporte a extensão de comportamento de transporte do Exchange. Essas classes exigem o .NET Framework 4.5. Você pode implementar os agentes de transporte com base nessas classes usando o Visual Studio 2012.
  
O instalador do Exchange 2013 instala os assemblies que são usados para desenvolvimento do agente de transporte e registra-los no cache de assembly global (GAC). Para começar a implementar um agente de transporte, crie uma referência para o assembly Microsoft.Exchange.Data.Transport em um projeto de biblioteca de classe.
  
## <a name="implementing-a-transport-agent"></a>Implementando um agente de transporte
<a name="bk_implementationExample"> </a>

O exemplo a seguir mostra um mínimo de implementação das classes que derivam das classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) e [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) . 
  
> [!CAUTION]
> Se vários agentes de transporte são instalados e registrados para o mesmo evento, todos os operadores serão chamados, mesmo se um agente remove todos os destinatários de um item de email. > Para evitar erros não tratados ou comportamento imprevisível, o agente de transporte deve lidar com casos em que a contagem de destinatários em um item de email é igual a zero. 
  
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

## <a name="installing-and-enabling-an-agent"></a>Instalar e ativar um operador
<a name="bk_InstallEnable"> </a>

Depois que você compila seu agente para uma DLL, você deve instalar e habilitar o agente em seu servidor do Exchange de desenvolvimento. No Shell de gerenciamento do Exchange, use o cmdlet [Install-TransportAgent](http://technet.microsoft.com/en-us/library/aa997998.aspx) para instalar o agente e o cmdlet [Enable-TransportAgent](http://technet.microsoft.com/en-us/library/bb124921.aspx) para habilitar o agente. Para obter informações sobre como usar o Shell de gerenciamento do Exchange, consulte [Exchange Server PowerShell (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).
  
> [!CAUTION]
> Agentes de transporte têm acesso total a todas as mensagens de email que eles encontrem. Exchange 2013 não restringe o comportamento de um agente de transporte. Agentes de transporte que estão instáveis ou que contenham falhas de segurança podem afetar a estabilidade e a segurança do Exchange 2013. Portanto, você deve instalar somente os agentes de transporte que você confia totalmente e que foram testados totalmente. 
  
Quando você usa o cmdlet **Install-TransportAgent** para instalar um operador, o Shell de gerenciamento do Exchange mantém um bloqueio no assembly. Para liberar o bloqueio do assembly, você deve fechar a instância do Shell de gerenciamento do Exchange que você usou para instalar o agente. Não será possível atualizar o assembly até que você libere o bloqueio. 
  
O exemplo a seguir mostra como usar o Shell de gerenciamento do Exchange para instalar e habilitar um agente chamado MyAgent usando uma classe derivada de [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) chamado MyAgents.MyAgentFactory. 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
Este exemplo chama o agente MyCustomAgent no servidor em que o agente está instalado. O exemplo a seguir mostra como habilitar o agente denominado MyCustomAgent.
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
Para gerenciar um agente de transporte no serviço Front End Transport em um servidor de acesso para cliente, adicione o seguinte valor ao comando: `-TransportService FrontEnd`. Por exemplo, para exibir os agentes de transporte no serviço Front End Transport, execute o seguinte comando.
  
 `Get-TransportAgent -TransportService FrontEnd`
  
Para obter mais informações sobre como instalar, habilitando e gerenciando seu agente, consulte [Gerenciar agentes de transporte](http://technet.microsoft.com/en-us/library/bb125175%28v=exchg.150%29.aspx).
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Criar um agente de transporte RoutingAgent para o Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [Criar um agente de transporte SmtpReceiveAgent para o Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [Criar um agente de transporte DeliveryAgent para o Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a>Confira também

- [Transporte conceitos de agente no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)   
- [Referência de agente de transporte do Exchange 2013](transport-agent-reference-for-exchange-2013.md)
    

