---
title: Backup e restauração para o Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 329902d9-0ecb-4cfb-86dd-5ce863deff3f
description: Encontre informações sobre a criação de backup e restaurar aplicativos para o Exchange 2013.
ms.openlocfilehash: 9eceb3d512a73ad9cb07a01864fb8b029d5b5772
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750627"
---
# <a name="backup-and-restore-for-exchange"></a>Backup e restauração para o Exchange
  
Exchange Server 2013 fornece grupos de disponibilidade de banco de dados (DAGs), que ajudam a manter os dados armazenados seguros e disponíveis e reduzir a necessidade de backup personalizado e restaurar aplicativos. DAGs permitem a redundância de dados fora da empresa ajudar a garantir que você não perca dados. No entanto, muitos planos de recuperação de desastres continuam a incluir mais tradicional de backup e restauração de métodos e sistemas, incluindo aplicativos personalizados, para redundância com o DAG. Para ajudar a garantir a disponibilidade de dados e redundância em sua organização, você pode criar aplicativos personalizados que usam tecnologias de sistema operacional do Exchange Server e Windows Server para fazer backup e restaurar dados do Exchange.

<a name="bk_plugin"> </a>

## <a name="backup-technologies-in-exchange-2013"></a>Tecnologias de backup no Exchange 2013

Exchange 2013 inclui um plug-in para o Backup do Windows Server que os administradores podem usar para fazer backups baseados em VSS dos dados do Exchange. Os administradores também podem usar o Backup do Windows Server para fazer backup e restaurar bancos de dados do Exchange. Se você estiver criando um backup e restaurar o aplicativo para o Exchange 2013, você precisará criar um aplicativo sensível ao Exchange que suporta o gravador VSS do Exchange 2013 e use a API CHKSGFILES para validar a consistência dos que o backup. Para obter mais informações, consulte [Validate integridade do backup, usando a API CHKSGFILES no Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md).

<a name="bk_vsswriter"> </a>

## <a name="vss-writer-in-exchange-2013"></a>Gravador VSS no Exchange 2013

Exchange 2013 apresenta uma alteração significativa para a arquitetura de gravador VSS no Exchange Server 2010 e o Exchange Server 2007. Exchange 2010 e Exchange 2007 incluem dois escritores VSS: uma dentro do serviço de repositório de informações do Exchange (store.exe) e outra dentro do serviço de replicação do Exchange (msexchangerepl.exe). No Exchange 2013, a funcionalidade de gravador VSS está localizada no serviço de replicação do Exchange. O aplicativo de backup e restauração usa o gravador VSS do novo, chamado o gravador do Microsoft Exchange, para fazer backup de cópias ativas e passivas de banco de dados e restaurar o backup cópias de banco de dados. Embora o gravador VSS do novo é executado no serviço de replicação do Exchange, o serviço de armazenamento de informações do Exchange deve estar executando para que o escritor esteja disponível. Como resultado, os dois serviços são necessárias para fazer backup ou restaurar bancos de dados do Exchange.
  
Embora a arquitetura de gravador VSS foi atualizada no Exchange 2013, a funcionalidade subjacente não foi alterado. Se você criou um aplicativo de backup e restauração para o Exchange 2010, você não precisará fazer alterações em seu aplicativo para o Exchange 2013. Certifique-se de que recompilar seu aplicativo com os arquivos mais recentes para garantir a compatibilidade. Para fazer backup e restaurar aplicativos criados para o Exchange 2007 ou versões anteriores, você precisará reescrever seus códigos para usar a API de CHKSGFILES mais recente.
  
## <a name="what-you-need-to-know-about-vss-backup-and-restore"></a>O que você precisa saber sobre o VSS backup e restauração

|Se você está se perguntando sobre...|Leia isto|
|:-----|:-----|
|Application architectures  <br/> |Backup e restauração de aplicativos que usam o VSS para fazer backup de bancos de dados geralmente consistem em um serviço em segundo plano que executa o backup, um serviço de agendamento e um console de aplicativo do Windows GUI que controla e configura o backup e restaurar o sistema do Exchange.  <br/> |
|Remote usage  <br/> |Aplicativos que usam VSS para fazer backup de servidores do Exchange devem ser executados no Windows Server 2008 computador no qual o processo de armazenamento do Exchange está sendo executado. Devido a flexibilidade em sistemas de armazenamento grande, o hardware que hospeda os volumes de armazenamento não pode ser fisicamente parte do computador que executa o Windows Server 2008.  <br/> |
|Languages and tools  <br/> |Você pode usar qualquer idioma compatível COM para usar o VSS. Ele é usado com mais frequência em aplicativos escritos em C++. Porque você precisou para levar o armazenamento do Exchange offline para criar cópias de sombra, aplicativos de backup são geralmente urgentes, que na maioria dos casos, facilita a utilização de idiomas como o Visual Basic ou o VBScript impraticável.  <br/> |
|Managed implementation  <br/> |Você pode usar as APIs de VSS em um ambiente de código gerenciado por meio de um Assembly de interoperabilidade COM.  <br/> |
|Scriptable  <br/> |Sim, mas não recomendado.  <br/> |
|Ferramentas de teste e depuração disponíveis  <br/> |Não há ferramentas especiais são necessárias para depurar aplicativos que usam o VSS do Windows.  <br/> |
   
## <a name="in-this-section"></a>Nesta se��o

- [Conceitos de backup e restauração do Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Criar um backup e restaurar aplicativos para o Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Referência de classe CChkSGFiles](cchksgfiles-class-reference.md)
    
## <a name="see-also"></a>Confira também

- [Serviço de cópias de sombra de volume (Windows)](http://msdn.microsoft.com/en-us/library/windows/desktop/bb968832%28v=vs.85%29.aspx)   
- [Explorar a API Gerenciada pelo EWS, EWS e serviços Web no Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [Shell de Gerenciamento do Exchange](../management/exchange-management-shell.md)   
- [Agentes de transporte no Exchange](../transport-agents/transport-agents-in-exchange-2013.md) 
    

