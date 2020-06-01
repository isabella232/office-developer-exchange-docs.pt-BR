---
title: Criar aplicativos de backup e restauração para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e5e952a5-add1-417c-a3c2-230f4dc99b00
description: Encontre informações sobre os componentes e arquitetura de aplicativos de backup e restauração para o Exchange 2013 e os requisitos do sistema para a criação de um aplicativo de backup e restauração.
ms.openlocfilehash: f8a332d0816792f8888c97a8394886b026f5204b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455266"
---
# <a name="build-backup-and-restore-applications-for-exchange-2013"></a>Criar aplicativos de backup e restauração para o Exchange 2013

Encontre informações sobre os componentes e arquitetura de aplicativos de backup e restauração para o Exchange 2013 e os requisitos do sistema para a criação de um aplicativo de backup e restauração.
  
**Aplica-se a:** Exchange Server 2013 
  
Você pode usar o [serviço de cópias de sombra de volume (VSS)](https://msdn.microsoft.com/library/bb968832%28VS.85%29.aspx) em versões do Windows Server começando com o windows Server 2008 para criar aplicativos que façam backup e restauração de dados do Exchange Server 2013. O VSS fornece uma infraestrutura que permite que você crie e gerencie cópias de sombra em sistemas de gerenciamento de armazenamento, aplicativos de negócios e hardware de terceiros. Você pode criar soluções baseadas na infraestrutura VSS que usam cópias de sombra para fazer backup e restaurar um ou mais bancos de dados do Exchange 2013. 
  
## <a name="backup-and-restore-application-prerequisites"></a>Pré-requisitos de backup e restauração do aplicativo
<a name="bk_systemrequirements"> </a>

Para seu aplicativo de backup e restauração personalizado e o VSS para fazer backup e restaurar os bancos de dados do Exchange 2013, seu ambiente deve incluir o seguinte:
  
- Uma versão do Windows Server começando com o Windows Server 2008 
    
- Exchange 2013
    
Além disso, se você estiver criando um aplicativo de backup e restauração, você deve estar ciente das seguintes restrições no ambiente de desenvolvimento:
  
- VSS é uma API COM não gerenciada que pode ser acessada a partir do código gerenciado do .NET Framework por meio de um assembly de interoperabilidade COM.
    
- O Shell de gerenciamento do Exchange é um aplicativo gerenciado que é acessado por meio do código gerenciado do .NET Framework.
    
- A API CHKSGFILES fornecida com o Exchange 2013 é uma DLL de código nativo de 64 bits. O uso da DLL de CHKSGFILES de bits do Exchange 2007 32 com bancos de dados do Exchange 2013 não é suportado.
    
## <a name="backup-and-restore-application-overview"></a>Visão geral do aplicativo de backup e restauração
<a name="bk_components"> </a>

O VSS coordena a comunicação entre os seguintes componentes: 
  
- O solicitante VSS, que é seu aplicativo de backup
    
- O gravador VSS
    
- O VSS Provider, que é o sistema, software ou componentes de hardware que criam cópias de sombra
    
Para usar o VSS para fazer o backup dos dados do Exchange 2013, seu aplicativo de backup deve ser um solicitador de VSS com reconhecimento de 2013 do Exchange. O Exchange 2013 inclui um gravador VSS, chamado Microsoft Exchange Writer, para o programa de backup do Windows Server; no entanto, o gravador do Exchange apenas faz o backup de volumes inteiros. Não faz backup de bancos de dados individuais do Exchange 2013. Se você precisar de mais flexibilidade, pode usar um aplicativo de backup de terceiros que tenha um gravador VSS com reconhecimento do Exchange que possa funcionar com bancos de dados individuais do Exchange ou pode criar um solicitante VSS personalizado.
  
Antes que o aplicativo chame o VSS para iniciar um backup, ele deve obter informações sobre a configuração de armazenamento para o sistema do Exchange 2013 em que está fazendo o backup. Essas informações são armazenadas nos serviços de domínio do Active Directory (AD DS). O aplicativo de backup pode obter dados de configuração de armazenamento do Exchange usando os comandos do Shell de gerenciamento do Exchange. Para obter mais informações, consulte [Exchange Server PowerShell (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps). 
  
Os aplicativos de backup do Exchange 2013 chamam as APIs COM VSS para criar backups completos, de cópia, diferencial e incremental dos bancos de dados do Exchange; Eles não interagem diretamente com o gravador VSS. A funcionalidade do DAG (grupo de disponibilidade de banco de dados) no Exchange também permite que o aplicativo crie um backup totalmente consistente, mesmo que o backup completo inicial e os backups incrementais mais recentes sejam provenientes de servidores diferentes no DAG. Depois que o VSS cria a cópia dos dados do Exchange, o aplicativo de backup armazena os dados na mídia pretendida.
  
Para restaurar um banco de dados do Exchange 2013, o aplicativo de restauração recupera o banco de dados e os arquivos de log da mídia de backup e os armazena no armazenamento em disco ativo de um servidor Exchange. Bancos de dados individuais não são associados a um servidor Exchange específico. 
  
Os aplicativos de backup e restauração devem especificar vários parâmetros específicos do Exchange 2013 para controlar e gerenciar corretamente as operações executadas pelo VSS em bancos de dados do Exchange 2013. Por exemplo, como o Exchange 2013 suporta até 100 bancos de dados ativos simultaneamente, o aplicativo de backup deve especificar corretamente e processar o arquivo de banco de dados, os arquivos de log de transações e os componentes de banco de dados de arquivos de ponto de verificação.
  
Para reconstruir um banco de dados que tinha alterações desde o último backup completo, o aplicativo de restauração requer bancos de dados e arquivos de log de diferentes backups. Por exemplo, pode exigir um backup completo semanal e um ou mais backups incrementais diários. Nos sistemas Exchange 2013 que usam o DAGs, o aplicativo de restauração pode recriar um banco de dados usando backups de diferentes cópias de banco de dados em diferentes servidores no mesmo DAG. No entanto, a única maneira compatível de restaurar um banco de dados do DAG do backup é restaurar todas as cópias ativas e passivas do banco de dados usando os mesmos dados.
  
Depois que todos os dados estiverem no local, o aplicativo de restauração sinalizará o Exchange para verificar a integridade dos arquivos de banco de dados e de log. Se o banco de dados e os arquivos de log tiverem sido restaurados corretamente, o servidor do Exchange poderá repetir os arquivos de log do banco de dados para atualizar o banco de dados e montá-lo. Se o banco de dados tiver sido recuperado para um servidor que já tenha uma cópia ativa do banco de dados montado, o banco de dados será tratado como um banco de dados de recuperação. Se o banco de dados tiver sido recuperado em um servidor diferente, o banco de dados pode ser montado independentemente, ou essa réplica pode ser adicionada ao DAG.
  
## <a name="backup-and-restore-system-architecture"></a>Arquitetura do sistema de backup e restauração
<a name="bk_ExchangeVSS"> </a>

O VSS se comunica com o sistema de arquivos do Windows Server e com o driver de dispositivo de armazenamento em massa por meio de um provedor de terceiros (ou personalizado). O provedor de hardware determina onde a cópia de sombra será criada. O VSS abstrai a cópia de sombra específica de hardware para que seu aplicativo de backup e restauração possa acessar a cópia de sombra sem informações sobre os detalhes de implementação de hardware. A figura a seguir mostra como o aplicativo de backup e restauração interage com o Exchange 2013 e o Windows Server.
  
**Figura 1. Arquitetura do sistema de backup e restauração**

![A diagram that shows how a backup and restore application interacts. Two way communication exists between Exchange, Windows Server, and the client application. The Windows server also interacts with a mass storage device or backup media.](media/VSS_architecture_E2k7.gif)
  
O aplicativo de backup e restauração funciona como o solicitante VSS. O solicitante se comunica com o VSS para obter informações sobre o Exchange 2013, para iniciar a criação de cópias de sombra e para obter acesso aos dados do backup. 
  
O repositório do Exchange é um componente do Exchange 2013 e acessa os bancos de dados do Exchange 2013 por meio do sistema de arquivos do Windows Server. No sistema de arquivos, cada servidor do Exchange pode montar simultaneamente até 100 bancos de dados com os arquivos de banco de dados (. edb) que o acompanham, os arquivos de log de transações e um arquivo de ponto de verificação.
  
Para oferecer suporte ao VSS, o Exchange 2013 inclui um gravador do Exchange que é integrado ao repositório do Exchange. O gravador do Exchange coordena com o repositório do Exchange (operando em nome do solicitante) para congelar e desmontar o banco de dados antes de fazer o backup e depois descongelar e montar o banco de dados após a conclusão do backup. Durante uma restauração, o aplicativo de backup e restauração instrui o gravador do Exchange a coordenar com o repositório do Exchange para desmontar o banco de dados, substituir os arquivos de banco de dados, montar o banco de dados e repetir os logs de transação (conforme necessário).
  
Durante uma restauração, o solicitante também se comunica com o VSS para preparar o sistema para a restauração e, em seguida, colocá-los novamente no dispositivo de armazenamento em massa. O aplicativo de backup e restauração também é responsável por trabalhar com o Windows Server para ler e gravar dados na mídia de armazenamento de backup, seja um arquivo morto em fita, uma rede de área de armazenamento ou outra mídia de backup.
  
O banco de dados restaurado pode ser montado como um banco de dados ativo normal ou como o banco de dados de recuperação do Exchange 2013. Apenas um banco de dados montado pode ser designado como um banco de dados de recuperação em cada servidor Exchange.
  
As informações necessárias para concluir com êxito as operações de backup e restauração entre o Exchange 2013, VSS e o aplicativo de backup e restauração são transferidas como parte dos metadados do gravador do Exchange.
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Tipos de operações de backup para o Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
    
- [Restauração de bancos de dados do Exchange 2013](restoring-exchange-2013-databases.md)
    
- [Validar a integridade do backup usando a API CHKSGFILES no Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
    
- [Validar a integridade do backup usando a ferramenta Eseutil no Exchange 2013](how-to-validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013.md)
    
## <a name="see-also"></a>Também consulte

- [Backup e restauração para o Exchange](backup-and-restore-for-exchange-2013.md) 
- [Referência de classe função cchksgfiles](cchksgfiles-class-reference.md) 
- [Serviço de cópias de sombra de volume](https://msdn.microsoft.com/library/bb968832%28VS.85%29.aspx) 
- [Windows PowerShell](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

