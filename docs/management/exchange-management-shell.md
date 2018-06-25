---
title: Shell de Gerenciamento do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8cc0c4fa-9e13-45cb-88da-0486f2ac1bd0
description: Encontre informações sobre como usar o Shell de gerenciamento do Exchange para desenvolver ferramentas de administração do Exchange server.
ms.openlocfilehash: 1cb0328bdb0eebda0ce4eda929e1bfb21be451f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750964"
---
# <a name="exchange-management-shell"></a>Shell de Gerenciamento do Exchange

Encontre informações sobre como usar o Shell de gerenciamento do Exchange para desenvolver ferramentas de administração do Exchange server.
  
**Aplica-se a:** Exchange Online | Exchange Server 2013 | Office 365
  
O Shell de gerenciamento do Exchange fornece um conjunto rico de comandos, com base na plataforma do Windows PowerShell para gerenciar o Exchange Online, Exchange Online como parte do Office 365 ou uma versão local do Exchange, começando com o Exchange 2013. Você pode usar o Shell de gerenciamento do Exchange para criar dois tipos de ferramentas: scripts de linha de comando que funcionam dentro do ambiente do Windows PowerShell e ferramentas que usam os cmdlets do Shell de gerenciamento do Exchange por meio de uma interface gerenciada. Você pode usar aplicativos gerenciados para criar um padrão do Windows ou a interface do usuário baseado na web para administrar um servidor Exchange. 
  
## <a name="what-you-need-to-know-about-the-exchange-management-shell"></a>O que você precisa saber sobre o Shell de gerenciamento do Exchange

|Se você está se perguntando sobre|Leia isto|
|:-----|:-----|
|Availability  <br/> |Comandos do Shell de gerenciamento do Exchange são instalados em todos os servidores que executam versões do Exchange, começando com o Exchange 2007.<br/>Aplicativos do cliente podem ser implantados em qualquer computador executando o Windows PowerShell 2.0.<br/> Para obter informações sobre como acessar o shell, consulte [Exchange Server PowerShell (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).  <br/> |
|Languages and tools  <br/> |Você pode criar scripts do Shell de gerenciamento do Exchange em qualquer editor de texto.<br/>Você pode usar uma das muitas ferramentas de terceiros para a criação de scripts do Windows PowerShell que podem ser usados com o Shell de gerenciamento do Exchange.  <br/> O [modelo de objeto do Shell de gerenciamento do Exchange](exchange-management-shell-namespaces.md) é baseado no .NET Framework.<br/>Você pode usar qualquer linguagem .NET para desenvolver aplicativos do Shell de gerenciamento do Exchange.  <br/> |
|Ferramentas de teste e depuração disponíveis  <br/> |Você pode usar um dos muitos aplicativos de terceiros para testar e depurar scripts do Shell de gerenciamento do Exchange.  <br/> Você pode usar o Visual Studio e gerenciados de ferramentas de terceiros para testar e depurar aplicativos do Shell de gerenciamento do Exchange.  <br/> |
|Server platform requirements  <br/> |Você pode usar o Shell de gerenciamento do Exchange em qualquer servidor do Exchange com o Windows PowerShell 2.0 instalado.  <br/> |
|Client platform requirements  <br/> |Aplicativos cliente do Shell de gerenciamento do Exchange exigem o Windows PowerShell 2.0.  <br/> |
|Permissões  <br/> |Executando um Shell de gerenciamento do Exchange aplicativo exige que o usuário tem direitos de controle de acesso baseado em função para os dados afetados no armazenamento do Exchange.<br/>Para obter mais informações sobre controle de acesso baseado em função, consulte [Understanding Role Based Access Control](http://technet.microsoft.com/en-us/library/dd298183.aspx).  <br/> |
   
Os artigos nesta seção descrevem os recursos do Shell de gerenciamento do Exchange que são importantes para a criação de ferramentas de gerenciamento do Exchange. Para obter informações sobre planejamento, configuração ou manutenção do Exchange, consulte o site do [Exchange](https://docs.microsoft.com/en-us/exchange/) .
  
## <a name="in-this-section"></a>Nesta se��o

- [Criar ferramentas do Shell de gerenciamento do Exchange](create-exchange-management-shell-tools.md)
    
- [Namespaces do Shell de gerenciamento do Exchange](exchange-management-shell-namespaces.md)
    
## <a name="see-also"></a>Confira também
  
- [Documentação do Windows PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/getting-started/getting-started-with-windows-powershell?view=powershell-6)
- [Script do PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/powershell-scripting?view=powershell-6)
    

