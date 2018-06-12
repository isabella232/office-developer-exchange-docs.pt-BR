---
title: O que há de novo no EWS e outros serviços da web do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: aff6328f-cff1-42a6-9a4d-ea4d2d0461cf
description: Descubra quais são as novidades nos serviços da web e do EWS no Exchange e o EWS Managed API.
ms.openlocfilehash: 9e848babc96707152be767f42b561a587fc6cff0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750965"
---
# <a name="whats-new-in-ews-and-other-web-services-in-exchange"></a>O que há de novo no EWS e outros serviços da web do Exchange

Descubra quais são as novidades nos serviços da web e do EWS no Exchange e o EWS Managed API.
  
Serviços Web no Exchange foram atualizados para incluir os novos recursos. 
  
**Tabela 1. Novo serviço web recursos no Exchange Online, Exchange 2013 e a API gerenciada de EWS**

|Recurso|Implementado no Exchange Online|Implementado no Exchange 2013|Implementada na API gerenciada de EWS|
|:-----|:-----:|:-----:|:-----:|
|[descoberta eletrônica](#eDisc) <br/> |Sim  <br/> |Sim  <br/> |Sim  <br/> |
|[Arquivamento](#arch) <br/> |Sim  <br/> |Sim  <br/> |Sim  <br/> |
|[Personagens](#personas) <br/> |Sim  <br/> |Sim  <br/> |Não  <br/> |
|[Repositório unificado de contatos](#unified) <br/> |Sim  <br/> |Sim  <br/> |Não  <br/> |
|[Políticas de retenção](#retentionpolicy) <br/> |Sim  <br/> |Sim  <br/> |Sim  <br/> |
|[Fotos dos usuários](#userphoto) <br/> |Sim  <br/> |Sim  <br/> |Não  <br/> |
|[Aplicativos de email para o gerenciamento do Outlook](#ewsmailapps) <br/> |Sim  <br/> |Sim  <br/> |Sim  <br/> |
|[Propor novo horário de reunião](#propose) <br/> |Sim  <br/> |Não  <br/> |Não  <br/> |

<a name="eDisc"> </a>

## <a name="ediscovery-in-ews"></a>descoberta eletrônica no EWS

descoberta eletrônica é um serviço web de consulta federados que permite que aplicativos externos, como o SharePoint 2013, executar consultas de dados do Exchange. Descoberta consiste em várias fases, incluindo identificando e preservar dados de chave, remoção para baixo e revisar os dados e produzindo dados no tribunal. consultas do eDiscovery facilitam o processo de descoberta, fornecendo um fluxo de trabalho de descoberta único entre Exchange e SharePoint.
  
**Tabela 2. Operações do EWS e métodos de API gerenciada de EWS para trabalhar com a descoberta eletrônica**

|**Nome da operação**|**Método API gerenciada de EWS**|**Descrição**|
|:-----|:-----|:-----|
|[Operação GetDiscoverySearchConfiguration](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |[ExchangeService.GetDiscoverySearchConfiguration()](http://msdn.microsoft.com/en-us/library/jj670206%28v=exchg.80%29.aspx) <br/> |Obtém informações de configuração de bloqueio in-loco, salvo pesquisas de descoberta e as caixas de correio que estão habilitadas para pesquisa de descoberta.  <br/> |
|[Operação GetHoldOnMailboxes](http://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |[ExchangeService.GetHoldOnMailboxes()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getholdonmailboxes%28v=exchg.80%29.aspx) <br/> |Obtém o status de uma isenção baseado em consulta, que é definido usando a operação **SetHoldOnMailboxes** .  <br/> |
|[Operação GetNonIndexableItemDetails](http://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |[ExchangeService.GetNonIndexableItemDetails()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getnonindexableitemdetails%28v=exchg.80%29.aspx) <br/> |Obtém os detalhes sobre os itens que não podem ser indexados. Isso inclui, mas não está limitado a, o identificador do item, um código de erro, uma descrição do erro, quando foi feita uma tentativa para indexar o item e informações adicionais sobre o item.  <br/> |
|[Operação GetNonIndexableItemStatistics](http://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |[ExchangeService.GetNonIndexableItemStatistics()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getnonindexableitemstatistics%28v=exchg.80%29.aspx) <br/> |Obtém a contagem de itens que não podem ser indexados em uma caixa de correio.  <br/> |
|[Operação GetSearchableMailboxes](http://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |[ExchangeService.GetSearchableMailboxes()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getsearchablemailboxes%28v=exchg.80%29.aspx) <br/> |Obtém uma lista de caixas de correio que o cliente tem permissão para pesquisar ou executar a descoberta eletrônica.  <br/> |
|[Operação SearchMailboxes](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |[ExchangeService.SearchMailboxes()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.searchmailboxes%28v=exchg.80%29.aspx) <br/> |Procura por itens em caixas de correio específicas que coincidem com palavras-chave de consulta.  <br/> |
|[Operação SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |[ExchangeService.SetHoldOnMailboxes()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) <br/> |Define uma consulta com base em espera em itens.  <br/> |

<a name="arch"> </a>

## <a name="archiving-in-ews"></a>Arquivamento no EWS

Caixas de correio de arquivo morto são secundárias caixas de correio que estão associadas um usuário. Caixas de correio de arquivo morto são geralmente usadas para gerenciar os limites de armazenamento de email. Por exemplo, itens de email mais antigos periodicamente talvez seja movidos de caixa de entrada para a caixa de correio de arquivo morto. 
  
Exchange introduz duas novas operações de EWS que você pode usar para arquivar um conjunto de itens de email de uma caixa de correio principal. Arquivamento de itens de caixa de entrada dessa maneira preserva a hierarquia de pastas dos itens. Além disso, as caixas de correio de arquivo morto agora podem ser armazenadas localmente em um cliente, ou remotamente, de forma que é opaca a um usuário, principalmente por meio de um caminho de pasta para apontar para o conteúdo do arquivamento.
  
**Tabela 3. Operações do EWS e métodos de API gerenciada de EWS para trabalhar com o arquivamento**

|**Nome da operação**|**Método API gerenciada de EWS**|**Descrição**|
|:-----|:-----|:-----|
|[Operação ArchiveItem](http://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |[ExchangeService.ArchiveItems()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.archiveitems%28v=exchg.80%29.aspx) <br/> |Move um item da caixa de correio principal para a caixa de correio de arquivo morto.  <br/> |
|[Operação CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |Não foi implementado.  <br/> |Cria uma hierarquia de pastas no primário ou a caixa de correio de arquivo morto.  <br/> |

<a name="personas"> </a>

## <a name="personas-in-ews"></a>Personagens no EWS

Uma *pessoa* é uma coleção de dados que é associados a um indivíduo. Os dados podem ser provenientes de uma ou mais fontes e associado com a pessoa por meio de uma ID de link comuns. Personagens no EWS permitem vincular, pesquise, navegue e recuperar informações sobre uma pessoa de várias fontes e organizar essas informações em uma única entidade lógica. Personagens diferem dos contatos que um contato é um conjunto de dados de uma única fonte que está associado um indivíduo; Por exemplo, um contato pessoal no Outlook ou uma entrada em uma lista de endereços global (GAL). 
  
A API gerenciada EWS não implementa essa funcionalidade.
  
> [!NOTE]
> O repositório unificado de contatos também expõe a funcionalidade de pessoa por meio das operações que suportam esse recurso. 
  
**Tabela 4. Operações do EWS para trabalhar com personagens**

|**Nome da operação**|**Descrição**|
|:-----|:-----|
|[Operação FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |Retorna todos os objetos de pessoa de uma pasta de contato especificada ou recupera todos os contatos que correspondem a uma cadeia de caracteres de consulta especificada.  <br/> |
|[Operação GetPersona](http://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |Recupera uma pessoa.  <br/> |

<a name="unified"> </a>

## <a name="unified-contact-store-in-ews"></a>Repositório unificado de contatos no EWS

O repositório unificado de contatos é um recurso que fornece uma experiência consistente de contato nos produtos do Office e atua como um ponto de integração para aplicativos de terceiros para usar o mesmo armazenamento de contato. Ele permite que os usuários e aplicativos armazenar, gerenciar e acessar informações de contato e disponibilizá-lo globalmente entre o Lync, Exchange 2013, Outlook, Outlook Web App e qualquer outro aplicativo que implementa o acesso ao repositório unificado de contatos. O Exchange é o repositório de contatos para a experiência do repositório unificado de contatos. 
  
A API gerenciada EWS não implementa essa funcionalidade.
  
**Tabela 5. Operações do EWS para trabalhar com o repositório unificado de contatos**

|**Nome da operação**|**Descrição**|
|:-----|:-----|
|[Operação AddNewImContactToGroup](http://msdn.microsoft.com/library/0cb5525f-faa3-48f1-9551-df55ffc26f46%28Office.15%29.aspx) <br/> |Adiciona um novo contato de mensagem Instantânea a um grupo. O repositório unificado de contatos pode conter um máximo de contatos de 1000.  <br/> |
|[Operação AddImContactToGroup](http://msdn.microsoft.com/library/376acc42-2684-4596-aca1-82a4a10865c9%28Office.15%29.aspx) <br/> |Adiciona um contato de mensagens Instantâneas existente a um grupo. O repositório unificado de contatos pode conter um máximo de contatos de 1000.  <br/> |
|[Operação AddImGroup](http://msdn.microsoft.com/library/6df6e504-b7c8-4773-b10f-ffa5defac229%28Office.15%29.aspx) <br/> |Adiciona um novo grupo de mensagens Instantâneas. O repositório unificado de contatos pode conter um máximo de 64 grupos.  <br/> |
|[Operação AddNewTelUriContactToGroup](http://msdn.microsoft.com/library/c9688ce8-2465-45bb-8bd2-94b32ed4885c%28Office.15%29.aspx) <br/> |Adiciona um novo contato a um grupo com base no número de telefone do contato.  <br/> |
|[Operação AddDistributionGroupToImList](http://msdn.microsoft.com/library/5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a%28Office.15%29.aspx) <br/> |Adiciona um novo grupo de lista de distribuição. O repositório unificado de contatos pode conter um máximo de 64 grupos.  <br/> |
|[Operação GetImItemList](http://msdn.microsoft.com/library/e31d14e1-0c1f-4b69-98b7-157d59c13698%28Office.15%29.aspx) <br/> |Recupera uma lista de grupos de mensagens Instantâneas e personagens contatos de mensagens Instantâneas.  <br/> |
|[Operação GetImItems](http://msdn.microsoft.com/library/51186691-46d2-4d5c-b8bc-4ee2bb20fbe7%28Office.15%29.aspx) <br/> |Recupera informações sobre os grupos especificados de mensagens Instantâneas e personagens contatos de mensagens Instantâneas.  <br/> |
|[Operação RemoveContactFromImList](http://msdn.microsoft.com/library/28ec96c3-45af-48ff-9f17-718a527dc0ad%28Office.15%29.aspx) <br/> |Remove o contato especificado de todos os grupos de mensagens Instantâneas.  <br/> |
|[Operação RemoveImContactFromGroup](http://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx) <br/> |Remove um contato de mensagens Instantâneas de um grupo.  <br/> |
|[Operação RemoveDistributionGroupFromImList](http://msdn.microsoft.com/library/252bddf2-98b6-4824-b548-2fba2bda5384%28Office.15%29.aspx) <br/> |Remove o grupo de lista de distribuição de mensagens Instantâneas especificado.  <br/> |
|[Operação RemoveImGroup](http://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx) <br/> |Remove o grupo de mensagens Instantâneas especificado.  <br/> |
|[Operação SetImGroup](http://msdn.microsoft.com/library/2d48aa07-8152-4c3d-a519-061253e80174%28Office.15%29.aspx) <br/> |Altera o nome de exibição de um grupo.  <br/> |

<a name="retentionpolicy"> </a>
  
## <a name="retention-policies-in-ews"></a>Políticas de retenção no EWS

Políticas de retenção são diretivas que são usadas no Exchange ao grupo de um ou mais marcas de retenção, para aplicar configurações de retenção para pastas individuais ou itens, tais como mensagens de email de voz e email e para aplicar configurações de retenção a uma caixa de correio.
  
Exchange inclui três tipos de marcas de retenção:
  
- Marcas de diretiva padrão que se aplicam a itens de caixa de correio que não tenham nenhum outro tipo de marca de retenção aplicada.
    
- Sistema pasta marcas de diretiva que são aplicadas às pastas padrão, como a caixa de entrada.
    
- Marcas pessoais que um usuário pode aplicar às pastas que eles criam ou para itens individuais.
    
Política de retenção de apenas um pode ser atribuída a uma caixa de correio, mas a diretiva pode ter um ou mais marcas de retenção dos vários tipos vinculadas a ela. Marcas de retenção podem ser vinculadas à ou desligadas de uma política de retenção a qualquer momento. EWS no Exchange expõe uma nova operação, [GetUserRetentionPolicyTags](http://msdn.microsoft.com/library/57c6ff23-5c2c-42ee-824b-5a1b6dafab8c%28Office.15%29.aspx), e a API gerenciada de EWS implementa um novo método, [ExchangeService.GetUserRetentionPolicyTags()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getuserretentionpolicytags%28v=exchg.80%29.aspx), que fornece uma lista de todas as marcas que são vinculados a uma política de retenção. Você pode definir e recuperar marcas de política de retenção para itens e pastas usando o **CreateItem**, **CreateFolder**, **UpdateItem**, **UpdateFolder**, **GetItem**e **GetFolder** operações. 

<a name="userphoto"> </a>

## <a name="requesting-user-photos"></a>Solicitando fotos dos usuários

Você pode solicitar fotos dos usuários do Exchange server usando uma das duas implementações da [operação GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx): [REST](how-to-get-user-photos-by-using-ews-in-exchange.md) ou SOAP. O ponto de extremidade do REST utiliza uma solicitação HTTPS **GET** padrão para obter a foto do usuário. O serviço seja retornará uma foto de usuário armazenada no Exchange ou uma foto dos serviços de domínio Active Directory (AD DS). 
  
A API gerenciada EWS não implementa essa funcionalidade. No entanto, você pode, usar a API gerenciada de EWS para retornar as fotos de usuário que são armazenadas em uma caixa de correio Obtendo a foto que está anexada a um contato.

<a name="blocksender"> </a>

## <a name="block-senders-and-mark-email-as-junk-in-ews"></a>Bloquear remetentes e marcar o email como lixo eletrônico no EWS

Agora você pode bloquear remetentes e marcar o email como lixo eletrônico usando a [operação MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) de novo no EWS ou o método [ExchangeService.MarkAsJunk()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) na API gerenciada do EWS. 

<a name="ewsmailapps"> </a>

## <a name="mail-apps-for-outlook"></a>Aplicativos de email para Outlook

EWS agora inclui suporte ao gerenciamento de aplicativos de email para Outlook. 
  
**Tabela 6. Operações do EWS e métodos de API gerenciada de EWS para trabalhar com aplicativos de email para Outlook**

|**Nome da operação**|**Método API gerenciada de EWS**|**Descrição**|
|:-----|:-----|:-----|
|[Operação DisableApp](http://msdn.microsoft.com/library/211731a3-2470-49af-bda3-1ddfc15a8e46%28Office.15%29.aspx) <br/> |[ExchangeService.DisableApp()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.disableapp%28v=exchg.80%29.aspx) <br/> |Desabilita um aplicativo instalado.  <br/> |
|[Operação GetAppManifests](http://msdn.microsoft.com/library/21a4987c-c24d-4a6e-ace4-e81edcda6303%28Office.15%29.aspx) <br/> |[ExchangeService.GetAppManifests()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getappmanifests%28v=exchg.80%29.aspx) <br/> |Obtém os manifestos de aplicativos para uma caixa de correio.  <br/> |
|[Operação GetAppMarketplaceUrl](http://msdn.microsoft.com/library/2c016fc3-0e13-4624-9a5b-d3e84577a860%28Office.15%29.aspx) <br/> |[ExchangeService.GetAppMarketplaceUrl()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getappmarketplaceurl%28v=exchg.80%29.aspx) <br/> |Obtém a URL do aplicativo marketplace.  <br/> |
|[Operação GetClientAccessToken](http://msdn.microsoft.com/library/086876cc-e22c-4e89-89f9-19e78af51217%28Office.15%29.aspx) <br/> |[ExchangeService.GetClientAccessToken()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getclientaccesstoken%28v=exchg.80%29.aspx) <br/> |Obtém os tokens de acesso de cliente.  <br/> |
|[Operação InstallApp](http://msdn.microsoft.com/library/596eae95-3e78-489a-8bb2-d2dd4a026405%28Office.15%29.aspx) <br/> |[ExchangeService.InstallApp()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.installapp%28v=exchg.80%29.aspx) <br/> |Instala um aplicativo para uma caixa de correio.  <br/> |
|[Operação UninstallApp](http://msdn.microsoft.com/library/7707aa6a-381d-43f7-a454-54f6343ed127%28Office.15%29.aspx) <br/> |[ExchangeService.UninstallApp](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.uninstallapp%28v=exchg.80%29.aspx) <br/> |Desinstala um aplicativo de uma caixa de correio.  <br/> |

<a name="propose"> </a>

## <a name="propose-new-meeting-time"></a>Propor novo horário de reunião

O novo recurso de tempo do propor foi introduzido no 15.00.0800.007 de versão do Exchange. Isso permite que os participantes [proponham novos horários](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) ao organizador da reunião. 
  
A API gerenciada EWS não implementa essa funcionalidade.
  
## <a name="see-also"></a>Confira também

- [Explorar a API Gerenciada pelo EWS, EWS e serviços Web no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md)
- [Aplicativos de email para o Outlook e o EWS no Exchange](mail-apps-for-outlook-and-ews-in-exchange.md)
- [Arquivamento no EWS no Exchange](archiving-in-ews-in-exchange.md)
- [eDiscovery do EWS no Exchange](ediscovery-in-ews-in-exchange.md)
- [Pessoas e contatos no EWS no Exchange](people-and-contacts-in-ews-in-exchange.md)
    

