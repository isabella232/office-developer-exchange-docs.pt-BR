---
title: Elementos de arquivo de configuração de agentes para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Agents
api_type:
- schema
ms.assetid: 3047653b-d712-46c1-ae0a-73f3975f5e9d
description: Encontre informações sobre os elementos XML no arquivo de configuração Agents e fetagents.config no Exchange 2013.
ms.openlocfilehash: dd58c4bc21a968db2ca5b13e0c53f7058b29f233
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751004"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a>Elementos de arquivo de configuração de agentes para o Exchange 2013

Encontre informações sobre os elementos XML no arquivo de configuração Agents e fetagents.config no Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013
  
Quando você instala o acesso para cliente ou a função de servidor de caixa de correio em um servidor Exchange, o instalador cria um arquivo XML que contém informações de configuração sobre os operadores que estão instalados no servidor. Você não pode gravar diretamente esse arquivo. 
  
O serviço Front End Transport é executado em servidores de acesso para cliente e grava um arquivo chamado fetagents.config. O serviço de transporte e o serviço de transporte de caixa de correio executados nos servidores de caixa de correio e gravar em um arquivo denominado Agents. Um computador que possui a função de servidor acesso para cliente e a função de servidor de caixa de correio terá um fetagents.config e um arquivo Agents. 
  
A única maneira com suporte para gravar esses arquivos é usando os cmdlets do agente de transporte no Shell de gerenciamento do Exchange. Para obter informações sobre os cmdlets do agente de transporte, consulte [Cmdlets de fluxo de email](http://technet.microsoft.com/en-us/library/aa998553%28v=exchg.150%29.aspx) no TechNet. 
  
> [!NOTE]
> Para distinguir entre os agentes que estendem o serviço Front End Transport no servidor de acesso para cliente e o serviço de transporte no servidor de caixa de correio, os cmdlets de agente de transporte tem um parâmetro _TransportService_ com um valor de "Hub" para o transporte serviço e "FrontEnd" para o serviço Front End Transport. 
  
Você pode ler a Agents ou arquivo fetagents.config para determinar a presença de e informações de configuração de um ou mais operadores no servidor. Esta documentação fornece uma referência que você pode usar para ler as informações do arquivo Agents exe ou o fetagents.config. O formato para ambos os arquivos é o mesmo. Esta documentação não fornece informações sobre como escrever para os arquivos.
  
> [!CAUTION]
> Usando métodos não suportados para gravar no arquivo Agents ou fetagents.config pode gerar resultados inesperados, inclusive falha de serviço de transporte ou agentes de transporte ou ambos. Não escreva diretamente a qualquer um desses arquivos. O único método suportado para gravar nesses arquivos é usando os cmdlets de agente de transporte do Shell de gerenciamento do Exchange. 
  
## <a name="location-of-the-transport-agent-configuration-files"></a>Local dos arquivos de configuração do agente de transporte
<a name="bk_ConfigLoc"> </a>

Quando você instala o Exchange 2013, o instalador cria um arquivo XML que é chamado agents.config.template ou fetagents.config.template, dependendo da função de servidor instalada, o \<ExchangeInstallFolder\>\TransportRoles\Agents pasta (onde \<ExchangeInstallFolder\> é a pasta na qual você instalou o Exchange 2013). Se você instalar a função de servidor acesso para cliente, o Exchange 2013 copia o arquivo fetagents.config.template para fetagents.config. Se você instalar a função de servidor de caixa de correio, o Exchange 2013 copia o arquivo agents.config.template para Agents. Exchange 2013 leituras e gravações esse arquivo, quando você altera a configuração de agentes de transporte no servidor.
  
## <a name="verifying-a-transport-agent-installation"></a>Verificando uma instalação do agente de transporte
<a name="bk_verifyinstall"> </a>

Você pode usar os recursos XML que o .NET Framework fornece para ler e validar o Agents ou o arquivo XML de fetagents.config. Para verificar a instalação e configuração de um agente de transporte, leia o XML no arquivo de configuração e localize o elemento de [agente](agent.md) que corresponde ao agente de transporte. Se não existir um elemento de **agente** para o agente de transporte específica, o agente de transporte não está instalado. Se o agente de transporte estiver instalado, você pode ler os atributos do elemento **agente** para determinar sua configuração. 
  
## <a name="configuration-file-element-hierarchy"></a>Hierarquia de elemento do arquivo de configuração
<a name="bk_elementref"> </a>

O código a seguir mostra a hierarquia de elemento no arquivo XML de configuração.
  
```XML
<configuration>
    <mexRuntime>
        <monitoring>
            <agentExecution/>
            <messageSnapshot/>
        </monitoring>
        <agentList>
            <agent/>
            <agent/>
            <agent />
        </agentList>
    </mexRuntim>
</configuration>
```

## <a name="in-this-section"></a>Nesta seção
<a name="bk_elementreflist"> </a>

- [agente](agent.md)
    
- [agentExecution](agentexecution.md)
    
- [agentList](agentlist.md)
    
- [configuração](configuration.md)
    
- [messageSnapshot](messagesnapshot.md)
    
- [mexRuntime](mexruntime.md)
    
- [monitoramento](monitoring.md)
    
## <a name="see-also"></a>Confira também

- [Agentes de transporte no Exchange](transport-agents-in-exchange-2013.md)
- [Transporte conceitos de agente no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)
- [Referência de agente de transporte do Exchange 2013](transport-agent-reference-for-exchange-2013.md)
- [Transporte namespaces de agente no Exchange 2013](transport-agent-namespaces-in-exchange-2013.md)
- [Cmdlets de fluxo de email](https://docs.microsoft.com/en-us/powershell/exchange/?view=exchange-ps)
    

