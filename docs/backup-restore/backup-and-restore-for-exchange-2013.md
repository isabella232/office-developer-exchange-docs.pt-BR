---
title: Backup e restauração para o Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 329902d9-0ecb-4cfb-86dd-5ce863deff3f
description: Encontre informações sobre a criação de aplicativos de backup e restauração para o Exchange 2013.
ms.openlocfilehash: 1c5d99be60501fd1c4414ea22294bd05645bb0a7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455237"
---
# <a name="backup-and-restore-for-exchange"></a>Backup e restauração para o Exchange
  
O Exchange Server 2013 fornece grupos de disponibilidade de banco de dados (DAGs), que ajudam a manter os dados armazenados seguros e disponíveis e a reduzir a necessidade de aplicativos personalizados de backup e restauração. DAGs habilitar a redundância de dados fora do site para ajudar a garantir que você não perca os dados. No entanto, muitos planos de recuperação de desastres continuam a incluir mais sistemas e métodos de backup e restauração tradicionais, incluindo aplicativos personalizados, para redundância com o DAG. Para ajudar a garantir a disponibilidade e a redundância de dados em sua organização, você pode criar aplicativos personalizados que usem as tecnologias de sistema operacional do Exchange Server e do Windows Server para fazer backup e restaurar os dados do Exchange.

<a name="bk_plugin"> </a>

## <a name="backup-technologies-in-exchange-2013"></a>Tecnologias de backup no Exchange 2013

O Exchange 2013 inclui um plug-in para o backup do Windows Server que os administradores podem usar para fazer backups baseados em VSS dos dados do Exchange. Os administradores também podem usar o backup do Windows Server para fazer backup e restaurar os bancos de dados do Exchange. Se você estiver criando um aplicativo de backup e restauração para o Exchange 2013, precisará criar um aplicativo compatível com o Exchange que ofereça suporte ao gravador VSS para o Exchange 2013 e usar a API CHKSGFILES para validar a consistência desse backup. Confira mais informações [em validar integridade do backup usando a API CHKSGFILES no Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md).

<a name="bk_vsswriter"> </a>

## <a name="vss-writer-in-exchange-2013"></a>Gravador VSS no Exchange 2013

O Exchange 2013 introduz uma alteração significativa na arquitetura de gravador VSS no Exchange Server 2010 e no Exchange Server 2007. O Exchange 2010 e o Exchange 2007 incluem dois gravadores VSS: um dentro do serviço de armazenamento de informações do Exchange (Store. exe) e um dentro do serviço de replicação do Exchange (MSExchangeRepl. exe). No Exchange 2013, a funcionalidade do gravador VSS está localizada no serviço de replicação do Exchange. O aplicativo de backup e restauração usa o novo gravador VSS, chamado de gravador do Microsoft Exchange, para fazer o backup de cópias ativas e passivas do banco de dados e para restaurar cópias de bancos de dados de backup. Embora o novo gravador VSS seja executado no serviço de replicação do Exchange, o serviço de armazenamento de informações do Exchange deve estar em execução para que o gravador esteja disponível. Com isso, ambos os serviços são necessários para o backup ou a restauração de bancos de dados do Exchange.
  
Embora a arquitetura do gravador VSS tenha sido atualizada no Exchange 2013, a funcionalidade subjacente não foi alterada. Se você tiver criado um aplicativo de backup e restauração para o Exchange 2010, não será necessário fazer qualquer alteração no aplicativo para o Exchange 2013. Certifique-se de recompilar seu aplicativo com os arquivos mais recentes para garantir a compatibilidade. Para aplicativos de backup e restauração criados para o Exchange 2007 ou versões anteriores, você precisará reescrever seu código para usar a API CHKSGFILES mais recente.
  
## <a name="what-you-need-to-know-about-vss-backup-and-restore"></a>O que você precisa saber sobre o backup e a restauração VSS

|Se você estiver se perguntando sobre...|Leia isto|
|:-----|:-----|
|Arquiteturas de aplicativos  <br/> |Os aplicativos de backup e restauração que usam o VSS para fazer backup de bancos de dados do Exchange geralmente consistem em um serviço de plano de fundo que realiza o backup, um serviço de agendamento e um console de aplicativo da GUI do Windows que controla e configura o sistema de backup e restauração.  <br/> |
|Uso remoto  <br/> |Os aplicativos que usam o VSS para fazer backup de servidores do Exchange devem ser executados no computador com Windows Server 2008 no qual o processo de armazenamento do Exchange está sendo executado. Devido à flexibilidade em sistemas de armazenamento de grande porte, o hardware que hospeda os volumes de armazenamento pode não fazer parte fisicamente do computador que executa o Windows Server 2008.  <br/> |
|Ferramentas e idiomas  <br/> |Você pode usar qualquer linguagem compatível com o COM para usar VSS. É usado com mais frequência em aplicativos escritos em C++. Como você precisa colocar o armazenamento offline do Exchange para criar cópias de sombra, os aplicativos de backup são normalmente sensíveis ao tempo, o que na maioria dos casos torna o uso de linguagens como Visual Basic ou VBScript impraticável.  <br/> |
|Implementação gerenciada  <br/> |Você pode usar as APIs VSS em um ambiente de código gerenciado por meio de um assembly de interoperabilidade COM.  <br/> |
|Programável  <br/> |Sim, mas não recomendado.  <br/> |
|Ferramentas de teste e depuração disponíveis  <br/> |Nenhuma ferramenta especial é necessária para depurar aplicativos que usam o Windows VSS.  <br/> |
   
## <a name="in-this-section"></a>Nesta seção

- [Conceitos de backup e restauração para o Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Criar aplicativos de backup e restauração para o Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Referência de classe função cchksgfiles](cchksgfiles-class-reference.md)
    
## <a name="see-also"></a>Confira também

- [Serviço de cópias de sombra de volume (Windows)](https://msdn.microsoft.com/library/windows/desktop/bb968832%28v=vs.85%29.aspx)   
- [Explorar os recursos da API gerenciada por EWS, EWS e serviços Web no Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [Exchange Management Shell](../management/exchange-management-shell.md)   
- [Agentes de transporte no Exchange](../transport-agents/transport-agents-in-exchange-2013.md) 
    

