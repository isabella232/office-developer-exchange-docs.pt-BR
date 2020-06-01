---
title: Shell de Gerenciamento do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8cc0c4fa-9e13-45cb-88da-0486f2ac1bd0
description: Encontre informações sobre como usar o Shell de gerenciamento do Exchange para desenvolver ferramentas para administração do Exchange Server.
ms.openlocfilehash: 38e75339a4ad97cf8ff99e1cbe9c01059e157941
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44435804"
---
# <a name="exchange-management-shell"></a>Shell de Gerenciamento do Exchange

Encontre informações sobre como usar o Shell de gerenciamento do Exchange para desenvolver ferramentas para administração do Exchange Server.
  
**Aplica-se a:** Exchange Online | Exchange Server 2013 | Office 365
  
O Shell de gerenciamento do Exchange fornece um conjunto avançado de comandos, com base na plataforma Windows PowerShell, para gerenciar o Exchange Online, o Exchange Online como parte do Office 365 ou uma versão local do Exchange a partir do Exchange 2013. Você pode usar o Shell de gerenciamento do Exchange para criar dois tipos de ferramentas: scripts de linha de comando que funcionam dentro do ambiente do Windows PowerShell e ferramentas que usam os cmdlets do Shell de gerenciamento do Exchange por meio de uma interface gerenciada. Você pode usar aplicativos gerenciados para criar uma interface do usuário do Windows ou baseada na Web padrão para administrar um servidor Exchange. 
  
## <a name="what-you-need-to-know-about-the-exchange-management-shell"></a>O que você precisa saber sobre o Shell de gerenciamento do Exchange

|Se você estiver se perguntando|Leia isto|
|:-----|:-----|
|Disponibilidade  <br/> |Os comandos do Shell de gerenciamento do Exchange são instalados em todos os servidores que executam versões do Exchange a partir do Exchange 2007.<br/>Os aplicativos cliente podem ser implantados em qualquer computador executando o Windows PowerShell 2,0.<br/> Para obter informações sobre como acessar o Shell, consulte [Exchange Server PowerShell (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).  <br/> |
|Ferramentas e idiomas  <br/> |Você pode criar scripts do Shell de gerenciamento do Exchange em qualquer editor de texto.<br/>Você pode usar uma das várias ferramentas de terceiros para a criação de scripts do Windows PowerShell que podem ser usadas com o Shell de gerenciamento do Exchange.  <br/> O [modelo de objeto do Shell de gerenciamento do Exchange](exchange-management-shell-namespaces.md) baseia-se no .NET Framework.<br/>Você pode usar qualquer linguagem .NET para desenvolver aplicativos do Shell de gerenciamento do Exchange.  <br/> |
|Ferramentas de teste e depuração disponíveis  <br/> |Você pode usar um dos vários aplicativos de terceiros para testar e depurar scripts do Shell de gerenciamento do Exchange.  <br/> Você pode usar o Visual Studio e ferramentas de terceiros para testar e depurar aplicativos do Shell de gerenciamento do Exchange gerenciados.  <br/> |
|Requisitos da plataforma do servidor  <br/> |Você pode usar o Shell de gerenciamento do Exchange em qualquer servidor Exchange que tenha o Windows PowerShell 2,0 instalado.  <br/> |
|Requisitos da plataforma do cliente  <br/> |Os aplicativos cliente do Shell de gerenciamento do Exchange exigem o Windows PowerShell 2,0.  <br/> |
|Permissions  <br/> |A execução de um aplicativo de Shell de gerenciamento do Exchange exige que o usuário tenha direitos de controle de acesso baseado em função para os dados afetados no repositório do Exchange.<br/>Para obter mais informações sobre o controle de acesso baseado em função, consulte [Understanding Role Based Access Control](https://technet.microsoft.com/library/dd298183.aspx).  <br/> |
   
Os artigos desta seção descrevem os recursos do Shell de gerenciamento do Exchange que são importantes para a criação de ferramentas de gerenciamento do Exchange. Para obter informações sobre planejamento, configuração ou manutenção do Exchange, consulte o site do [Exchange](https://docs.microsoft.com/exchange/) .
  
## <a name="in-this-section"></a>Nesta seção

- [Criar ferramentas do Shell de gerenciamento do Exchange](create-exchange-management-shell-tools.md)
    
- [Namespaces do Shell de gerenciamento do Exchange](exchange-management-shell-namespaces.md)
    
## <a name="see-also"></a>Também consulte
  
- [Documentação do Windows PowerShell](https://docs.microsoft.com/powershell/scripting/getting-started/getting-started-with-windows-powershell?view=powershell-6)
- [Script do PowerShell](https://docs.microsoft.com/powershell/scripting/powershell-scripting?view=powershell-6)
    

