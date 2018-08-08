---
title: Desenvolvimento do Exchange Online e do Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f33d1093-75ba-4ff2-8d15-b0bf73a401bf
description: Encontre documentação completa de desenvolvedor para o Exchange Server, incluindo o Exchange Online como parte do Office 365, do Exchange Online, do Exchange 2013, do API Gerenciada do EWS, do Exchange 2010 e do Exchange 2007.
ms.openlocfilehash: 2af9e52c3f7cf03d7571d1640ef7bfa45b5e97be
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353242"
---
# <a name="exchange-online-and-exchange-development"></a>Desenvolvimento do Exchange Online e do Exchange

Encontre documentação completa de desenvolvedor para o Exchange Server, incluindo o Exchange Online como parte do Office 365, do Exchange Online, do Exchange 2013, do API Gerenciada do EWS, do Exchange 2010 e do Exchange 2007.

Você pode usar a documentação de referência como, iniciar, novo recurso e API para desenvolver ferramentas para acessar e gerenciar dados de caixas de correio de serviços, sites, PCs e dispositivos móveis, e para criar soluções personalizadas para email, calendário, contatos e outros itens que ficam armazenados no Exchange Online ou em um servidor Exchange 2013.

Você pode usar o Serviços Web do Exchange (EWS), a Descoberta Automática, suplementos do Outlook ou APIs para desenvolver seus aplicativos. Esta página ajuda você a escolher a tecnologia correta do Exchange.

## <a name="exchange-developer-content"></a>Conteúdo de desenvolvedor do Exchange

Use a tabela a seguir para identificar a tecnologia e o conteúdo relacionado à API que ajudarão você a atingir suas metas de desenvolvimento.

> [!IMPORTANT]
> O Microsoft Graph é a API recomendada para acessar dados do Exchange Online. Os novos aplicativos desenvolvidos para acessar dados do Exchange Online devem usar o Microsoft Graph.

|Se você estiver criando…|Comece aqui|
|:-----|:-----|
|Um aplicativo com base em REST para acessar o Exchange Online como parte do Office 365.|[APIs REST do Microsoft Graph para email, calendários e contatos](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md) |
|Um aplicativo contextual para exibir as informações no Outlook, Outlook Web App ou OWA para Dispositivos. |[Suplementos do Outlook e EWS no Exchange](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) |
|Um cliente de caixa de correio que não se baseia em .NET Framework ou em Java. |[Explorar os recursos da API gerenciada por EWS, EWS e serviços web do Exchange](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) |
|Um cliente de caixa de correio que usa o .NET Framework para acessar o EWS |[Introdução aos aplicativos clientes de API gerenciada por EWS](exchange-web-services/get-started-with-ews-managed-api-client-applications.md) |
|Um cliente de caixa de correio que usa o Java para acessar o EWS |[API Java EWS no GitHub](https://github.com/OfficeDev/ews-java-api) |
|Um aplicativo que personaliza a interface do usuário do Outlook ou depende da lógica de negócios do Outlook  |[Referência do VBA do Outlook](https://msdn.microsoft.com/pt-BR/VBA/VBA-Outlook) |
|Um aplicativo que tem como alvo o Exchange Online ou o Exchange 2013 e que precisa ser migrado de uma versão anterior do Exchange  |[Migrando para as tecnologias Exchange](migrating-to-exchange-online-and-exchange-2013-technologies.md) |
|Uma ferramenta de gerenciamento personalizada que usa o Windows PowerShell a partir do código gerenciado   |[Shell de Gerenciamento do Exchange](management/exchange-management-shell.md) |
|Uma solução de backup ou restauração de dados do Exchange  |[Backup e restauração para o Exchange](backup-restore/backup-and-restore-for-exchange-2013.md) |
|Uma extensão para suportar o acesso a mensagens no pipeline de transporte.   |[Agentes de transporte no Exchange](transport-agents/transport-agents-in-exchange-2013.md)  |
|Um cliente de caixa de correio para um dispositivo móvel   |[Exchange ActiveSync](https://technet.microsoft.com/pt-BR/library/aa998357.aspx) |

## <a name="exchange-interactions-with-custom-applications"></a>Interações do Exchange com aplicativos personalizados

Algumas destas tecnologias permitem que seus aplicativos funcionem com dados armazenados no Exchange, outros são usados para gerenciar e controlar o servidor do Exchange. Em vários casos, você pode utilizar mais de uma tecnologia ou linguagem de programação para concluir uma tarefa, o que possibilita o uso das tecnologias e linguagens com as quais você está mais familiarizado. Por exemplo, você pode definir propriedades em itens do repositório do Exchange usando a API REST de Email, EWS ou o API Gerenciada do EWS.

O Exchange interage com aplicativos personalizados de várias maneiras, dependendo da arquitetura e da funcionalidade do aplicativo. Em seu núcleo, o Exchange não somente transporta mensagens, mas também realiza manutenção em caixas de correio, executa aplicativos baseados em forma, e muito mais.

|Interação do Exchange
|Descrição|
|:-----|:-----|
|**Transporte de mensagens**|O Exchange funciona como um servidor de email padrão para aplicativos que enviam mensagens.<br/>O Exchange inclui várias APIs que transferem mensagens, incluindo REST, EWS, e o API Gerenciada do EWS.<br/>Além disso, os aplicativos podem usar agentes de transporte para responder conforme as mensagens são processadas e entregues pelo Exchange. |
|**Armazenamento de caixa de correio** |O Exchange oferece uma estrutura hierárquica de pastas, itens e propriedades para aplicativos que acessam dados armazenados em caixas de correio.<br/>Você pode acessar essas informações armazenadas usando uma combinação de bancos de dados e estilos de objeto do componente.<br/>Você pode realizar consultas nos dados e o Exchange gerencia o acesso aos dados armazenados com base nas permissões de usuário e de armazenamento.<br/>Os aplicativos que manipulam dados de caixas de correio geralmente usam REST, EWS ou a API gerenciada do EWS.|
|**Servidor de empresa gerenciada** |O Exchange funciona como um servidor gerenciado de aplicativos que gerenciam lojas e servidores do Exchange.<br/>Os aplicativos podem configurar, controlar e monitorar a atividade e a integridade atuais dos servidores do Exchange em toda a organização.<br/>Os aplicativos de gerenciamento do Exchange usam o Shell de Gerenciamento do Exchange para gerenciar servidores do Exchange. |

## <a name="see-also"></a>Confira também

- 
  [Referência de API de servidor para Exchange](https://msdn.microsoft.com/en-us/library/dn186243(v=exchg.150).aspx)
- [Ler sobre Exchange em Blogs do Office](https://www.microsoft.com/pt-BR/microsoft-365/blog/)
- [Obter 101 amostras de código para o Exchange 2013](https://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c)
- [Obter a API gerenciada do EWS (GitHub)](https://github.com/OfficeDev/ews-managed-api/blob/master/README.md)
- [Obter suporte para o Exchange Server](https://support.microsoft.com/en-us/getsupport?oaspworkflow=start_1.0.0.0&wf=0&wfname=productselection&gprid=730&x=13&y=7&st=1&wfxredirect=1&sd=gn&ccsid=635890984021344661&forceorigin=esmc)
