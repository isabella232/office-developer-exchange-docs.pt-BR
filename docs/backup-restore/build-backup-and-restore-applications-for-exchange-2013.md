---
title: Criar um backup e restaurar aplicativos para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e5e952a5-add1-417c-a3c2-230f4dc99b00
description: Encontre informações sobre os componentes e arquitetura dos aplicativos de backup e restauração para o Exchange 2013 e os requisitos do sistema para criar um backup e restaurar o aplicativo.
ms.openlocfilehash: e85a5364c40c472c9e1ea9d1d3b4e89329b1676f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750638"
---
# <a name="build-backup-and-restore-applications-for-exchange-2013"></a>Criar um backup e restaurar aplicativos para o Exchange 2013

Encontre informações sobre os componentes e arquitetura dos aplicativos de backup e restauração para o Exchange 2013 e os requisitos do sistema para criar um backup e restaurar o aplicativo.
  
**Aplica-se a:** Exchange Server 2013 
  
Você pode usar o [Serviço de cópia de sombra de Volume (VSS)](http://msdn.microsoft.com/en-us/library/bb968832%28VS.85%29.aspx) nas versões do Windows Server, começando com o Windows Server 2008 para criar aplicativos que fazer backup e restaurar dados do Exchange Server 2013. VSS oferece uma infra-estrutura que lhe permite criar e gerenciar cópias de sombra entre sistemas de gerenciamento de armazenamento de terceiros, aplicativos de negócios e hardware. Você pode criar soluções baseadas na infraestrutura VSS e que usam cópias de sombra para fazer backup e restaurar um ou mais bancos de dados do Exchange 2013. 
  
## <a name="backup-and-restore-application-prerequisites"></a>Pré-requisitos de aplicativo de backup e restauração
<a name="bk_systemrequirements"> </a>

Na ordem para o seu backup personalizado e o aplicativo de restauração e o VSS para fazer backup e restaurar bancos de dados do Exchange 2013, seu ambiente deve incluir o seguinte:
  
- Uma versão do Windows Server, começando com o Windows Server 2008 
    
- Exchange 2013
    
Além disso, se você estiver criando um backup e restaurar o aplicativo, você deve ser ciente das seguintes restrições no ambiente de desenvolvimento:
  
- VSS é uma API COM não gerenciado que pode ser acessado a partir de código gerenciado do .NET Framework via um Assembly de interoperabilidade COM.
    
- O Shell de gerenciamento do Exchange é um aplicativo gerenciado que é acessado por meio de código gerenciado do .NET Framework.
    
- A API CHKSGFILES fornecido com o Exchange 2013 é uma DLL de 64 bits de código nativo. Não há suporte para o uso do Exchange 2007 32 bits CHKSGFILES DLL com bancos de dados do Exchange 2013.
    
## <a name="backup-and-restore-application-overview"></a>Visão geral dos aplicativos de backup e restauração
<a name="bk_components"> </a>

VSS coordena a comunicação entre os seguintes componentes: 
  
- O solicitante VSS, que é o seu aplicativo de backup
    
- O gravador VSS
    
- O provedor de VSS, os componentes do sistema, software ou hardware que criar cópias de sombra
    
Para usar o VSS para fazer backup de dados do Exchange 2013, o seu aplicativo de backup deve ser um solicitante VSS sensível ao Exchange 2013. Exchange 2013 inclui um gravador VSS, chamado o gravador do Microsoft Exchange, para o programa de backup do Windows Server. No entanto, o gravador do Exchange só faz o backup de todo volumes. Ele não faz backup individual do Exchange 2013 bancos de dados. Se precisar de mais flexibilidade, você pode usar um aplicativo de backup de terceiros que tenha um gravador VSS sensível ao Exchange que pode trabalhar com bancos de dados individuais do Exchange, ou você pode criar um solicitante VSS personalizado.
  
Antes de seu aplicativo chama VSS para iniciar o backup, ela deve obter informações sobre a configuração de armazenamento para o sistema do Exchange 2013 que está aumentando. Que informações são armazenadas nos serviços de domínio Active Directory (AD DS). Os aplicativos de backup podem obter dados de configuração de armazenamento do Exchange usando comandos do Shell de gerenciamento do Exchange. Para obter mais informações, consulte [Exchange Server PowerShell (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps). 
  
Aplicativos de backup do Exchange 2013 chamam as APIs de COM do VSS para criar completo, cópia, diferenciais e incrementais backups dos bancos de dados do Exchange; eles não interagir diretamente com o gravador VSS. A funcionalidade de grupo de disponibilidade de banco de dados (DAG) do Exchange também permite que seu aplicativo para criar um backup totalmente consistente, mesmo se o backup completo inicial e posterior backups incrementais vêm de servidores diferentes no DAG. Depois que o VSS cria a cópia dos dados do Exchange, seu aplicativo de backup armazena os dados em uma mídia o pretendido.
  
Para restaurar um banco de dados do Exchange 2013, seu aplicativo de restauração recupera os arquivos de log e de banco de dados da mídia de backup e armazenando-as no armazenamento de disco ativo de um servidor Exchange. Bancos de dados individuais não estão associados um determinado servidor Exchange. 
  
Aplicativos de backup e restauração devem especificar um número de parâmetros específicos do Exchange 2013 corretamente, controlar e gerenciar as operações executadas por VSS em relação a bancos de dados do Exchange 2013. Por exemplo, como Exchange 2013 oferece suporte a até 100 bancos de dados de ativos ao mesmo tempo, o aplicativo de backup corretamente deve especificar e processar o arquivo de banco de dados, arquivos de log de transação e componentes de banco de dados do arquivo de ponto de verificação.
  
Para reconstruir um banco de dados que tiveram alterações desde o último back completo, seu aplicativo de restauração requer os arquivos de log e de banco de dados de backups diferentes. Por exemplo, ele pode exigir um backup completo semanal e um ou mais backups incrementais diários. No Exchange 2013 sistemas que usam DAGs, seu aplicativo de restauração pode recriar um banco de dados usando backups de cópias de banco de dados diferente em servidores diferentes no mesmo DAG. No entanto, é a única maneira com suporte para restaurar um banco de dados do DAG de backup restaurar todas as cópias ativas e passivas do banco de dados usando os mesmos dados.
  
Após todos os dados no lugar, o seu aplicativo de restauração sinaliza Exchange para verificar a integridade dos arquivos de log e de banco de dados. Se os arquivos de log e de banco de dados tiverem sido restaurados corretamente, o servidor do Exchange pode então repetição durante os arquivos de log do banco de dados para colocar o banco de dados atualizado e montá-lo. Se o banco de dados foi recuperado para um servidor que já tenha uma cópia ativa do banco de dados montado, o banco de dados é tratado como um banco de dados de recuperação. Se o banco de dados foi recuperado em um servidor diferente, o banco de dados pode ser independentemente montado ou que a réplica pode então ser adicionada ao DAG.
  
## <a name="backup-and-restore-system-architecture"></a>Arquitetura do sistema de backup e restauração
<a name="bk_ExchangeVSS"> </a>

VSS se comunica com o sistema de arquivos do Windows Server e com o driver do dispositivo de armazenamento em massa através de um provedor de terceiros (ou personalizado). O provedor de hardware determina onde a cópia de sombra será criada. VSS abstrai a cópia de sombra de hardware específicos, para que seu aplicativo de backup e restauração possa acessar a cópia de sombra sem informações sobre os detalhes da implementação de hardware. A figura a seguir mostra como o seu aplicativo de backup e restauração interage com o Exchange 2013 e no Windows Server.
  
**Figura 1. Arquitetura do sistema de backup e restauração**

![A diagram that shows how a backup and restore application interacts. Two way communication exists between Exchange, Windows Server, and the client application. The Windows server also interacts with a mass storage device or backup media.](media/VSS_architecture_E2k7.gif)
  
O aplicativo de backup e restauração funciona como o solicitante VSS. O solicitante se comunica com VSS para obter informações sobre o Exchange 2013, para iniciar a criação de cópias de sombra e para obter acesso aos dados de backup. 
  
O armazenamento do Exchange é um componente do Exchange 2013 e acessa os bancos de dados do Exchange 2013 através do sistema de arquivo do Windows Server. Dentro do sistema de arquivo, cada servidor Exchange pode montar simultaneamente até 100 bancos de dados com um arquivo de ponto de verificação, arquivos de log de transação e seus arquivos de banco de dados (. edb) acompanha.
  
Para suportar VSS, o Exchange 2013 inclui um gravador do Exchange é feito no armazenamento do Exchange. O gravador do Exchange coordena com o repositório do Exchange (operacional em nome do solicitante) congelada e desmontar o banco de dados antes de fazer o backup e, em seguida descongelar e monte o banco de dados após o backup for concluído. Durante uma recuperação, o seu aplicativo de backup e restauração instrui o gravador do Exchange para coordenar com o repositório do Exchange para desmontar o banco de dados, substituir os arquivos de banco de dados, monte o banco de dados e, em seguida, repetição durante os logs de transações (conforme necessário).
  
Durante uma recuperação, o solicitante também se comunica com o VSS para preparar o sistema para restaurar e, em seguida, para colocar os dados de volta para o dispositivo de armazenamento em massa. Seu aplicativo de backup e restauração também é responsável para trabalhar com o Windows Server dados a partir de ler e gravar dados em mídia de armazenamento de backup, se uma fita arquivar, uma rede de área de armazenamento ou outra mídia de backup.
  
O banco de dados restaurado pode ser montado como um banco de dados ativo regular, ou como o banco de dados de recuperação do Exchange 2013. Apenas um banco de dados montado pode ser designado como um banco de dados de recuperação em cada servidor do Exchange.
  
Informações necessárias para concluir o backup e restaurar as operações entre o Exchange 2013, VSS, com êxito e seu aplicativo de backup e restauração será transferido como parte dos metadados do gravador do Exchange.
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Tipos de operações de backup para o Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
    
- [Restaurando bancos de dados do Exchange 2013](restoring-exchange-2013-databases.md)
    
- [Validar a integridade do backup, usando a API CHKSGFILES no Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
    
- [Validar a integridade do backup, usando a ferramenta Eseutil no Exchange 2013](how-to-validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013.md)
    
## <a name="see-also"></a>Confira também

- [Backup e restauração para o Exchange](backup-and-restore-for-exchange-2013.md) 
- [Referência de classe CChkSGFiles](cchksgfiles-class-reference.md) 
- [Serviço de cópias de sombra de volume](http://msdn.microsoft.com/en-us/library/bb968832%28VS.85%29.aspx) 
- [O Windows PowerShell](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

