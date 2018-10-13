---
title: Suplementos do Outlook e EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 821c8eb9-bb58-42e8-9a3a-61ca635cba59
description: Encontre informações sobre os suplementos do Outlook e como eles funcionam com o EWS no Exchange.
ms.openlocfilehash: 7eae834fe0bb93e2e94f094e811ab6cf002fc71b
ms.sourcegitcommit: 42eecc78e7aed7e95f73370d6c39ab8f4e96bf68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/12/2018
ms.locfileid: "25541635"
---
# <a name="outlook-add-ins-and-ews-in-exchange"></a>Suplementos do Outlook e EWS no Exchange

Encontre informações sobre os suplementos do Outlook e como eles funcionam com o EWS no Exchange.

Suplementos do Outlook fornecem uma interface única e um modelo de programação que usa os padrões da web para habilitá-lo criar uma experiência personalizada para seus usuários de email. Você pode criar aplicativos de email que exibem informações contextuais ou úteis em um quadro de HTML5 hospedado no Outlook; Por exemplo, um aplicativo de email pode mostrar um Bing map com um endereço realçado quando uma mensagem de email contém um endereço. Ou quando um usuário está redigindo uma mensagem, um aplicativo de email pode mostrar informações adicionais sobre o destinatário e inserir uma saudação padrão em email com o toque de um botão.

> [!NOTE]
> "Outlook" neste artigo se refere ao cliente avançado do Outlook, Outlook RT, Outlook Web App, e OWA para Dispositivos.

A interface de aplicativos de email é parte da API do JavaScript para Office. Você pode usar a API para acessar informações no Exchange para permitir que seu aplicativo de email para:

- [Recognize entidades](http://msdn.microsoft.com/library/a6b0904b-afe9-4882-9136-3d8cfd57fcf8%28Office.15%29.aspx), como números de telefone, endereços, sugestões de tarefa ou sugestões de reunião em um email.

- Abrir e exibir o existente de [mensagens](http://msdn.microsoft.com/library/d0bca550-70c3-457c-85f8-e19b39e3b892%28Office.15%29.aspx) e [compromissos](http://msdn.microsoft.com/library/6cfbc29d-8581-474e-9a8b-510471e4bf8b%28Office.15%29.aspx) em um modo de exibição separado, para que os usuários podem fazer referência cruzada informações em uma ou mais mensagens.

- [Tornar o EWS solicitações](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) ao servidor do Exchange que hospeda a caixa de correio do usuário. Um aplicativo de email pode, por exemplo, obter uma lista de pastas, para que o usuário possa escolher uma para armazenar a mensagem ou mostrar todos os itens em uma conversa ou marcar uma mensagem de email como lixo eletrônico.

- [Obter um token](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) para identificar exclusivamente uma conta de email para habilitar um único entrar em um serviço de terceiros.

- [Obter um token](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) que permite a um serviço de terceiros para fazer solicitações EWS em nome do usuário, por exemplo, para extrair os anexos de um item ou obter um item do servidor do Exchange para processamento adicional.

Você pode usar aplicativos de email para personalizar a experiência do Outlook Web App para seus usuários; Se, no entanto, você desejar personalizar a "aparência" do Outlook Web App, consulte estes artigos no TechNet:

- [Criar um tema para o Outlook Web App](http://technet.microsoft.com/en-us/library/bb201700%28v=exchg.150%29.aspx)

- [Personalizar o Outlook Web App entrar, seleção de idioma e páginas de erro](http://technet.microsoft.com/en-us/library/ee633483%28v=exchg.150%29.aspx)

Sua organização pode instalar aplicativos de email em um servidor interno para limitar o acesso aos usuários autorizados ou outros desenvolvedores de aplicativos de email e você podem colocar aplicativos de email no [Office Store](http://office.microsoft.com/store/) para venda para o público em geral. Qualquer pessoa que está executando o Outlook pode baixar, instalar e usar aplicativos de email no marketplace.

Se você deseja saber mais sobre a criação de aplicativos de email, confira a [documentação de suplementos do Outlook](/outlook/add-ins) ou a amostra de [fazer uma solicitação EWS](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Outlook-Make-770b2528) .

## <a name="ews-and-outlook-add-ins"></a>Suplementos EWS e Outlook

Você pode usar um subconjunto das operações do EWS no Exchange server que hospeda a conta que executa um aplicativo de email.

A função [mailbox.makeEwsRequestAsync](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) permite que você faça solicitações EWS do seu aplicativo de email volta para o servidor que hospeda a caixa de correio do usuário. Crie o envelope SOAP e solicitação XML e as chamadas de função **makeEwsRequestAsync** EWS com um token de autenticação que identifica a caixa de correio e aplicativo que está fazendo a solicitação de email. Para ajudar a proteger a caixa de correio do usuário, o Exchange server rejeitará quaisquer solicitações que não vêm do aplicativo de email ou de uma caixa de correio que não está hospedada no servidor.

Como qualquer outro aplicativo, um aplicativo de email precisa ter permissões para trabalhar. O administrador precisa:

- [EWS conceder acesso](controlling-client-application-access-to-ews-in-exchange.md) ao usuário de aplicativos de email.

- [Set "OAuthAuthentication" como true](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx) no diretório do EWS de servidor de acesso do cliente.

Você também precisará certificar-se de que o seu aplicativo solicita a permissão de caixa de correio de leitura/gravação em aplicativos para Office [modelo de permissão](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).

Quando essas etapas forem concluídas, um subconjunto das operações de EWS do item e pasta estão disponíveis para o aplicativo de email usar.

**Tabela 1. Operações de pasta e item EWS que aplicativos de email podem usar**

|**Operações de pasta**|**Operações de item**|
|:-----|:-----|
|[Operação CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [Operação FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [Operação GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [Operação UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |[Operação CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [Operação CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [Operação FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> [Operação FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> [Operação GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> [Operação GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [Operação MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) <br/> [Operação MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [Operação SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) <br/> [Operação UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |

### <a name="service-callback-tokens"></a>Tokens de retorno de chamada do serviço

Tokens de retorno de chamada do serviço permitem que aplicativos de email passar um token de acesso a um serviço de terceiros para que o serviço possa fazer solicitações EWS ao servidor do Exchange que hospeda a caixa de correio. Por exemplo, um aplicativo de email pode passar um token de retorno de chamada do serviço para um serviço de terceiros, juntamente com uma lista de IDs de anexo para imagens anexados a um email. O serviço, em seguida, pode usar o anexo IDs e o token de retorno de chamada para fazer uma solicitação EWS ao servidor do Exchange do usuário para obter as imagens anexadas. Aplicativos de email também podem usar o token de serviço de retorno de chamada com uma lista de IDs de item para obter itens de compromisso e de email do Exchange server.

O token de retorno de chamada de serviço é um token de opaco que o serviço de terceiros anexa à solicitação de EWS em um cabeçalho de autenticação do transportador. O token identifica o aplicativo de email e a caixa de correio para ajudar a proteger a solicitação do EWS. Para saber como usar os tokens de retorno de chamada de serviço, consulte o [suplementos do Outlook: fazer anexos a partir de um servidor Exchange](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Office-Get-38babdc9) amostra.

## <a name="see-also"></a>Confira também


- [Controlando o acesso do aplicativo de cliente para o EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md)

- [Método Mailbox.makeEwsRequestAsync (API do JavaScript para Office)](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx)

- 
  [Suplementos do Outlook](https://docs.microsoft.com/outlook/add-ins)

- [Método Mailbox.getUserIdentityTokenAsync (API do JavaScript para Office)](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx)

- [Autenticar um suplemento do Outlook usando tokens de identidade do Exchange](http://msdn.microsoft.com/library/c0520a1e-d9ba-495a-a99f-6816d7d2a23e%28Office.15%29.aspx)

- [Especificar as permissões para Outlook suplemento acesso à caixa de correio do usuário](https://docs.microsoft.com/en-us/outlook/add-ins/understanding-outlook-add-in-permissions)

- [Set-WebServicesVirtualDirectory](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx)

- [Suplementos do Outlook: tornar uma solicitação EWS](http://code.msdn.microsoft.com/office/Mail-apps-for-Outlook-Make-770b2528)

- [Suplementos do Outlook: Use um token de identidade do cliente](http://code.msdn.microsoft.com/Mail-apps-for-Outlook-Use-b20a66b6)

- [Suplementos do Outlook: obter os anexos de um servidor do Exchange](http://code.msdn.microsoft.com/office/Mail-apps-for-Office-Get-38babdc9)
