---
title: Grupos de distribuição e EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: fe08c2e3-92a0-43ec-bc61-69b14caee8fe
description: Saiba mais sobre os diferentes tipos de grupos de distribuição disponíveis no Exchange e como gerenciá-los em sua API Gerenciada EWS ou aplicativo EWS.
ms.openlocfilehash: 71dc1a1e4c71310943eb19f8a5d6b3f470ab7ccb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512300"
---
# <a name="distribution-groups-and-ews-in-exchange"></a>Grupos de distribuição e EWS no Exchange

Saiba mais sobre os diferentes tipos de grupos de distribuição disponíveis no Exchange e como gerenciá-los em sua API Gerenciada EWS ou aplicativo EWS.
  
Um grupo de distribuição é uma coleção de endereços de email associados a um único alias ou endereço de email. Grupos de distribuição (também chamados de listas de distribuição) permitem que um usuário envie emails para várias pessoas usando um único endereço de destinatário. Como a associação ao grupo de distribuição e, portanto, os destinatários da mensagem podem ser gerenciadas fora de threads de email individuais, os grupos de distribuição fornecem uma excelente maneira de habilitar a distribuição de emails para um grupo de usuários. Você pode criar e gerenciar grupos de distribuição programaticamente usando a API Gerenciada do EWS, o EWS e o Shell de Gerenciamento Exchange EWS. Antes de começar a programar, vamos explorar os diferentes tipos de grupos de distribuição disponíveis e suas opções para gerende-los.
  
## <a name="types-of-distribution-groups"></a>Tipos de grupos de distribuição

Exchange suporta três tipos de grupos de distribuição:
  
- [Grupos de distribuição universais](distribution-groups-and-ews-in-exchange.md#bk_DistributionGroup) — objetos de grupo de distribuição universal do Active Directory habilitados para email. Os grupos de distribuição universais são usados para distribuir mensagens para um grupo de destinatários. 
    
- [Grupos de segurança](distribution-groups-and-ews-in-exchange.md#bk_SecurityGroup) — objetos do Active Directory habilitados para email; também conhecidos como grupos de segurança universais. Os grupos de segurança são usados para atribuir permissões de acesso a recursos nos Serviços de Domínio do Active Directory (AD DS), bem como para distribuir mensagens. 
    
- [Grupos de contatos](distribution-groups-and-ews-in-exchange.md#bk_ContactGroup) — Grupos de distribuição privados localizados na caixa de correio de um usuário. 
    
O tipo de grupo de distribuição escolhido dependerá de onde você planeja armazenar o grupo de distribuição, quem o usará e para o que ele será usado.

<a name="bk_DistributionGroup"> </a>

### <a name="universal-distribution-groups"></a>Grupos de distribuição universais

Você pode usar grupos de distribuição universais para consolidar grupos de destinatários em um único alias ou endereço de email. Como os grupos de distribuição universais são armazenados no AD DS, qualquer pessoa pode usá-los para enviar emails, incluindo usuários de fora da sua organização. Você pode usar a API Gerenciada do EWS ou o EWS para expandir um grupo de distribuição, mas para criar e gerenciar grupos de distribuição, você precisará usar [cmdlets](#bk_UsingEMS)do Shell de Gerenciamento Exchange .
  
Você também pode usar grupos de distribuição universais para conter uma coleção de salas; por exemplo, para facilitar que os usuários encontrem uma sala de conferência para uma reunião. Os usuários podem adicionar uma lista de sala — um grupo de distribuição universal que contém caixas de correio de recursos de sala — a uma solicitação de reunião para encontrar uma sala disponível sem precisar adicionar cada sala individualmente.
  
Você pode criar um grupo de distribuição universal estático que permanece o mesmo até atualizar a associação ou criar um grupo dinâmico de distribuição universal. Um grupo de distribuição universal dinâmico consulta objetos habilitados para email do Active Directory e cria a associação de grupo com base nos resultados. A associação de grupos é recalculada sempre que uma mensagem de email é enviada ao grupo. 

<a name="bk_SecurityGroup"> </a>

### <a name="security-groups"></a>Grupos de segurança

Grupos de distribuição universais e grupos de segurança são idênticos na maioria das maneiras. No entanto, diferentemente dos grupos de distribuição universais, você pode usar grupos de segurança para atribuir permissões aos recursos de rede no AD DS. Não é possível usar a API Gerenciada do EWS ou o EWS para criar e gerenciar grupos de segurança; em vez disso, você [Exchange cmdlets do Shell de Gerenciamento.](#bk_UsingEMS) Mas, assim como os grupos de distribuição universais, você pode usar a API Gerenciada EWS ou o EWS para expandir grupos de segurança.

<a name="bk_ContactGroup"> </a>

### <a name="contact-groups"></a>Grupos de contatos

Se você não quiser dar a cada usuário acesso administrativo ao servidor para criar grupos de distribuição, mas quiser permitir que eles enviem uma única mensagem para uma grande coleção de pessoas, você pode fazer isso usando grupos de contatos. Um grupo de contatos não tem um endereço de email associado a ele e existe apenas na caixa de correio de um usuário; outros usuários não terão acesso a ele. Você pode [usar a API Gerenciada do EWS ou o EWS para criar grupos de contatos.](how-to-create-contact-groups-by-using-ews-in-exchange.md)
  
## <a name="managing-distribution-groups-by-using-the-ews-managed-api-or-ews"></a>Gerenciando grupos de distribuição usando a API Gerenciada do EWS ou o EWS

Você pode usar a API Gerenciada do EWS ou o EWS para expandir um grupo de distribuição universal ou um grupo de segurança e controlar a criação e o gerenciamento de um grupo de contatos; no entanto, você não pode usar essas tecnologias para criar ou editar os membros desses grupos. 
  
**Tabela 1. Métodos de API Gerenciada EWS e operações EWS para gerenciar grupos de distribuição**

|**Método da API Gerenciada do EWS**|**Operação do EWS**|**Use para...**|
|:-----|:-----|:-----|
|[Métodos de classe ContactGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx)  <br/> |[CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |Crie um grupo de contatos no Exchange store.<br/><br/>**OBSERVAÇÃO**: Não é possível criar um grupo de distribuição universal ou um grupo de segurança usando a API Gerenciada do EWS ou o EWS.           |
|[ExpandGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) <br/> |[ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) <br/> |Expanda um grupo de distribuição universal, grupo de segurança ou grupo de contatos recuperando uma lista de seus membros.  <br/> |
|[FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |Procure grupos de contatos na caixa de correio.  <br/> |
|[GetRooms](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) <br/> |[GetRooms](https://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) <br/> |Recupere uma coleção de todas as salas em uma lista de salas especificada em uma organização. Uma lista de sala é um grupo de distribuição que contém apenas caixas de correio de recursos de sala.  <br/> |
|[ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |Pesquise e retorne possíveis candidatos para corresponder a um nome ambíguo. Os candidatos podem ser grupos de distribuição.  <br/> |
   
Você pode usar as informações retornadas pelo [método ExpandGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) ou pela operação [ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) para determinar quais tipos de membros estão no grupo. Os tipos de membros são definidos pela enumeração de API Gerenciada [mailboxType](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.mailboxtype%28v=exchg.80%29.aspx) EWS e o [elemento MailboxType](https://msdn.microsoft.com/library/696e5fdb-d8c5-40f0-9e79-885eae65dfa4%28Office.15%29.aspx) EWS. 
  
**Tabela 2. Tipos de membros do grupo de distribuição**

|**Valor da enumeração MailboxType**|**Valor do elemento MailboxType**|**Descrição**|
|:-----|:-----|:-----|
|Mailbox  <br/> |Mailbox  <br/> |Um objeto Active Directory habilitado para email.  <br/> |
|PublicGroup  <br/> |PublicDL  <br/> |Um grupo de distribuição contido no grupo que você acabou de expandir. Para obter uma lista completa de membros, expanda esse grupo também.  <br/> |
|ContactGroup  <br/> |PrivateDL  <br/> |Um grupo de contatos que está localizado na caixa de correio e está disponível apenas para usuários dessa caixa de correio.  <br/> |
|Contact  <br/> |Contact  <br/> |Um contato Exchange banco de dados ou contato de email do Active Directory.  <br/> |

<a name="bk_UsingEMS"> </a>

## <a name="managing-distribution-groups-by-using-the-exchange-management-shell"></a>Gerenciando grupos de distribuição usando o Shell Exchange Gerenciamento

Você pode [usar Exchange cmdlets](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx) do Shell de Gerenciamento para criar e gerenciar grupos universais de distribuição e grupos de segurança em seu código. 
  
> [!NOTE]
> Não é possível usar Exchange cmdlets do Shell de Gerenciamento para gerenciar grupos de contatos. 
  
**Tabela 3. Exchange Cmdlets do Shell de Gerenciamento para trabalhar com grupos de distribuição**

|**Cmdlet**|**Use para...**|
|:-----|:-----|
|[Disable-DistributionGroup](https://technet.microsoft.com/library/aa997942%28v=exchg.150%29.aspx) <br/> |Remova os recursos de email de um grupo de distribuição habilitado para email.  <br/> |
|[Enable-DistributionGroup](https://technet.microsoft.com/library/aa998916%28v=exchg.150%29.aspx) <br/> |Habilitação de email para um grupo universal existente.  <br/> |
|[Get-DistributionGroup](https://technet.microsoft.com/library/bb124755%28v=exchg.150%29.aspx) <br/> |Consulta para grupos de distribuição existentes.  <br/> |
|[New-DistributionGroup](https://technet.microsoft.com/library/aa998856%28v=exchg.150%29.aspx) <br/> |Criar um grupo de distribuição.  <br/> |
|[Remove-DistributionGroup](https://technet.microsoft.com/library/aa997627%28v=exchg.150%29.aspx) <br/> |Exclua um grupo de distribuição existente do AD DS.  <br/> |
|[Set-DistributionGroup](https://technet.microsoft.com/library/bb124955%28v=exchg.150%29.aspx) <br/> |Modifique as configurações de um grupo de distribuição existente.  <br/> |
|[Add-DistributionGroupMember](https://technet.microsoft.com/library/bb124340%28v=exchg.150%29.aspx) <br/> |Adicione um destinatário a um grupo de distribuição.  <br/> |
|[Get-DistributionGroupMember](https://technet.microsoft.com/library/aa996367%28v=exchg.150%29.aspx) <br/> |Encontre membros do grupo de distribuição existentes.  <br/> |
|[Remove-DistributionGroupMember](https://technet.microsoft.com/library/aa998016%28v=exchg.150%29.aspx) <br/> |Remova um destinatário existente de um grupo de distribuição.  <br/> |
|[Update-DistributionGroupMember](https://technet.microsoft.com/library/dd335049%28v=exchg.150%29.aspx) <br/> |Atualize um membro de um grupo de distribuição especificado.  <br/> |
|[Get-DynamicDistributionGroup](https://technet.microsoft.com/library/bb124762%28v=exchg.150%29.aspx) <br/> |Recupere as configurações em um grupo de distribuição dinâmico existente.  <br/> |
|[New-DynamicDistributionGroup](https://technet.microsoft.com/library/bb125127%28v=exchg.150%29.aspx) <br/> |Crie um grupo dinâmico de distribuição.  <br/> |
|[Remove-DynamicDistributionGroup](https://technet.microsoft.com/library/bb125038%28v=exchg.150%29.aspx) <br/> |Exclua um grupo de distribuição dinâmico existente. Este cmdlet remove o grupo dinâmico de distribuição do AD DS.  <br/> |
|[Set-DynamicDistributionGroup](https://technet.microsoft.com/library/bb123796%28v=exchg.150%29.aspx) <br/> |Modifique as configurações de um grupo de distribuição dinâmico existente.  <br/> |

<a name="bk_UsingEMS"> </a>

## <a name="in-this-section"></a>Nesta seção

- [Criar grupos de contatos usando o EWS em Exchange](how-to-create-contact-groups-by-using-ews-in-exchange.md)   
- [Expandir grupos de distribuição usando o EWS no Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    
## <a name="see-also"></a>Confira também

- [Desenvolver clientes do serviço Web para o Exchange](develop-web-service-clients-for-exchange.md)   
- [Chamando Exchange Cmdlets do Shell de Gerenciamento do Código Gerenciado](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx)
    

