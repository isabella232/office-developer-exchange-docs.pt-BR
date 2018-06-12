---
title: Exchange Online e o desenvolvimento do Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f33d1093-75ba-4ff2-8d15-b0bf73a401bf
description: Encontre documentação completa de desenvolvedor para o Exchange Server, incluindo o Exchange Online como parte do Office 365, do Exchange Online, do Exchange 2013, do API Gerenciada do EWS, do Exchange 2010 e do Exchange 2007.
ms.openlocfilehash: b933bd1bdc6dfcbe4941f23dbee9a587745c7bd7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750645"
---
# <a name="exchange-online-and-exchange-development"></a>Exchange Online e o desenvolvimento do Exchange

Encontre documentação completa de desenvolvedor para o Exchange Server, incluindo o Exchange Online como parte do Office 365, do Exchange Online, do Exchange 2013, do API Gerenciada do EWS, do Exchange 2010 e do Exchange 2007. 

Você pode usar o como, obtenha iniciado, o novo recurso e documentação de referência de API para desenvolver ferramentas para acessar e gerenciar dados de caixa de correio de serviços, sites, computadores desktop e dispositivos móveis e para criar soluções personalizadas para email, calendário, contatos, e outros itens que estão armazenadas no Exchange Online ou em um servidor Exchange 2013. 

Você pode usar o Serviços Web do Exchange (EWS), a Descoberta Automática, aplicativos de email do Office ou outras APIs para desenvolver seus aplicativos. Esta página ajuda você a escolher a tecnologia Exchange direita.

## <a name="exchange-developer-content"></a>Conteúdo de desenvolvedor do Exchange  

Use a tabela a seguir para identificar a tecnologia e o conteúdo de API relacionado que ajudará você a alcançar seus objetivos de desenvolvimento.  
  
|Se você estiver criando…|Comece aqui|
|:-----|:-----|
|Um aplicativo baseado em REST para acessar o Exchange Online como parte do Office 365|[APIs de restante do Office 365 para emails, calendários e contatos](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md) |
|Um aplicativo sensível ao contexto para exibir informações no Outlook, Outlook Web App ou OWA para dispositivos |[Aplicativos de email para o Outlook e o EWS no Exchange](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) |
|Um cliente de caixa de correio que não seja baseado no .NET Framework ou Java |[Explorar a API Gerenciada pelo EWS, EWS e serviços Web no Exchange](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) |
|Um cliente de caixa de correio que usa o .NET Framework para acessar o EWS |[Introdução aos aplicativos de cliente API gerenciada de EWS](exchange-web-services/get-started-with-ews-managed-api-client-applications.md) |
|Um cliente de caixa de correio que usa o Java para acessar o EWS |[API Java do EWS no GitHub](https://github.com/OfficeDev/ews-java-api) |
|Um aplicativo que personaliza a interface de usuário do Outlook ou depende de lógica de negócios do Outlook  |[Referência de VBA do Outlook](https://msdn.microsoft.com/en-us/VBA/VBA-Outlook) |
|Um aplicativo que tem como destino o Exchange Online ou o Exchange 2013 que você precisa saber para migrar de uma versão anterior do Exchange  |[Migrar para as tecnologias do Exchange ](migrating-to-exchange-online-and-exchange-2013-technologies.md) |
|Uma ferramenta de gerenciamento personalizado que usa o Windows PowerShell do código gerenciado   |[Shell de Gerenciamento do Exchange](management/exchange-management-shell.md) |
|Uma solução de backup ou restaurar dados do Exchange  |[Backup e restauração para o Exchange](backup-restore/backup-and-restore-for-exchange-2013.md) |
|Uma extensão para dar suporte ao acessar mensagens no pipeline de transporte   |[Agentes de transporte no Exchange](transport-agents/transport-agents-in-exchange-2013.md)  |
|Um cliente de caixa de correio para um dispositivo móvel   |[Exchange ActiveSync](https://technet.microsoft.com/en-us/library/aa998357.aspx) |
   
## <a name="exchange-interactions-with-custom-applications"></a>Exchange interações com aplicativos personalizados

Algumas destas tecnologias permitem que seus aplicativos funcionem com dados armazenados no Exchange, outros são usados para gerenciar e controlar o servidor do Exchange. Em vários casos, você pode utilizar mais de uma tecnologia ou linguagem de programação para concluir uma tarefa, o que possibilita o uso das tecnologias e linguagens com as quais você está mais familiarizado. Por exemplo, você pode definir propriedades em itens do repositório do Exchange usando a API REST de Email, EWS ou o API Gerenciada do EWS.
  
O Exchange interage com aplicativos personalizados de várias maneiras, dependendo da arquitetura e da funcionalidade do aplicativo. Em seu núcleo, o Exchange não somente transporta mensagens, mas também realiza manutenção em caixas de correio, executa aplicativos baseados em forma, e muito mais.

|Interações do Exchange|Descrição|
|:-----|:-----|
|**Transporte de mensagem**|O Exchange funciona como um servidor de email padrão para aplicativos que enviam mensagens.<br/>O Exchange inclui várias APIs que transferem mensagens, incluindo REST, EWS, e o API Gerenciada do EWS.<br/>Além disso, os aplicativos podem usar agentes de transporte para responder conforme as mensagens sejam processadas e entregues pelo Exchange. |
|**Armazenamento de caixa de correio** |O Exchange fornece uma estrutura hieráquica de pastas, itens e propriedades para aplicativos que acessam dados armazenados em caixas de correio.<br/>Você pode acessar essas informações armazenadas usando uma combinação de bancos de dados e estilos de objeto do componente.<br/>Você pode realizar consultas nos dados e o Exchange gerencia o acesso aos dados armazenados com base nas permissões de usuário e de armazenamento.<br/>Os aplicativos que manipulam dados de caixa de correio normalmente utilizam REST, EWS ou o API Gerenciada do EWS.|
|**Servidor enterprise gerenciada** |O Exchange funciona como um servidor gerenciado para aplicativos que gerenciam servidores e repositórios do Exchange.<br/>Os aplicativos podem configurar, controlar e monitorar a atividade e a integridade atuais dos servidores do Exchange em toda a organização.<br/>Os aplicativos de gerenciamento do Exchange usam o Shell de Gerenciamento do Exchange para gerenciar servidores do Exchange. |
   
## <a name="see-also"></a>Confira também

- [Referência de API do servidor do Exchange](https://msdn.microsoft.com/en-us/library/dn186243(v=exchg.150).aspx)
- [Leia sobre o Exchange nos Blogs do Office](https://www.microsoft.com/en-us/microsoft-365/blog/) 
- [Obtenha 101 exemplos de código para o Exchange 2013](https://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c)
- [Obtenha a API gerenciada de EWS (GitHub)](https://github.com/OfficeDev/ews-managed-api/blob/master/README.md)
- [Obtenha suporte para o Exchange Server](https://support.microsoft.com/en-us/getsupport?oaspworkflow=start_1.0.0.0&wf=0&wfname=productselection&gprid=730&x=13&y=7&st=1&wfxredirect=1&sd=gn&ccsid=635890984021344661&forceorigin=esmc)


