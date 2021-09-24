---
title: Shell de Gerenciamento do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 8cc0c4fa-9e13-45cb-88da-0486f2ac1bd0
description: Encontre informações sobre como usar o Shell de Gerenciamento Exchange para desenvolver ferramentas para Exchange de servidor.
ms.openlocfilehash: ee1cbcb174c7153ca6cd9bb089580b372bf9029b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516149"
---
# <a name="exchange-management-shell"></a>Shell de Gerenciamento do Exchange

Encontre informações sobre como usar o Shell de Gerenciamento Exchange para desenvolver ferramentas para Exchange de servidor.
  
**Aplica-se a:** Exchange Online | Exchange Server 2013 | Office 365
  
O Shell de Gerenciamento do Exchange fornece um conjunto rico de comandos, com base na plataforma Windows PowerShell, para gerenciar Exchange Online, Exchange Online como parte do Office 365 ou uma versão local do Exchange começando com Exchange 2013. Você pode usar o Shell de Gerenciamento Exchange para criar dois tipos de ferramentas: scripts de linha de comando que funcionam no ambiente Windows PowerShell e ferramentas que usam os cmdlets do Shell de Gerenciamento Exchange por meio de uma interface gerenciada. Você pode usar aplicativos gerenciados para criar uma interface do usuário Windows padrão ou baseada na Web para administrar um Exchange servidor. 
  
## <a name="what-you-need-to-know-about-the-exchange-management-shell"></a>O que você precisa saber sobre o shell de gerenciamento Exchange gerenciamento

|Se você estiver se perguntando sobre|Leia isto|
|:-----|:-----|
|Disponibilidade  <br/> |Exchange Os comandos do Shell de Gerenciamento são instalados em todos os servidores que executam versões Exchange a partir Exchange 2007.<br/>Os aplicativos cliente podem ser implantados em qualquer computador que Windows PowerShell 2.0.<br/> Para obter informações sobre como acessar o shell, [consulte Exchange Server PowerShell (Exchange Shell](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)de Gerenciamento) .  <br/> |
|Ferramentas e idiomas  <br/> |Você pode criar Exchange scripts do Shell de Gerenciamento em qualquer editor de texto.<br/>Você pode usar uma das muitas ferramentas de terceiros para criar Windows PowerShell scripts que podem ser usados com o Shell de Gerenciamento Exchange.  <br/> O [Exchange de objeto shell de gerenciamento](exchange-management-shell-namespaces.md) baseia-se no .NET Framework.<br/>Você pode usar qualquer idioma .NET para desenvolver aplicativos Exchange Shell de Gerenciamento.  <br/> |
|Ferramentas de teste e depuração disponíveis  <br/> |Você pode usar um dos vários aplicativos de terceiros para testar e depurar Exchange scripts do Shell de Gerenciamento.  <br/> Você pode usar Visual Studio e ferramentas de terceiros para testar e depurar aplicativos gerenciados Exchange Shell de Gerenciamento.  <br/> |
|Requisitos da plataforma do servidor  <br/> |Você pode usar o Shell de Gerenciamento Exchange em qualquer servidor Exchange que tenha Windows PowerShell 2.0 instalado.  <br/> |
|Requisitos da plataforma do cliente  <br/> |Exchange Os aplicativos cliente shell de gerenciamento exigem Windows PowerShell 2.0.  <br/> |
|Permissões  <br/> |Executar um Exchange aplicativo Shell de Gerenciamento exige que o usuário tenha direitos de controle de acesso baseado em função para os dados afetados no Exchange store.<br/>Para obter mais informações sobre o controle de acesso baseado em função, consulte [Understanding Role Based Access Control](https://technet.microsoft.com/library/dd298183.aspx).  <br/> |
   
Os artigos nesta seção descrevem Exchange recursos do Shell de Gerenciamento que são importantes para criar Exchange de gerenciamento. Para obter informações sobre planejamento, configuração ou manutenção Exchange, consulte [o](https://docs.microsoft.com/exchange/) Exchange site.
  
## <a name="in-this-section"></a>Nesta seção

- [Criar ferramentas do Shell de Gerenciamento do Exchange](create-exchange-management-shell-tools.md)
    
- [Namespaces do Shell de Gerenciamento do Exchange](exchange-management-shell-namespaces.md)
    
## <a name="see-also"></a>Confira também
  
- [Windows PowerShell documentação](https://docs.microsoft.com/powershell/scripting/getting-started/getting-started-with-windows-powershell?view=powershell-6)
- [Scripts do PowerShell](https://docs.microsoft.com/powershell/scripting/powershell-scripting?view=powershell-6)
    

