---
title: Criar aplicativos de backup e restauração para Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e5e952a5-add1-417c-a3c2-230f4dc99b00
description: Encontre informações sobre os componentes e a arquitetura dos aplicativos de backup e restauração para Exchange 2013 e os requisitos do sistema para criar um aplicativo de backup e restauração.
ms.openlocfilehash: 590ac029e157196d370cbcbe54e5df75bc1a830b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513875"
---
# <a name="build-backup-and-restore-applications-for-exchange-2013"></a>Criar aplicativos de backup e restauração para Exchange 2013

Encontre informações sobre os componentes e a arquitetura dos aplicativos de backup e restauração para Exchange 2013 e os requisitos do sistema para criar um aplicativo de backup e restauração.
  
**Aplica-se a:** Exchange Server 2013 
  
Você pode usar o Serviço de Cópia de Sombra de [Volume (VSS)](https://msdn.microsoft.com/library/bb968832%28VS.85%29.aspx) em versões do Windows Server a partir do Windows Server 2008 para criar aplicativos que backup e restauração Exchange Server dados 2013. O VSS fornece uma infraestrutura que permite que você crie e gerencie cópias de sombra em sistemas de gerenciamento de armazenamento de terceiros, aplicativos comerciais e hardware. Você pode criar soluções com base na infraestrutura VSS que use cópias de sombra para fazer backup e restaurar um ou mais bancos de dados Exchange 2013. 
  
## <a name="backup-and-restore-application-prerequisites"></a>Pré-requisitos de backup e restauração de aplicativos
<a name="bk_systemrequirements"> </a>

Para que seu aplicativo de backup e restauração personalizado e VSS faça backup e restauração de bancos de dados Exchange 2013, seu ambiente deve incluir o seguinte:
  
- Uma versão do Windows Server começando com Windows Server 2008 
    
- Exchange 2013
    
Além disso, se você estiver criando um aplicativo de backup e restauração, deve estar ciente das seguintes restrições no ambiente de desenvolvimento:
  
- VSS é uma API COM não gerenciada que pode ser acessada .NET Framework código gerenciado por meio de um Assembly de Interop COM.
    
- O Exchange Shell de Gerenciamento é um aplicativo gerenciado que é acessado por meio .NET Framework código gerenciado.
    
- A API CHKSGFILES fornecida com o Exchange 2013 é uma DLL de 64 bits de código nativo. Não há suporte Exchange DLL do CHKSGFILES 2007 2007 com bancos de dados Exchange 2013.
    
## <a name="backup-and-restore-application-overview"></a>Visão geral do aplicativo de backup e restauração
<a name="bk_components"> </a>

O VSS coordena a comunicação entre os seguintes componentes: 
  
- O solicitante VSS, que é seu aplicativo de backup
    
- O escritor VSS
    
- O provedor VSS, que é o sistema, software ou componentes de hardware que criam as cópias de sombra
    
Para usar o VSS para fazer backup Exchange dados 2013, seu aplicativo de backup deve ser um solicitador VSS Exchange 2013 com conhecimento em 2013. Exchange 2013 inclui um escritor VSS, chamado de Escritor do Microsoft Exchange, para o programa de backup do Windows Server; no entanto, Exchange o autor de Exchange apenas fazer o back up de volumes inteiros. Ele não faz o back up individual Exchange 2013 databases. Se você precisar de mais flexibilidade, poderá usar um aplicativo de backup de terceiros que tenha um Exchange VSS que possa trabalhar com bancos de dados Exchange individuais ou pode criar um solicitante VSS personalizado.
  
Antes de seu aplicativo chamar o VSS para iniciar um backup, ele deve obter informações sobre a configuração de armazenamento para o sistema Exchange 2013 que ele está com backup. Essas informações são armazenadas nos Serviços de Domínio do Active Directory (AD DS). Seu aplicativo de backup pode obter Exchange de configuração de armazenamento usando Exchange comandos do Shell de Gerenciamento. Para obter mais informações, [consulte Exchange Server PowerShell (Exchange Shell](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)de Gerenciamento) . 
  
Exchange aplicativos de backup 2013 chamam as APIs COM VSS para criar backups completos, de cópia, diferenciais e incrementais de bancos de dados Exchange; eles não interagem diretamente com o escritor VSS. A funcionalidade do Grupo de Disponibilidade de Banco de Dados (DAG) no Exchange também permite que seu aplicativo crie um backup totalmente consistente, mesmo que o backup completo inicial e posteriores backups incrementais venham de servidores diferentes no DAG. Depois que o VSS cria a cópia dos dados Exchange, seu aplicativo de backup armazena os dados na mídia pretendido.
  
Para restaurar um banco de dados Exchange 2013, o aplicativo de restauração recupera o banco de dados e os arquivos de log da mídia de backup e os armazena no armazenamento em disco ativo de um servidor Exchange. Bancos de dados individuais não estão associados a um servidor Exchange específico. 
  
Os aplicativos de backup e restauração devem especificar um número de parâmetros específicos Exchange 2013 para controlar e gerenciar corretamente as operações executados pelo VSS em relação aos bancos de dados Exchange 2013. Por exemplo, como o Exchange 2013 oferece suporte a até 100 bancos de dados simultaneamente ativos, o aplicativo de backup deve especificar e processar corretamente o arquivo de banco de dados, os arquivos de log de transações e os componentes do banco de dados de arquivo de ponto de verificação.
  
Para reconstruir um banco de dados que teve alterações desde o último back completo, seu aplicativo de restauração requer arquivos de banco de dados e log de backups diferentes. Por exemplo, pode exigir um backup completo semanal e um ou mais backups incrementais diários. No Exchange 2013 que usam DAGs, seu aplicativo de restauração pode recriar um banco de dados usando backups de diferentes cópias de banco de dados em servidores diferentes no mesmo DAG. No entanto, a única maneira com suporte para restaurar um banco de dados do DAG a partir do backup é restaurar todas as cópias ativas e passivas do banco de dados usando os mesmos dados.
  
Depois que todos os dados estão no local, seu aplicativo de restauração sinaliza Exchange verificar a integridade do banco de dados e arquivos de log. Se os arquivos de banco de dados e de log foram restaurados corretamente, o servidor Exchange pode então repetir os arquivos de log do banco de dados para colocar o banco de dados atualizado e montá-lo. Se o banco de dados tiver sido recuperado para um servidor que já tenha uma cópia ativa do banco de dados montado, o banco de dados será tratado como um banco de dados de recuperação. Se o banco de dados tiver sido recuperado em um servidor diferente, o banco de dados poderá ser montado independentemente ou essa réplica poderá ser adicionada ao DAG.
  
## <a name="backup-and-restore-system-architecture"></a>Arquitetura do sistema de backup e restauração
<a name="bk_ExchangeVSS"> </a>

O VSS se comunica com o sistema de arquivos Windows Server e com o driver de dispositivo de armazenamento em massa por meio de um provedor (ou personalizado) de terceiros. O provedor de hardware determina onde a cópia de sombra será criada. O VSS abstrai a cópia de sombra específica de hardware para que seu aplicativo de backup e restauração possa acessar a cópia de sombra sem informações sobre os detalhes da implementação de hardware. A figura a seguir mostra como seu aplicativo de backup e restauração interage com Exchange 2013 e Windows Server.
  
**Figura 1. Arquitetura do sistema de backup e restauração**

![A diagram that shows how a backup and restore application interacts. Two way communication exists between Exchange, Windows Server, and the client application. The Windows server also interacts with a mass storage device or backup media.](media/VSS_architecture_E2k7.gif)
  
O aplicativo de backup e restauração funciona como o solicitante VSS. O solicitante se comunica com o VSS para obter informações sobre o Exchange 2013, para iniciar a criação de cópias de sombra e para obter acesso aos dados para backup. 
  
O Exchange store é um componente do Exchange 2013 e acessa Exchange bancos de dados 2013 por meio do sistema de arquivos Windows Server. Dentro do sistema de arquivos, cada Exchange servidor pode montar simultaneamente até 100 bancos de dados com seus arquivos de banco de dados (.edb) de acompanhamento, arquivos de log de transações e um arquivo de ponto de verificação.
  
Para dar suporte ao VSS, Exchange 2013 inclui um Exchange que é integrado ao Exchange store. O Exchange do Exchange coordena com o armazenamento Exchange (operando em nome do solicitante) para congelar e desmontar o banco de dados antes de fazer o backup e, em seguida, descongelar e montar o banco de dados depois que o backup for concluído. Durante uma restauração, seu aplicativo de backup e restauração instrui o Exchange a coordenar com o armazenamento Exchange para desmontar o banco de dados, substituir os arquivos de banco de dados, montar o banco de dados e, em seguida, repetir os logs de transação (conforme necessário).
  
Durante uma restauração, o solicitante também se comunica com o VSS para preparar o sistema para a restauração e, em seguida, colocar os dados de volta no dispositivo de armazenamento em massa. Seu aplicativo de backup e restauração também é responsável por trabalhar com o Windows Server para ler dados e gravar dados na mídia de armazenamento de backup, seja um arquivo morto em fita, uma rede de área de armazenamento ou outro meio de backup.
  
O banco de dados restaurado pode ser montado como um banco de dados regular e ativo ou como o banco de dados de recuperação Exchange 2013. Somente um banco de dados montado pode ser designado como um banco de dados de recuperação em cada Exchange servidor.
  
As informações necessárias para concluir com êxito operações de backup e restauração entre o Exchange 2013, VSS e seu aplicativo de backup e restauração são transferidas como parte dos metadados do Exchange de escritor.
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Tipos de operações de backup para Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
    
- [Restaurando Exchange bancos de dados 2013](restoring-exchange-2013-databases.md)
    
- [Validar a integridade do backup usando a API CHKSGFILES no Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
    
- [Validar a integridade do backup usando a ferramenta Eseutil no Exchange 2013](how-to-validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013.md)
    
## <a name="see-also"></a>Confira também

- [Backup e restauração para o Exchange](backup-and-restore-for-exchange-2013.md) 
- [Referência da classe CChkSGFiles](cchksgfiles-class-reference.md) 
- [Serviço de cópias de sombra de volume](https://msdn.microsoft.com/library/bb968832%28VS.85%29.aspx) 
- [Windows PowerShell](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

