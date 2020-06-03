---
title: Grupos de distribuição e EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fe08c2e3-92a0-43ec-bc61-69b14caee8fe
description: Saiba mais sobre os diferentes tipos de grupos de distribuição que estão disponíveis no Exchange e como você pode gerenciá-los na API gerenciada do EWS ou no aplicativo EWS.
ms.openlocfilehash: 083a2c7380e8b9677ddacc9ae3c9465d6a9db97f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528430"
---
# <a name="distribution-groups-and-ews-in-exchange"></a>Grupos de distribuição e EWS no Exchange

Saiba mais sobre os diferentes tipos de grupos de distribuição que estão disponíveis no Exchange e como você pode gerenciá-los na API gerenciada do EWS ou no aplicativo EWS.
  
Um grupo de distribuição é uma coleção de endereços de email que estão associados a um único alias ou endereço de email. Os grupos de distribuição (às vezes também chamados de listas de distribuição) permitem que um usuário envie emails para várias pessoas usando um único endereço de destinatário. Como a associação ao grupo de distribuição e, portanto, os destinatários das mensagens, podem ser gerenciadas fora de segmentos de email individuais, os grupos de distribuição oferecem uma excelente maneira de habilitar a distribuição de emails para um grupo de usuários. Você pode criar e gerenciar grupos de distribuição programaticamente usando a API gerenciada do EWS, o EWS e o Shell de gerenciamento do Exchange. Antes de começar a programação, vamos explorar os diferentes tipos de grupos de distribuição que estão disponíveis e suas opções para gerenciá-los.
  
## <a name="types-of-distribution-groups"></a>Tipos de grupos de distribuição

O Exchange oferece suporte a três tipos de grupos de distribuição:
  
- [Grupos de distribuição universal](distribution-groups-and-ews-in-exchange.md#bk_DistributionGroup) – objetos de grupo de distribuição universal do Active Directory habilitados para email. Grupos de distribuição universal são usados para distribuir mensagens para um grupo de destinatários. 
    
- [Grupos de segurança](distribution-groups-and-ews-in-exchange.md#bk_SecurityGroup) — objetos do Active Directory que são habilitados para email; também conhecido como grupos de segurança universais. Os grupos de segurança são usados para atribuir permissões de acesso a recursos nos serviços de domínio do Active Directory (AD DS), bem como para distribuir mensagens. 
    
- [Grupos de contatos](distribution-groups-and-ews-in-exchange.md#bk_ContactGroup) — grupos de distribuição privada que estão localizados na caixa de correio de um usuário. 
    
O tipo de grupo de distribuição escolhido dependerá de onde você planeja armazenar o grupo de distribuição, quem o usará e o que será usado.

<a name="bk_DistributionGroup"> </a>

### <a name="universal-distribution-groups"></a>Grupos de distribuição universal

Você pode usar grupos de distribuição universal para consolidar grupos de destinatários em um único alias ou endereço de email. Como os grupos de distribuição universal são armazenados no AD DS, qualquer pessoa pode usá-los para enviar emails, incluindo usuários de fora da sua organização. Você pode usar a API gerenciada do EWS ou EWS para expandir um grupo de distribuição, mas para criar e gerenciar grupos de distribuição, será necessário usar os [cmdlets do Shell de gerenciamento do Exchange](#bk_UsingEMS).
  
Você também pode usar grupos de distribuição universal para conter uma coleção de salas; por exemplo, para facilitar para os usuários a localização de uma sala de conferência para uma reunião. Os usuários podem adicionar uma lista de salas — um grupo de distribuição universal que contém caixas de correio de recursos de sala — a uma solicitação de reunião para localizar uma sala disponível sem ter que adicionar cada sala individualmente.
  
Você pode criar um grupo de distribuição universal estático que permanece o mesmo até que você atualize a associação ou pode criar um grupo dinâmico de distribuição universal. Um grupo dinâmico de distribuição universal consulta objetos habilitados para email do Active Directory e cria a associação de grupo com base nos resultados. A associação de grupos é recalculada sempre que uma mensagem de email é enviada ao grupo. 

<a name="bk_SecurityGroup"> </a>

### <a name="security-groups"></a>Grupos de segurança

Grupos de distribuição e grupos de segurança universais são idênticos na maioria das formas. No entanto, ao contrário dos grupos de distribuição universal, você pode usar grupos de segurança para atribuir permissões a recursos de rede no AD DS. Você não pode usar a API gerenciada do EWS ou o EWS para criar e gerenciar grupos de segurança; em vez disso, você usa os [cmdlets do Shell de gerenciamento do Exchange](#bk_UsingEMS). Mas, assim como os grupos de distribuição universal, você pode usar a API gerenciada do EWS ou o EWS para expandir os grupos de segurança.

<a name="bk_ContactGroup"> </a>

### <a name="contact-groups"></a>Grupos de contatos

Se você não deseja conceder a cada usuário acesso administrativo ao servidor para criar grupos de distribuição, mas deseja permitir que eles enviem uma única mensagem para uma grande coleção de pessoas, você pode fazer isso usando grupos de contatos. Um grupo de contatos não tem um endereço de email associado a ele e existe apenas na caixa de correio de um usuário. outros usuários não terão acesso a ele. Você pode [usar a API gerenciada do EWS ou o EWS para criar grupos de contatos](how-to-create-contact-groups-by-using-ews-in-exchange.md).
  
## <a name="managing-distribution-groups-by-using-the-ews-managed-api-or-ews"></a>Gerenciando grupos de distribuição usando a API gerenciada do EWS ou o EWS

Você pode usar a API gerenciada do EWS ou o EWS para expandir um grupo de distribuição universal ou grupo de segurança e para controlar a criação e o gerenciamento de um grupo de contatos; no entanto, você não pode usar essas tecnologias para criar ou editar os membros desses grupos. 
  
**Tabela 1. Métodos da API gerenciada do EWS e operações do EWS para gerenciamento de grupos de distribuição**

|**Método de API gerenciada do EWS**|**Operação do EWS**|**Use para...**|
|:-----|:-----|:-----|
|Métodos de [classe de contato](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx)  <br/> |[CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |Criar um grupo de contatos no repositório do Exchange.<br/><br/>**Observação**: não é possível criar um grupo de distribuição universal ou grupo de segurança usando a API gerenciada do EWS ou o EWS.           |
|[ExpandGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) <br/> |[ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) <br/> |Expanda um grupo de distribuição universal, um grupo de segurança ou um grupo de contatos recuperando uma lista de seus membros.  <br/> |
|[FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |Procurar grupos de contatos na caixa de correio.  <br/> |
|[Getrooms](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) <br/> |[Getrooms](https://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) <br/> |Recupere uma coleção de todas as salas em uma lista de salas especificada em uma organização. Uma lista de salas é um grupo de distribuição que contém apenas caixas de correio de recursos de sala.  <br/> |
|[Resolvedor](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |Procure e retorne possíveis candidatos para corresponder a um nome ambíguo. Os candidatos podem ser grupos de distribuição.  <br/> |
   
Você pode usar as informações retornadas pelo método [Expand](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) ou a operação [ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) para determinar quais tipos de membros estão no grupo. Os tipos de membro são definidos pela enumeração API gerenciada do EWS da [caixa de correio](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.mailboxtype%28v=exchg.80%29.aspx) e o elemento [MailboxType](https://msdn.microsoft.com/library/696e5fdb-d8c5-40f0-9e79-885eae65dfa4%28Office.15%29.aspx) EWS. 
  
**Tabela 2. Tipos de membro do grupo de distribuição**

|**Valor de enumeração MailboxType**|**Valor do elemento MailboxType**|**Descrição**|
|:-----|:-----|:-----|
|Caixa de correio  <br/> |Caixa de correio  <br/> |Um objeto do Active Directory habilitado para email.  <br/> |
|Public  <br/> |PublicDL  <br/> |Um grupo de distribuição contido no grupo que você acabou de expandir. Para obter uma lista completa de membros, expanda também esse grupo.  <br/> |
|Contato  <br/> |PrivateDL  <br/> |Um grupo de contatos localizado na caixa de correio e só está disponível para usuários dessa caixa de correio.  <br/> |
|Contato  <br/> |Contato  <br/> |Um contato de banco de dados do Exchange ou contato de email do Active Directory.  <br/> |

<a name="bk_UsingEMS"> </a>

## <a name="managing-distribution-groups-by-using-the-exchange-management-shell"></a>Gerenciando grupos de distribuição usando o Shell de gerenciamento do Exchange

Você pode [usar os cmdlets do Shell de gerenciamento do Exchange](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx) para criar e gerenciar grupos de distribuição universais e grupos de segurança no seu código. 
  
> [!NOTE]
> Você não pode usar os cmdlets do Shell de gerenciamento do Exchange para gerenciar grupos de contatos. 
  
**Tabela 3. Cmdlets do Shell de gerenciamento do Exchange para trabalhar com grupos de distribuição**

|**Cmdlet**|**Use para...**|
|:-----|:-----|
|[Disable-Distribution](https://technet.microsoft.com/library/aa997942%28v=exchg.150%29.aspx) <br/> |Remova os recursos de email de um grupo de distribuição habilitado para email.  <br/> |
|[Enable-Distribution](https://technet.microsoft.com/library/aa998916%28v=exchg.150%29.aspx) <br/> |Habilitar um grupo universal existente para email.  <br/> |
|[Get-Distribution](https://technet.microsoft.com/library/bb124755%28v=exchg.150%29.aspx) <br/> |Consultar grupos de distribuição existentes.  <br/> |
|[New-Distribution](https://technet.microsoft.com/library/aa998856%28v=exchg.150%29.aspx) <br/> |Criar um grupo de distribuição.  <br/> |
|[Remove-the Distribution](https://technet.microsoft.com/library/aa997627%28v=exchg.150%29.aspx) <br/> |Excluir um grupo de distribuição existente do AD DS.  <br/> |
|[Set-grupo de distribuição](https://technet.microsoft.com/library/bb124955%28v=exchg.150%29.aspx) <br/> |Modificar as configurações de um grupo de distribuição existente.  <br/> |
|[Add-DistributionGroupMember](https://technet.microsoft.com/library/bb124340%28v=exchg.150%29.aspx) <br/> |Adicionar um destinatário a um grupo de distribuição.  <br/> |
|[Get-DistributionGroupMember](https://technet.microsoft.com/library/aa996367%28v=exchg.150%29.aspx) <br/> |Localizar membros existentes do grupo de distribuição.  <br/> |
|[Remove-DistributionGroupMember](https://technet.microsoft.com/library/aa998016%28v=exchg.150%29.aspx) <br/> |Remover um destinatário existente de um grupo de distribuição.  <br/> |
|[Update-DistributionGroupMember](https://technet.microsoft.com/library/dd335049%28v=exchg.150%29.aspx) <br/> |Atualizar um membro de um grupo de distribuição especificado.  <br/> |
|[Get-DynamicDistributionGroup](https://technet.microsoft.com/library/bb124762%28v=exchg.150%29.aspx) <br/> |Recupere as configurações em um grupo dinâmico de distribuição existente.  <br/> |
|[New-DynamicDistributionGroup](https://technet.microsoft.com/library/bb125127%28v=exchg.150%29.aspx) <br/> |Criar um grupo dinâmico de distribuição.  <br/> |
|[Remove-DynamicDistributionGroup](https://technet.microsoft.com/library/bb125038%28v=exchg.150%29.aspx) <br/> |Excluir um grupo dinâmico de distribuição existente. Este cmdlet Remove o grupo dinâmico de distribuição do AD DS.  <br/> |
|[Set-DynamicDistributionGroup](https://technet.microsoft.com/library/bb123796%28v=exchg.150%29.aspx) <br/> |Modificar as configurações de um grupo dinâmico de distribuição existente.  <br/> |

<a name="bk_UsingEMS"> </a>

## <a name="in-this-section"></a>Nesta seção

- [Criar grupos de contatos usando o EWS no Exchange](how-to-create-contact-groups-by-using-ews-in-exchange.md)   
- [Expandir grupos de distribuição usando EWS no Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    
## <a name="see-also"></a>Confira também

- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)   
- [Chamar os cmdlets do Shell de gerenciamento do Exchange a partir do código gerenciado](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx)
    

