---
title: Suplementos do Outlook e EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 821c8eb9-bb58-42e8-9a3a-61ca635cba59
description: Encontre informações sobre os suplementos do Outlook e como eles funcionam com o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: 2b0cee2017c24d714fa444c094ab1797be1fbe99
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456273"
---
# <a name="outlook-add-ins-and-ews-in-exchange"></a>Suplementos do Outlook e EWS no Exchange

Encontre informações sobre os suplementos do Outlook e como eles funcionam com o EWS no Exchange.

Os suplementos do Outlook oferecem uma interface única e um modelo de programação que usa padrões da Web para permitir que você crie uma experiência personalizada para seus usuários de email. Você pode criar aplicativos de email que exibem informações contextuais ou úteis em um quadro HTML5 hospedado no Outlook; por exemplo, um aplicativo de email pode mostrar um mapa do Bing com um endereço realçado quando uma mensagem de email contém um endereço. Ou quando um usuário está redigindo uma mensagem, um aplicativo de email pode mostrar informações adicionais sobre o destinatário e inserir uma saudação padrão no email com o toque de um botão.

> [!NOTE]
> "Outlook" neste artigo se refere ao cliente avançado do Outlook, Outlook RT, Outlook Web App, e OWA para Dispositivos.

A interface de aplicativos de email faz parte da API JavaScript para Office. Você pode usar a API para acessar informações no Exchange para habilitar o aplicativo de email para:

- [Reconhecer entidades](https://msdn.microsoft.com/library/a6b0904b-afe9-4882-9136-3d8cfd57fcf8%28Office.15%29.aspx), como endereços, números de telefone, sugestões de tarefas ou sugestões de reunião em um email.

- Abrir e exibir [mensagens](https://msdn.microsoft.com/library/d0bca550-70c3-457c-85f8-e19b39e3b892%28Office.15%29.aspx) e [compromissos](https://msdn.microsoft.com/library/6cfbc29d-8581-474e-9a8b-510471e4bf8b%28Office.15%29.aspx) existentes em um modo de exibição separado para que os usuários possam fazer referência cruzada de informações em uma ou mais mensagens.

- [Faça solicitações de EWS](https://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) para o servidor Exchange que hospeda a caixa de correio do usuário. Um aplicativo de email pode, por exemplo, obter uma lista de pastas para que o usuário possa escolher uma para armazenar a mensagem ou mostrar todos os itens em uma conversa ou marcar uma mensagem de email como lixo eletrônico.

- [Obtenha um token](https://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) para identificar exclusivamente uma conta de email a fim de habilitar o logon único em um serviço de terceiros.

- [Obter um token](https://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) que permite que um serviço de terceiros faça solicitações do EWS em nome do usuário, por exemplo, para extrair os anexos de um item ou para obter um item do Exchange Server para processamento adicional.

Você pode usar aplicativos de email para personalizar a experiência do Outlook Web App para seus usuários; se, no entanto, você quiser personalizar a "aparência" do Outlook Web App, consulte estes artigos no TechNet:

- [Criar um tema para o Outlook Web App](https://technet.microsoft.com/library/bb201700%28v=exchg.150%29.aspx)

- [Personalizar as páginas de entrada, de seleção de idioma e de erro do Outlook Web App](https://technet.microsoft.com/library/ee633483%28v=exchg.150%29.aspx)

Sua organização pode instalar aplicativos de email em um servidor interno para limitar o acesso a usuários autorizados ou você e outros desenvolvedores de aplicativos de email podem colocar aplicativos de email na [Office Store](https://office.microsoft.com/store/) para venda ao público geral. Qualquer pessoa que esteja executando o Outlook pode baixar, instalar e usar aplicativos de email do Marketplace.

Se você quiser saber mais sobre a criação de aplicativos de email, confira a [documentação dos suplementos do Outlook](/outlook/add-ins) ou [faça um](https://code.msdn.microsoft.com/exchange/Mail-apps-for-Outlook-Make-770b2528) exemplo de solicitação do EWS.

## <a name="ews-and-outlook-add-ins"></a>Suplementos do EWS e do Outlook

Você pode usar um subconjunto de operações EWS no servidor Exchange que hospeda a conta que executa um aplicativo de email.

A função [Mailbox. makeEwsRequestAsync](https://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) permite que você faça solicitações de EWS do seu aplicativo de email de volta para o servidor que hospeda a caixa de correio do usuário. Você cria o envelope SOAP e a solicitação XML, e a função **makeEwsRequestAsync** chama o EWS com um token de autenticação que identifica a caixa de correio e o aplicativo de email que está fazendo a solicitação. Para ajudar a proteger a caixa de correio do usuário, o servidor Exchange rejeitará todas as solicitações que não são provenientes do aplicativo de email ou de uma caixa de correio que não esteja hospedada no servidor.

Como qualquer outro aplicativo, um aplicativo de email precisa de permissões para funcionar. O administrador precisa:

- [Conceda acesso do EWS](controlling-client-application-access-to-ews-in-exchange.md) ao usuário de aplicativos de email.

- [Defina "OAuthAuthentication" como true](https://technet.microsoft.com/library/aa997233%28v=exchg.150%29.aspx) no diretório EWS do servidor de acesso para cliente.

Você também precisa certificar-se de que seu aplicativo solicite a permissão de leitura/gravação de caixa de correio no [modelo de permissão](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)de aplicativos para Office.

Quando essas etapas estiverem concluídas, um subconjunto de operações do EWS de pasta e item estará disponível para o aplicativo de email a ser usado.

**Tabela 1. Operações de pasta e item do EWS que os aplicativos de email podem usar**

|**Operações de pasta**|**Operações de item**|
|:-----|:-----|
|[Operação CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [Operação FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [Operação GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [Operação UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |[Operação CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [Operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [Operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> [Operação FindConversation](https://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> [Operação GetConversationItems](https://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> [Operação GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [Operação MarkAsJunk](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) <br/> [Operação MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [Operação SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) <br/> [Operação UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |

### <a name="service-callback-tokens"></a>Tokens de retorno de chamada de serviço

Os tokens de retorno de chamada de serviço permitem que os aplicativos de email transmitam um token de acesso para um serviço de terceiros, para que o serviço possa fazer solicitações de EWS ao servidor Exchange que hospeda a caixa de correio. Por exemplo, um aplicativo de email pode passar um token de retorno de chamada de serviço para um serviço de terceiros junto com uma lista de IDs de anexo para imagens anexadas a um email. O serviço pode então usar as IDs de anexo e o token de retorno de chamada para fazer uma solicitação de EWS ao servidor Exchange do usuário para obter as imagens anexadas. Os aplicativos de email também podem usar o token de retorno de chamada de serviço com uma lista de IDs de item para receber itens de email e de compromisso do servidor Exchange.

O token de retorno de chamada de serviço é um token opaco que o serviço de terceiros anexa à solicitação EWS em um cabeçalho de autenticação de portador. O token identifica o aplicativo de email e a caixa de correio para ajudar a proteger a solicitação do EWS. Para saber como usar tokens de retorno de chamada de serviço, confira os [suplementos do Outlook: obter anexos de um exemplo do Exchange Server](https://code.msdn.microsoft.com/exchange/Mail-apps-for-Office-Get-38babdc9) .

## <a name="see-also"></a>Confira também


- [Controlando o acesso do aplicativo cliente ao EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md)

- [Método Mailbox. makeEwsRequestAsync (API JavaScript para Office)](https://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx)

- [Suplementos do Outlook](https://docs.microsoft.com/outlook/add-ins)

- [Método Mailbox. getUserIdentityTokenAsync (API JavaScript para Office)](https://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx)

- [Autenticar um suplemento do Outlook usando tokens de identidade do Exchange](https://msdn.microsoft.com/library/c0520a1e-d9ba-495a-a99f-6816d7d2a23e%28Office.15%29.aspx)

- [Noções básicas sobre permissões de suplemento do Outlook](https://docs.microsoft.com/outlook/add-ins/understanding-outlook-add-in-permissions)

- [Set-WebServicesVirtualDirectory](https://technet.microsoft.com/library/aa997233%28v=exchg.150%29.aspx)

- [Suplementos do Outlook: fazer uma solicitação de EWS](https://code.msdn.microsoft.com/office/Mail-apps-for-Outlook-Make-770b2528)

- [Suplementos do Outlook: usar um token de identidade do cliente](https://code.msdn.microsoft.com/Mail-apps-for-Outlook-Use-b20a66b6)

- [Suplementos do Outlook: obter anexos de um servidor Exchange](https://code.msdn.microsoft.com/office/Mail-apps-for-Office-Get-38babdc9)
