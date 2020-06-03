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
description: Encontre informações sobre os elementos XML no arquivo de configuração Agents. config e fetagents. config no Exchange 2013.
ms.openlocfilehash: f19fe8316a78cef668db881e630562d3be8be64a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461566"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a>Elementos de arquivo de configuração de agentes para o Exchange 2013

Encontre informações sobre os elementos XML no arquivo de configuração Agents. config e fetagents. config no Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013
  
Quando você instala a função de servidor Acesso para cliente ou caixa de correio em um servidor Exchange, o instalador cria um arquivo XML que contém informações de configuração sobre os agentes instalados no servidor. Você não pode gravar diretamente neste arquivo. 
  
O serviço de transporte de front-end é executado em servidores de acesso para cliente e grava em um arquivo chamado fetagents. config. O serviço de transporte e o serviço de transporte de caixa de correio são executados em servidores de caixa de correio e grava em um arquivo chamado Agents. config. Um computador que tenha a função de servidor de acesso para cliente e a função de servidor de caixa de correio terá um fetagents. config e um arquivo agents. config. 
  
A única maneira compatível de gravar nesses arquivos é usando os cmdlets do agente de transporte no Shell de gerenciamento do Exchange. Para obter informações sobre os cmdlets do agente de transporte, consulte [cmdlets de fluxo de emails](https://technet.microsoft.com/library/aa998553%28v=exchg.150%29.aspx) no TechNet. 
  
> [!NOTE]
> Para distinguir entre agentes que estendem o serviço de transporte de front-end no servidor de acesso para cliente e o serviço de transporte no servidor de caixa de correio, os cmdlets do agente de transporte têm um parâmetro _TransportService_ com um valor de "Hub" para o serviço de transporte e "frontend" para o serviço de transporte de front-end. 
  
Você pode ler o arquivo agents. config ou fetagents. config para determinar a presença e as informações de configuração de um ou mais agentes no servidor. Esta documentação fornece uma referência que você pode usar para ler as informações no arquivo agents. config ou no fetagents. config. O formato de ambos os arquivos é o mesmo. Esta documentação não fornece informações sobre como gravar nos arquivos.
  
> [!CAUTION]
> O uso de métodos sem suporte para gravar no arquivo agents. config ou fetagents. config pode produzir resultados inesperados, incluindo a falha do serviço de transporte ou agentes de transporte, ou ambos. Não escreva diretamente para nenhum desses arquivos. O único método com suporte para gravar nesses arquivos é usando os cmdlets do agente de transporte do Shell de gerenciamento do Exchange. 
  
## <a name="location-of-the-transport-agent-configuration-files"></a>Local dos arquivos de configuração do agente de transporte
<a name="bk_ConfigLoc"> </a>

Quando você instala o Exchange 2013, o instalador cria um arquivo XML chamado Agents. config. Template ou fetagents. config. Template, dependendo da função de servidor instalada, na \<ExchangeInstallFolder\> pasta \TransportRoles\Agents (onde \<ExchangeInstallFolder\> é a pasta na qual você instalou o Exchange 2013). Se você instalar a função de servidor Acesso para cliente, o Exchange 2013 copiará o arquivo fetagents. config. Template para fetagents. config. Se você instalar a função de servidor caixa de correio, o Exchange 2013 copiará o arquivo agents. config. Template para o Agents. config. O Exchange 2013 lê e grava esse arquivo quando você altera a configuração dos agentes de transporte no servidor.
  
## <a name="verifying-a-transport-agent-installation"></a>Verificar a instalação de um agente de transporte
<a name="bk_verifyinstall"> </a>

Você pode usar os recursos de XML que o .NET Framework fornece para ler e validar os agentes. config ou o arquivo XML fetagents. config. Para verificar a instalação e a configuração de um agente de transporte, leia o XML no arquivo de configuração e localize o elemento do [agente](agent.md) que corresponde ao agente de transporte. Se não existir um elemento de **agente** para o agente de transporte específico, o agente de transporte não será instalado. Se o agente de transporte estiver instalado, você poderá ler os atributos do elemento **Agent** para determinar sua configuração. 
  
## <a name="configuration-file-element-hierarchy"></a>Hierarquia de elemento do arquivo de configuração
<a name="bk_elementref"> </a>

O código a seguir mostra a hierarquia do elemento no arquivo XML de configuração.
  
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

- [Agente](agent.md)
    
- [agentExecution](agentexecution.md)
    
- [agentlist](agentlist.md)
    
- [configuration](configuration.md)
    
- [messageSnapshot](messagesnapshot.md)
    
- [mexRuntime](mexruntime.md)
    
- [monitoramento](monitoring.md)
    
## <a name="see-also"></a>Confira também

- [Agentes de transporte no Exchange](transport-agents-in-exchange-2013.md)
- [Conceitos de agente de transporte no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)
- [Referência do agente de transporte para o Exchange 2013](transport-agent-reference-for-exchange-2013.md)
- [Namespaces do agente de transporte no Exchange 2013](transport-agent-namespaces-in-exchange-2013.md)
- [Cmdlets de fluxo de emails](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)
    

