---
title: Elementos de arquivo de configuração de agentes para Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Agents
api_type:
- schema
ms.assetid: 3047653b-d712-46c1-ae0a-73f3975f5e9d
description: Encontre informações sobre os elementos XML no arquivo agents.config e fetagents.config de configuração Exchange 2013.
ms.openlocfilehash: bdf394130f7818c5b956e8b15eed86a6318b9698
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510418"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a>Elementos de arquivo de configuração de agentes para Exchange 2013

Encontre informações sobre os elementos XML no arquivo agents.config e fetagents.config de configuração Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013
  
Quando você instala o Acesso para Cliente ou a função de servidor de Caixa de Correio em um servidor Exchange, o instalador cria um arquivo XML que contém informações de configuração sobre agentes instalados no servidor. Não é possível gravar diretamente nesse arquivo. 
  
O serviço de Transporte de Front-End é executado em servidores de Acesso para Cliente e grava em um arquivo chamado fetagents.config. O serviço de Transporte e o serviço de Transporte de Caixa de Correio são executados em servidores de Caixa de Correio e escrevem em um arquivo chamado agents.config. Um computador que tenha a função de servidor de Acesso para Cliente e a função de servidor de Caixa de Correio terá um fetagents.config e um arquivo agents.config cliente. 
  
A única maneira suportada de gravar nesses arquivos é usando os cmdlets do agente de transporte no Shell de Gerenciamento Exchange. Para obter informações sobre os cmdlets do agente de transporte, consulte [Mail Flow Cmdlets](https://technet.microsoft.com/library/aa998553%28v=exchg.150%29.aspx) no TechNet. 
  
> [!NOTE]
> Para distinguir entre agentes que estendem o serviço de Transporte de Front-End no servidor de Acesso para Cliente e o serviço de Transporte no servidor de Caixa de Correio, os cmdlets de agente de transporte têm um parâmetro  _TransportService_ com um valor de "Hub" para o serviço de Transporte e "FrontEnd" para o serviço de Transporte front-end. 
  
Você pode ler o arquivo agents.config ou fetagents.config para determinar a presença e informações de configuração de um ou mais agentes no servidor. Esta documentação fornece uma referência que você pode usar para ler as informações no arquivo agents.config ou no fetagents.config. O formato para ambos os arquivos é o mesmo. Esta documentação não fornece informações sobre como gravar nos arquivos.
  
> [!CAUTION]
> Usar métodos sem suporte para gravar no arquivo agents.config ou fetagents.config pode produzir resultados inesperados, incluindo falha do serviço de transporte ou agentes de transporte ou ambos. Não escreva diretamente em nenhum desses arquivos. O único método suportado para escrever nesses arquivos é usando os cmdlets do agente de transporte do Shell de Gerenciamento Exchange gerenciamento. 
  
## <a name="location-of-the-transport-agent-configuration-files"></a>Local dos arquivos de configuração do agente de transporte
<a name="bk_ConfigLoc"> </a>

Quando você instala o Exchange 2013, o instalador cria um arquivo XML chamado agents.config.template ou fetagents.config.template, dependendo da função de servidor instalada, na pasta \TransportRoles\Agents (onde está a pasta na qual você instalou o \<ExchangeInstallFolder\> \<ExchangeInstallFolder\> Exchange 2013). Se você instalar a função de servidor de Acesso para Cliente, Exchange 2013 copia o arquivo fetagents.config.template para fetagents.config. Se você instalar a função de servidor de Caixa de Correio, Exchange 2013 copia o arquivo agents.config.template para agents.config. Exchange 2013 lê e grava esse arquivo quando você altera a configuração dos agentes de transporte no servidor.
  
## <a name="verifying-a-transport-agent-installation"></a>Verificar a instalação de um agente de transporte
<a name="bk_verifyinstall"> </a>

Você pode usar os recursos XML que o .NET Framework fornece para ler e validar o agents.config ou o arquivo XML do fetagents.config. Para verificar a instalação e a configuração de um agente [](agent.md) de transporte, leia o XML no arquivo de configuração e encontre o elemento agente que corresponde ao agente de transporte. Se um **elemento de** agente para o agente de transporte específico não existir, o agente de transporte não será instalado. Se o agente de transporte estiver instalado, você poderá ler os atributos do **elemento agente** para determinar sua configuração. 
  
## <a name="configuration-file-element-hierarchy"></a>Hierarquia de elementos de arquivo de configuração
<a name="bk_elementref"> </a>

O código a seguir mostra a hierarquia de elementos no arquivo XML de configuração.
  
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

- [agent](agent.md)
    
- [agentExecution](agentexecution.md)
    
- [agentList](agentlist.md)
    
- [configuration](configuration.md)
    
- [messageSnapshot](messagesnapshot.md)
    
- [mexRuntime](mexruntime.md)
    
- [monitoramento](monitoring.md)
    
## <a name="see-also"></a>Confira também

- [Agentes de transporte no Exchange](transport-agents-in-exchange-2013.md)
- [Conceitos de agente de transporte no Exchange 2013](transport-agent-concepts-in-exchange-2013.md)
- [Referência do agente de transporte Exchange 2013](transport-agent-reference-for-exchange-2013.md)
- [Namespaces do agente de transporte Exchange 2013](transport-agent-namespaces-in-exchange-2013.md)
- [Cmdlets Flow email](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)
    

