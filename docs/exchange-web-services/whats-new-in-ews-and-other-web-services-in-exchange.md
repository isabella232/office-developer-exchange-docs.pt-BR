---
title: O que há de novo no EWS e outros serviços Web no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: aff6328f-cff1-42a6-9a4d-ea4d2d0461cf
description: Descubra as novidades do EWS e dos serviços Web no Exchange e a API gerenciada do EWS.
localization_priority: Priority
ms.openlocfilehash: 5e74ad9d4cf5083983c28e477fd50d48e2d7fbb6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529837"
---
# <a name="whats-new-in-ews-and-other-web-services-in-exchange"></a>O que há de novo no EWS e outros serviços Web no Exchange

Descubra as novidades do EWS e dos serviços Web no Exchange e a API gerenciada do EWS.
  
Os serviços Web do Exchange foram atualizados para incluir novos recursos. 
  
**Tabela 1. Novos recursos de serviço Web no Exchange Online, no Exchange 2013 e na API gerenciada do EWS**

|Recurso|Implementado no Exchange Online|Implementado no Exchange 2013|Implementado na API gerenciada do EWS|
|:-----|:-----:|:-----:|:-----:|
|[Descoberta eletrônica](#eDisc) <br/> |Sim  <br/> |Sim  <br/> |Sim  <br/> |
|[Arquivamento](#arch) <br/> |Sim  <br/> |Sim  <br/> |Sim  <br/> |
|[Personas](#personas) <br/> |Sim  <br/> |Sim  <br/> |Não  <br/> |
|[Repositório de Contatos Unificado](#unified) <br/> |Sim  <br/> |Sim  <br/> |Não  <br/> |
|[Políticas de retenção](#retentionpolicy) <br/> |Sim  <br/> |Sim  <br/> |Sim  <br/> |
|[Fotos do usuário](#userphoto) <br/> |Sim  <br/> |Sim  <br/> |Não  <br/> |
|[Aplicativos de email para gerenciamento do Outlook](#ewsmailapps) <br/> |Sim  <br/> |Sim  <br/> |Sim  <br/> |
|[Propor novo horário de reunião](#propose) <br/> |Sim  <br/> |Não  <br/> |Não  <br/> |

<a name="eDisc"> </a>

## <a name="ediscovery-in-ews"></a>Descoberta eletrônica no EWS

a descoberta eletrônica é um serviço Web de consulta federada que permite que aplicativos externos, como o SharePoint 2013, realizem consultas de dados do Exchange. A descoberta consiste em várias fases, incluindo a identificação e preservação de dados importantes, a remoção e a revisão dos dados e a produção de dados no tribunal. as consultas de descoberta eletrônica facilitam o processo de descoberta fornecendo um único fluxo de trabalho de descoberta no Exchange e no SharePoint.
  
**Tabela 2. Operações do EWS e métodos da API gerenciada do EWS para trabalhar com a descoberta eletrônica**

|**Nome da operação**|**Método de API gerenciada do EWS**|**Descrição**|
|:-----|:-----|:-----|
|[Operação GetDiscoverySearchConfiguration](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |[ExchangeService. GetDiscoverySearchConfiguration ()](https://msdn.microsoft.com/library/jj670206%28v=exchg.80%29.aspx) <br/> |Obtém informações de configuração para bloqueios in-loco, pesquisas salvas de descoberta e caixas de correio habilitadas para pesquisa de descoberta.  <br/> |
|[Operação GetHoldOnMailboxes](https://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |[ExchangeService. GetHoldOnMailboxes ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getholdonmailboxes%28v=exchg.80%29.aspx) <br/> |Obtém o status de um bloqueio baseado em consulta, que é definido usando a operação **SetHoldOnMailboxes** .  <br/> |
|[Operação GetNonIndexableItemDetails](https://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |[ExchangeService. GetNonIndexableItemDetails ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getnonindexableitemdetails%28v=exchg.80%29.aspx) <br/> |Obtém detalhes sobre os itens que não podem ser indexados. Isso inclui, mas não está limitado a, o identificador de item, um código de erro, uma descrição de erro, quando uma tentativa é feita para indexar o item e informações adicionais sobre o item.  <br/> |
|[Operação GetNonIndexableItemStatistics](https://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |[ExchangeService. GetNonIndexableItemStatistics ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getnonindexableitemstatistics%28v=exchg.80%29.aspx) <br/> |Obtém a contagem de itens que não podem ser indexados em uma caixa de correio.  <br/> |
|[Operação GetSearchableMailboxes](https://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |[ExchangeService. GetSearchableMailboxes ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getsearchablemailboxes%28v=exchg.80%29.aspx) <br/> |Obtém uma lista de caixas de correio nas quais o cliente tem permissão para pesquisar ou executar a descoberta eletrônica.  <br/> |
|[Operação SearchMailboxes](https://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |[ExchangeService. SearchMailboxes ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.searchmailboxes%28v=exchg.80%29.aspx) <br/> |Procura itens em caixas de correio específicas que correspondam a palavras-chave de consulta.  <br/> |
|[Operação SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |[ExchangeService. SetHoldOnMailboxes ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) <br/> |Define um bloqueio baseado em consulta nos itens.  <br/> |

<a name="arch"> </a>

## <a name="archiving-in-ews"></a>Arquivamento no EWS

Caixas de correio de arquivo morto são caixas de correio secundárias associadas a um usuário. As caixas de correio de arquivo morto normalmente são usadas para gerenciar limites de armazenamento de email. Por exemplo, os itens de email mais antigos podem ser movidos periodicamente da caixa de entrada para a caixa de correio de arquivo morto. 
  
O Exchange apresenta duas novas operações do EWS que você pode usar para arquivar um conjunto de itens de email de uma caixa de correio principal. O arquivamento de itens da caixa de entrada dessa forma preserva a hierarquia de pastas dos itens. Além disso, as caixas de correio de arquivo morto agora podem ser armazenadas localmente em um cliente ou remotamente, de modo mais opaco para um usuário, usando um caminho de pasta para apontar para o conteúdo do arquivo morto.
  
**Tabela 3. Operações do EWS e métodos da API gerenciada do EWS para trabalhar com arquivamento**

|**Nome da operação**|**Método de API gerenciada do EWS**|**Descrição**|
|:-----|:-----|:-----|
|[Operação ArchiveItem](https://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |[ExchangeService. ArchiveItems ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.archiveitems%28v=exchg.80%29.aspx) <br/> |Move um item da caixa de correio principal para a caixa de correio de arquivo morto.  <br/> |
|[Operação createfolderpath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |Não implementado.  <br/> |Cria uma hierarquia de pastas em uma caixa de correio primária ou de arquivo morto.  <br/> |

<a name="personas"> </a>

## <a name="personas-in-ews"></a>Pessoas no EWS

Uma *pessoa* é uma coleção de dados associada a um indivíduo. Os dados podem ser provenientes de uma ou mais fontes e associados à persona por meio de uma ID de link comum. As pessoas no EWS permitem que você vincule, pesquise, procure e recupere informações sobre uma pessoa de várias fontes e organize-as em uma única entidade lógica. As pessoas diferem dos contatos em que um contato é uma coleção de dados de uma única fonte associada a um indivíduo; por exemplo, um contato pessoal do Outlook ou uma entrada em uma GAL (lista de endereços global). 
  
A API gerenciada EWS não implementa essa funcionalidade.
  
> [!NOTE]
> O repositório unificado de contatos também expõe a funcionalidade persona por meio das operações que dão suporte a esse recurso. 
  
**Tabela 4. Operações do EWS para trabalhar com pessoas**

|**Nome da operação**|**Descrição**|
|:-----|:-----|
|[Operação FindPeople](https://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |Retorna todos os objetos persona de uma pasta de contatos especificada ou recupera todos os contatos que correspondem a uma cadeia de caracteres de consulta especificada.  <br/> |
|[Operação getpersona](https://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |Recupera um persona.  <br/> |

<a name="unified"> </a>

## <a name="unified-contact-store-in-ews"></a>Repositório unificado de contatos no EWS

O repositório unificado de contatos é um recurso que fornece uma experiência de contato consistente em produtos do Office e atua como um ponto de integração para aplicativos de terceiros usarem o mesmo repositório de contatos. Ele permite que os usuários e aplicativos armazenem, gerenciem e acessem informações de contato e o disponibilizem globalmente entre o Lync, o Exchange 2013, o Outlook, o Outlook Web App e qualquer outro aplicativo que implemente o acesso ao repositório unificado de contatos. O Exchange é o repositório de contatos para a experiência do repositório unificado de contatos. 
  
A API gerenciada EWS não implementa essa funcionalidade.
  
**Tabela 5. Operações do EWS para trabalhar com o repositório unificado de contatos**

|**Nome da operação**|**Descrição**|
|:-----|:-----|
|[Operação AddNewImContactToGroup](https://msdn.microsoft.com/library/0cb5525f-faa3-48f1-9551-df55ffc26f46%28Office.15%29.aspx) <br/> |Adiciona um novo contato de mensagens instantâneas a um grupo. O repositório unificado de contatos pode conter no máximo 1000 contatos.  <br/> |
|[Operação AddImContactToGroup](https://msdn.microsoft.com/library/376acc42-2684-4596-aca1-82a4a10865c9%28Office.15%29.aspx) <br/> |Adiciona um contato de IM existente a um grupo. O repositório unificado de contatos pode conter no máximo 1000 contatos.  <br/> |
|[Operação AddImGroup](https://msdn.microsoft.com/library/6df6e504-b7c8-4773-b10f-ffa5defac229%28Office.15%29.aspx) <br/> |Adiciona um novo grupo de IM. O repositório unificado de contatos pode conter no máximo 64 grupos.  <br/> |
|[Operação AddNewTelUriContactToGroup](https://msdn.microsoft.com/library/c9688ce8-2465-45bb-8bd2-94b32ed4885c%28Office.15%29.aspx) <br/> |Adiciona um novo contato a um grupo com base no número de telefone de um contato.  <br/> |
|[Operação AddDistributionGroupToImList](https://msdn.microsoft.com/library/5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a%28Office.15%29.aspx) <br/> |Adiciona um novo grupo de lista de distribuição. O repositório unificado de contatos pode conter no máximo 64 grupos.  <br/> |
|[Operação GetImItemList](https://msdn.microsoft.com/library/e31d14e1-0c1f-4b69-98b7-157d59c13698%28Office.15%29.aspx) <br/> |Recupera uma lista de grupos de IM e pessoas de contato de mensagens instantâneas.  <br/> |
|[Operação GetImItems](https://msdn.microsoft.com/library/51186691-46d2-4d5c-b8bc-4ee2bb20fbe7%28Office.15%29.aspx) <br/> |Recupera informações sobre os grupos de mensagens instantâneas e as pessoas de contato de mensagens instantâneas especificados.  <br/> |
|[Operação RemoveContactFromImList](https://msdn.microsoft.com/library/28ec96c3-45af-48ff-9f17-718a527dc0ad%28Office.15%29.aspx) <br/> |Remove o contato especificado de todos os grupos de IM.  <br/> |
|[Operação RemoveImContactFromGroup](https://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx) <br/> |Remove um contato de mensagens instantâneas de um grupo.  <br/> |
|[Operação RemoveDistributionGroupFromImList](https://msdn.microsoft.com/library/252bddf2-98b6-4824-b548-2fba2bda5384%28Office.15%29.aspx) <br/> |Remove o grupo de lista de distribuição de IM especificado.  <br/> |
|[Operação RemoveImGroup](https://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx) <br/> |Remove o grupo de mensagens instantâneas especificado.  <br/> |
|[Operação SetImGroup](https://msdn.microsoft.com/library/2d48aa07-8152-4c3d-a519-061253e80174%28Office.15%29.aspx) <br/> |Altera o nome de exibição de um grupo.  <br/> |

<a name="retentionpolicy"> </a>
  
## <a name="retention-policies-in-ews"></a>Políticas de retenção no EWS

As políticas de retenção são políticas usadas no Exchange para agrupar uma ou mais marcas de retenção, para aplicar configurações de retenção a pastas ou itens individuais, como mensagens de email e email de voz, e para aplicar configurações de retenção a uma caixa de correio.
  
O Exchange inclui três tipos de marcas de retenção:
  
- Marcas de política padrão que se aplicam a itens de caixa de correio que não têm nenhum outro tipo de marca de retenção aplicada.
    
- Marcas de política de pasta do sistema aplicadas a pastas padrão, como a caixa de entrada.
    
- Marcas pessoais que um usuário pode aplicar a pastas elas criam ou a itens individuais.
    
Apenas uma política de retenção pode ser atribuída a uma caixa de correio, mas a política pode ter uma ou mais marcas de retenção de vários tipos vinculados a ela. As marcas de retenção podem ser vinculadas ou desvinculadas de uma política de retenção a qualquer momento. O EWS no Exchange expõe uma nova operação, [GetUserRetentionPolicyTags](https://msdn.microsoft.com/library/57c6ff23-5c2c-42ee-824b-5a1b6dafab8c%28Office.15%29.aspx)e a API gerenciada do EWS implementa um novo método, [ExchangeService. GetUserRetentionPolicyTags ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuserretentionpolicytags%28v=exchg.80%29.aspx), que fornece uma lista de todas as marcas que estão vinculadas a uma política de retenção. Você pode definir e recuperar marcas de política de retenção para itens e pastas usando as operações **CreateItem**, **CreateFolder**, **UpdateItem**, **UpdateFolder**, **GetItem**e **GetFolder** . 

<a name="userphoto"> </a>

## <a name="requesting-user-photos"></a>Solicitando fotos do usuário

Você pode solicitar fotos de usuário do servidor Exchange usando uma das duas implementações da [operação GetUserPhoto](https://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx): [REST](how-to-get-user-photos-by-using-ews-in-exchange.md) ou SOAP. O ponto de extremidade REST usa uma solicitação HTTPS padrão **Get** para obter a foto do usuário. O serviço retornará uma foto do usuário armazenada no Exchange ou uma foto dos serviços de domínio do Active Directory (AD DS). 
  
A API gerenciada EWS não implementa essa funcionalidade. No entanto, você pode usar a API gerenciada do EWS para retornar fotos de usuários armazenadas em uma caixa de correio obtendo a foto que está anexada a um contato.

<a name="blocksender"> </a>

## <a name="block-senders-and-mark-email-as-junk-in-ews"></a>Bloquear remetentes e marcar email como lixo eletrônico no EWS

Agora você pode bloquear remetentes e marcar email como lixo eletrônico usando a nova [operação MarkAsJunk](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) no EWS ou o método [ExchangeService. MarkAsJunk ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) na API gerenciada do EWS. 

<a name="ewsmailapps"> </a>

## <a name="mail-apps-for-outlook"></a>Aplicativos de email para Outlook

O EWS agora inclui suporte para o gerenciamento de aplicativos de email para o Outlook. 
  
**Tabela 6. Operações do EWS e métodos da API gerenciada do EWS para trabalhar com aplicativos de email para o Outlook**

|**Nome da operação**|**Método de API gerenciada do EWS**|**Descrição**|
|:-----|:-----|:-----|
|[Operação DisableApp](https://msdn.microsoft.com/library/211731a3-2470-49af-bda3-1ddfc15a8e46%28Office.15%29.aspx) <br/> |[ExchangeService. DisableApp ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.disableapp%28v=exchg.80%29.aspx) <br/> |Desabilita um aplicativo instalado.  <br/> |
|[Operação GetAppManifests](https://msdn.microsoft.com/library/21a4987c-c24d-4a6e-ace4-e81edcda6303%28Office.15%29.aspx) <br/> |[ExchangeService. GetAppManifests ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getappmanifests%28v=exchg.80%29.aspx) <br/> |Obtém os manifestos de aplicativo para uma caixa de correio.  <br/> |
|[Operação GetAppMarketplaceUrl](https://msdn.microsoft.com/library/2c016fc3-0e13-4624-9a5b-d3e84577a860%28Office.15%29.aspx) <br/> |[ExchangeService. GetAppMarketplaceUrl ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getappmarketplaceurl%28v=exchg.80%29.aspx) <br/> |Obtém a URL do Marketplace de aplicativos.  <br/> |
|[Operação GetClientAccessToken](https://msdn.microsoft.com/library/086876cc-e22c-4e89-89f9-19e78af51217%28Office.15%29.aspx) <br/> |[ExchangeService. GetClientAccessToken ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getclientaccesstoken%28v=exchg.80%29.aspx) <br/> |Obtém tokens de acesso para cliente.  <br/> |
|[Operação InstallApp](https://msdn.microsoft.com/library/596eae95-3e78-489a-8bb2-d2dd4a026405%28Office.15%29.aspx) <br/> |[ExchangeService. InstallApp ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.installapp%28v=exchg.80%29.aspx) <br/> |Instala um aplicativo para uma caixa de correio.  <br/> |
|[Operação UninstallApp](https://msdn.microsoft.com/library/7707aa6a-381d-43f7-a454-54f6343ed127%28Office.15%29.aspx) <br/> |[ExchangeService. UninstallApp](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.uninstallapp%28v=exchg.80%29.aspx) <br/> |Desinstala um aplicativo de uma caixa de correio.  <br/> |

<a name="propose"> </a>

## <a name="propose-new-meeting-time"></a>Propor novo horário de reunião

O recurso propor novo horário foi introduzido na versão 15.00.0800.007 do Exchange. Isso permite que os participantes da reunião [proponham novos horários de reunião](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) ao organizador da reunião. 
  
A API gerenciada EWS não implementa essa funcionalidade.
  
## <a name="see-also"></a>Confira também

- [Explorar os recursos da API gerenciada por EWS, EWS e serviços Web no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)
- [Aplicativos de email para Outlook e EWS no Exchange](mail-apps-for-outlook-and-ews-in-exchange.md)
- [Arquivamento no EWS no Exchange](archiving-in-ews-in-exchange.md)
- [Descoberta eletrônica no EWS no Exchange](ediscovery-in-ews-in-exchange.md)
- [Pessoas e contatos no EWS no Exchange](people-and-contacts-in-ews-in-exchange.md)
    

