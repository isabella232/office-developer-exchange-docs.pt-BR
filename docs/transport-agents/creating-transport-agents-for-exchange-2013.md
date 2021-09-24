---
title: Criando agentes de transporte para Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d291ab78-7cdd-4dbe-a5f4-9dc8e9650a33
description: Encontre informações sobre como criar agentes de transporte personalizados para Exchange 2013 e os requisitos do sistema para criar um agente personalizado.
ms.openlocfilehash: ea5ae1fab85fde781cb365a21b7a40ccd52955b3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520952"
---
# <a name="creating-transport-agents-for-exchange-2013"></a>Criando agentes de transporte para Exchange 2013

Encontre informações sobre como criar agentes de transporte personalizados para Exchange 2013 e os requisitos do sistema para criar um agente personalizado.
  
**Aplica-se a:** Exchange Server 2013
  
Exchange Server 2013 inclui vários agentes de transporte que você pode usar para processar mensagens. Usando os assemblies que vêm com Exchange, você pode criar seus próprios agentes personalizados para executar tarefas específicas de acordo com as necessidades da sua organização. Por exemplo, você pode usar um agente de transporte SmtpReceiveAgent para interceptar mensagens recebidas por meio do protocolo SMTP e processar a mensagem para converter o formato do corpo para conter texto pré-formatado. Você pode usar um agente de transporte RoutingAgent para registrar as mensagens que passam pelo servidor na rota para outro servidor. Você também pode criar recursos mais complexos que usam mais de um tipo de agente. Por exemplo, para criar um agente antivírus, você pode implementar um SmtpReceiveAgent e um agente RoutingAgent. Se você tiver um componente em sua rede que não suporte o protocolo SMTP, poderá usar um agente de transporte DeliveryAgent para lidar com a comunicação entre seu servidor Exchange e seu componente externo. 
  
Este artigo fornece informações sobre os pré-requisitos e tarefas envolvidas na criação do seu próprio agente de transporte. Para obter informações sobre como criar agentes de transporte específicos, consulte [Create a RoutingAgent transport agent for Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [Create an SmtpReceiveAgent transport agent for Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)e [Create a DeliveryAgent transport agent for Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).
  
## <a name="prerequisites-for-creating-a-transport-agent"></a>Pré-requisitos para a criação de um agente de transporte
<a name="bk_prerequisites"> </a>

Veja a seguir os pré-requisitos necessários para implementar um agente de transporte:
  
- Um computador executando Exchange 2013 que está executando o serviço de Transporte de Front-End em um servidor de Acesso para Cliente ou Transporte de Borda ou o serviço de Transporte em um servidor de Caixa de Correio. Para obter informações sobre a arquitetura de função de servidor no Exchange 2013, consulte Conceitos de agente de [transporte em Exchange 2013](transport-agent-concepts-in-exchange-2013.md).
    
- Os assemblies a seguir para as classes de agente de transporte:
    
  - Microsoft.Exchange.Data.dll
    
  - Microsoft.Exchange.Data.Common.dll
    
  - Microsoft.Exchange.Transport.dll
    
- O .NET Framework 4.5
    
Também recomendamos que você instale o Visual Studio 2012. Você pode implementar agentes de transporte usando Visual Basic .NET ou C#.
  
## <a name="referencing-the-assemblies"></a>Fazendo referência aos assemblies
<a name="bk_ReferenceAssemblies"> </a>

Exchange 2013 fornece uma biblioteca de classes que suportam a extensão do Exchange de transporte. Essas classes exigem .NET Framework 4,5. Você pode implementar agentes de transporte com base nessas classes usando Visual Studio 2012.
  
O Exchange instalador 2013 instala assemblies usados para o desenvolvimento de agentes de transporte e os registra no cache de assembly global (GAC). Para começar a implementar um agente de transporte, crie uma referência à Microsoft. Exchange. Assembly Data.Transport em um projeto de biblioteca de classes.
  
## <a name="implementing-a-transport-agent"></a>Implementando um agente de transporte
<a name="bk_implementationExample"> </a>

O exemplo a seguir mostra uma implementação mínima de classes derivadas das classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) e [SmtpReceiveAgent.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) 
  
> [!CAUTION]
> Se vários agentes de transporte são instalados e registrados para o mesmo evento, todos os agentes serão invocados, mesmo que um agente remova todos os destinatários de um item de email. > Para evitar erros não tratamentos ou comportamento imprevisível, o agente de transporte deve lidar com casos em que a contagem de destinatários em um item de email seja igual a zero. 
  
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

Depois de compilar seu agente em uma DLL, você deve instalar e habilitar o agente em seu servidor de Exchange de desenvolvimento. No Shell de Gerenciamento Exchange, use o cmdlet [Install-TransportAgent](https://technet.microsoft.com/library/aa997998.aspx) para instalar seu agente e o cmdlet [Enable-TransportAgent](https://technet.microsoft.com/library/bb124921.aspx) para habilitar seu agente. Para obter informações sobre como usar o Shell de Gerenciamento Exchange, consulte [Exchange Server PowerShell (Exchange Shell](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)de Gerenciamento) .
  
> [!CAUTION]
> Os agentes de transporte têm acesso total a todas as mensagens de email que encontrarem. Exchange 2013 não restringe o comportamento de um agente de transporte. Agentes de transporte instável ou que contêm falhas de segurança podem afetar a estabilidade e a segurança do Exchange 2013. Portanto, você só deve instalar agentes de transporte em que você confia totalmente e que foram totalmente testados. 
  
Quando você usa o cmdlet **Install-TransportAgent** para instalar um agente, o Shell de Gerenciamento Exchange mantém um bloqueio no assembly. Para liberar o bloqueio no assembly, você deve fechar a instância do Shell de Gerenciamento Exchange que você usou para instalar o agente. Você não poderá atualizar o assembly até liberar o bloqueio. 
  
O exemplo a seguir mostra como usar o Shell de Gerenciamento Exchange para instalar e habilitar um agente chamado MyAgent usando uma classe derivada de [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) chamada MyAgents.MyAgentFactory. 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
Este exemplo nomeia o agente MyCustomAgent no servidor no qual o agente está instalado. O exemplo a seguir mostra como habilitar o agente chamado MyCustomAgent.
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
Para gerenciar um agente de transporte no serviço de Transporte de Front-End em um servidor de Acesso para Cliente, adicione o seguinte valor ao comando:  `-TransportService FrontEnd` . Por exemplo, para exibir os agentes de transporte no serviço de Transporte front-end, execute o seguinte comando.
  
 `Get-TransportAgent -TransportService FrontEnd`
  
Para obter mais informações sobre como instalar, habilenciar e gerenciar seu agente, consulte [Manage Transport Agents](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx).
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Criar um agente de transporte RoutingAgent para Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [Criar um agente de transporte SmtpReceiveAgent para Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [Criar um agente de transporte DeliveryAgent para Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a>Confira também

- [Conceitos de agente de transporte no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)   
- [Referência do agente de transporte Exchange 2013](transport-agent-reference-for-exchange-2013.md)
    

