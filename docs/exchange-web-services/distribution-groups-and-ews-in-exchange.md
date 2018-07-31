---
title: Grupos de distribuição e EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fe08c2e3-92a0-43ec-bc61-69b14caee8fe
description: Saiba mais sobre os diferentes tipos de grupos de distribuição que estão disponíveis no Exchange e como você pode gerenciá-los em sua API gerenciada de EWS ou aplicativos do EWS.
ms.openlocfilehash: 725b02c69f004a58c7216763d3c44f1e9d2df2ab
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353956"
---
# <a name="distribution-groups-and-ews-in-exchange"></a>Grupos de distribuição e EWS no Exchange

Saiba mais sobre os diferentes tipos de grupos de distribuição que estão disponíveis no Exchange e como você pode gerenciá-los em sua API gerenciada de EWS ou aplicativos do EWS.
  
Um grupo de distribuição é uma coleção de endereços de email que estão associados um único endereço de email ou alias. Grupos de distribuição (também chamados de listas de distribuição) habilitar um usuário enviar email a várias pessoas usando um único endereço de destinatário. Porque a associação de grupo de distribuição e, portanto, os destinatários da mensagem, podem ser gerenciados fora de threads de email individuais, os grupos de distribuição fornecem uma excelente maneira de habilitar a distribuição de email para um grupo de usuários. Programaticamente, você pode criar e gerenciar grupos de distribuição usando a API gerenciada de EWS, EWS e o Shell de gerenciamento do Exchange. Antes de começar a programação, vamos explorar os diferentes tipos de grupos de distribuição que estão disponíveis e suas opções para gerenciá-los.
  
## <a name="types-of-distribution-groups"></a>Tipos de grupos de distribuição

O Exchange oferece suporte a três tipos de grupos de distribuição:
  
- [Grupos de distribuição universal](distribution-groups-and-ews-in-exchange.md#bk_DistributionGroup) — objetos de grupo de distribuição universal do Active Directory que são habilitados para email. Grupos de distribuição universal são usados para distribuir mensagens a um grupo de destinatários. 
    
- [Grupos de segurança](distribution-groups-and-ews-in-exchange.md#bk_SecurityGroup) — os objetos do Active Directory que são habilitados para email; também conhecidos como grupos de segurança universais. Grupos de segurança são usados para conceder permissões de acesso a recursos nos serviços de domínio Active Directory (AD DS), bem como para distribuir mensagens. 
    
- [Grupos de contatos](distribution-groups-and-ews-in-exchange.md#bk_ContactGroup) — os grupos de distribuição privada que estão localizados na caixa de correio do usuário. 
    
O tipo de grupo de distribuição que você escolher dependerá de onde você planeja armazenar o grupo de distribuição que irá usá-lo, e o que ele será usado.

<a name="bk_DistributionGroup"> </a>

### <a name="universal-distribution-groups"></a>Grupos de distribuição universal

Você pode usar grupos de distribuição universal para consolidar grupos de destinatários em um único endereço de email ou alias. Como os grupos de distribuição universal são armazenados no AD DS, qualquer pessoa pode usá-los para enviar email, incluindo usuários fora da sua organização. Você pode usar a API gerenciada de EWS ou o EWS para expandir um grupo de distribuição, mas para criar e gerenciar grupos de distribuição, você precisará usar [os cmdlets do Shell de gerenciamento do Exchange](#bk_UsingEMS).
  
Você também pode usar grupos de distribuição universal contenha uma coleção de salas; Por exemplo, para facilitar para os usuários a localizar uma sala de conferência para uma reunião. Os usuários podem adicionar uma lista de salas — um grupo de distribuição universal que contenha caixas de correio de recurso de sala — a uma solicitação de reunião para localizar uma sala disponível sem precisar adicionar cada sala individualmente.
  
Você pode criar um grupo de distribuição universal estática que permanece o mesmo até atualizar a associação, ou você pode criar um grupo dinâmico de distribuição universal. Um grupo dinâmico de distribuição universal consultas objetos habilitados para email do Active Directory e cria a associação de grupo com base nos resultados. A associação ao grupo é recalculada sempre que uma mensagem de email é enviada ao grupo. 

<a name="bk_SecurityGroup"> </a>

### <a name="security-groups"></a>Grupos de segurança

Grupos de distribuição universal e grupos de segurança são idênticos na maioria das formas. No entanto, ao contrário de grupos de distribuição universal, você pode usar grupos de segurança para atribuir permissões a recursos de rede no AD DS. É possível usar a API gerenciada de EWS ou o EWS para criar e gerenciar grupos de segurança; em vez disso, você pode usar [cmdlets do Shell de gerenciamento do Exchange](#bk_UsingEMS). Mas, assim como os grupos de distribuição universal, você pode usar a API gerenciada de EWS ou o EWS para expandir grupos de segurança.

<a name="bk_ContactGroup"> </a>

### <a name="contact-groups"></a>Grupos de contatos

Se você não deseja dar cada acesso administrativo do usuário para o servidor para criar grupos de distribuição, mas você deseja habilitá-los enviar uma única mensagem para um grande conjunto de pessoas, você pode fazer isso usando grupos de contatos. Um grupo de contatos não tem um endereço de email associado a ela e existe apenas na caixa de correio de um usuário. outros usuários não terão acesso a ele. Você pode [usar a API gerenciada de EWS ou o EWS para criar grupos de contatos](how-to-create-contact-groups-by-using-ews-in-exchange.md).
  
## <a name="managing-distribution-groups-by-using-the-ews-managed-api-or-ews"></a>Gerenciando grupos de distribuição usando o EWS Managed API ou o EWS

Você pode usar a API gerenciada de EWS ou o EWS para expandir um grupo de distribuição universal ou o grupo de segurança e controlar a criação e gerenciamento de um grupo de contatos; No entanto, você não pode usar essas tecnologias para criar ou editar os membros desses grupos. 
  
**Tabela 1. Operações de EWS para gerenciar grupos de distribuição e os métodos de API gerenciada de EWS**

|**Método API gerenciada de EWS**|**Operação do EWS**|**Use para …**|
|:-----|:-----|:-----|
|Métodos da [classe ContactGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx)  <br/> |[CreatItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |Crie um grupo de contatos no armazenamento do Exchange.<br/><br/>**Observação**: você não pode criar um grupo de distribuição universal ou grupo de segurança usando a API gerenciada de EWS ou EWS.           |
|[ExpandGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) <br/> |[ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) <br/> |Recuperando uma lista de seus membros, expanda um grupo de distribuição universal, grupo de segurança ou grupo de contatos.  <br/> |
|[FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |Procurar grupos de contatos na caixa de correio.  <br/> |
|[GetRooms](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) <br/> |[GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) <br/> |Recupere uma coleção de todas as salas de uma lista de salas especificado em uma organização. Uma lista de salas é um grupo de distribuição que contém apenas de caixas de correio de recurso de sala.  <br/> |
|[ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |Pesquisar e retornar candidatos possíveis para coincidir com um nome ambíguo. Os candidatos podem ser grupos de distribuição.  <br/> |
   
Você pode usar as informações retornadas pelo método o [ExpandGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) ou a operação [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) para determinar quais tipos de membros no grupo. Os tipos de membro são definidos pela enumeração [MailboxType](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.mailboxtype%28v=exchg.80%29.aspx) EWS Managed API e o elemento do EWS [MailboxType](http://msdn.microsoft.com/library/696e5fdb-d8c5-40f0-9e79-885eae65dfa4%28Office.15%29.aspx) . 
  
**Tabela 2. Tipos de membro do grupo de distribuição**

|**Valor de enumeração MailboxType**|**Valor do elemento MailboxType**|**Descrição**|
|:-----|:-----|:-----|
|Mailbox  <br/> |Mailbox  <br/> |Um objeto do Active Directory habilitado para email.  <br/> |
|PublicGroup  <br/> |PublicDL  <br/> |Um grupo de distribuição contido no grupo que você acabou de ser expandido. Para obter uma lista completa dos membros, expanda também esse grupo.  <br/> |
|ContactGroup  <br/> |PrivateDL  <br/> |Um grupo de contatos que está localizado na caixa de correio e só está disponível para os usuários daquela caixa de correio.  <br/> |
|Contato  <br/> |Contato  <br/> |Um contato de banco de dados do Exchange ou o contato de email do Active Directory.  <br/> |

<a name="bk_UsingEMS"> </a>

## <a name="managing-distribution-groups-by-using-the-exchange-management-shell"></a>Gerenciando grupos de distribuição usando o Shell de gerenciamento do Exchange

Você pode [usar os cmdlets do Shell de gerenciamento do Exchange](http://msdn.microsoft.com/en-us/library/ff326159%28v=exchg.140%29.aspx) para criar e gerenciar grupos de distribuição universal e grupos de segurança em seu código. 
  
> [!NOTE]
> Você não pode usar cmdlets do Shell de gerenciamento do Exchange para gerenciar grupos de contatos. 
  
**Tabela 3. Cmdlets do Shell de gerenciamento do Exchange para trabalhar com grupos de distribuição**

|**Cmdlet**|**Use para …**|
|:-----|:-----|
|[Disable-DistributionGroup](http://technet.microsoft.com/en-us/library/aa997942%28v=exchg.150%29.aspx) <br/> |Remova os recursos de email de um grupo de distribuição habilitado para email.  <br/> |
|[Enable-DistributionGroup](http://technet.microsoft.com/en-us/library/aa998916%28v=exchg.150%29.aspx) <br/> |Ativar o email de um grupo universal existente.  <br/> |
|[Get-DistributionGroup](http://technet.microsoft.com/en-us/library/bb124755%28v=exchg.150%29.aspx) <br/> |Consulta para grupos de distribuição existente.  <br/> |
|[New-DistributionGroup](http://technet.microsoft.com/en-us/library/aa998856%28v=exchg.150%29.aspx) <br/> |Crie um grupo de distribuição.  <br/> |
|[Remove-DistributionGroup](http://technet.microsoft.com/en-us/library/aa997627%28v=exchg.150%29.aspx) <br/> |Exclua um grupo de distribuição existente do AD DS.  <br/> |
|[Set-DistributionGroup](http://technet.microsoft.com/en-us/library/bb124955%28v=exchg.150%29.aspx) <br/> |Modifique as configurações de um grupo de distribuição existente.  <br/> |
|[Adicionar-DistributionGroupMember](http://technet.microsoft.com/en-us/library/bb124340%28v=exchg.150%29.aspx) <br/> |Adicione um destinatário a um grupo de distribuição.  <br/> |
|[Get-DistributionGroupMember](http://technet.microsoft.com/en-us/library/aa996367%28v=exchg.150%29.aspx) <br/> |Localize membros do grupo de distribuição existente.  <br/> |
|[Remove-DistributionGroupMember](http://technet.microsoft.com/en-us/library/aa998016%28v=exchg.150%29.aspx) <br/> |Remova um destinatário existente de um grupo de distribuição.  <br/> |
|[Update-DistributionGroupMember](http://technet.microsoft.com/en-us/library/dd335049%28v=exchg.150%29.aspx) <br/> |Atualize um membro de um grupo de distribuição especificado.  <br/> |
|[Get-DynamicDistributionGroup](http://technet.microsoft.com/en-us/library/bb124762%28v=exchg.150%29.aspx) <br/> |Recupere as configurações em um grupo dinâmico de distribuição existente.  <br/> |
|[New-DynamicDistributionGroup](http://technet.microsoft.com/en-us/library/bb125127%28v=exchg.150%29.aspx) <br/> |Crie um grupo dinâmico de distribuição.  <br/> |
|[Remove-DynamicDistributionGroup](http://technet.microsoft.com/en-us/library/bb125038%28v=exchg.150%29.aspx) <br/> |Exclua um grupo dinâmico de distribuição existente. Este cmdlet Remove o grupo dinâmico de distribuição do AD DS.  <br/> |
|[Set-DynamicDistributionGroup](http://technet.microsoft.com/en-us/library/bb123796%28v=exchg.150%29.aspx) <br/> |Modifique as configurações de um grupo dinâmico de distribuição existente.  <br/> |

<a name="bk_UsingEMS"> </a>

## <a name="in-this-section"></a>Nesta seção

- [Criar grupos de contatos usando o EWS no Exchange](how-to-create-contact-groups-by-using-ews-in-exchange.md)   
- [Expandir grupos de distribuição, usando o EWS no Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    
## <a name="see-also"></a>Confira também

- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)   
- [Cmdlets do Shell de gerenciamento do chamada Exchange do código gerenciado](http://msdn.microsoft.com/en-us/library/ff326159%28v=exchg.140%29.aspx)
    

