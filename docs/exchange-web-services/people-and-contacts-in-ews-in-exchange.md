---
title: Pessoas e contatos no EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 043c33be-a0d1-4bad-a840-85715eda4813
description: Saiba mais sobre personas, o repositório unificado de contatos e como trabalhar com contatos usando a API gerenciada do EWS ou o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: f0590a0d8a99b8320cc1b316829177e05e443de6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457667"
---
# <a name="people-and-contacts-in-ews-in-exchange"></a>Pessoas e contatos no EWS no Exchange

Saiba mais sobre personas, o repositório unificado de contatos e como trabalhar com contatos usando a API gerenciada do EWS ou o EWS no Exchange. 
  
Os contatos são itens no Exchange que armazenam informações sobre um indivíduo, grupo ou organização. Os contatos podem incluir nomes e endereços de email e outras informações, incluindo endereços de mensagens instantâneas, endereços físicos, aniversários, informações da família e uma foto ou imagem que representa o contato.
  
As informações de contato são armazenadas em um dos dois locais:
  
- Active Directory Domain Services (AD DS), se o contato estiver dentro da organização.
    
- A pasta contatos ou outra pasta na caixa de correio de um usuário, se o contato estiver fora da organização.
    
Vários itens de contato podem representar uma única pessoa. O Exchange usa personas para ajudar a trazer esses diferentes itens de contato juntos. Uma *pessoa* é uma agregação de informações de contato para a mesma pessoa de fontes diferentes. Além das informações de contato no Exchange, as pessoas também podem ser agregadas das informações no cache de destinatários da caixa de correio, uma pasta oculta para contatos de mensagens instantâneas chamadas QuickContacts e de fontes de dados de terceiros. O repositório unificado de contatos no Exchange permite que clientes de mensagens instantâneas usem essa agregação; a única diferença é que o repositório unificado de contatos não agrega informações do AD DS, conforme mostrado na Figura 1. 
  
**Figura 1. Fontes de informações de contato para pessoas e para o repositório unificado de contatos**

![Imagem que mostra as fontes que são agregadas em personas em comparação com as fontes que são incluídas no Repositório de Contatos Unificado. O Repositório de Contatos Unificado não agrega informações de contato do serviço de diretório.](media/EX15_PersonaOverview.png)
  
**Tabela 1. Métodos da API gerenciada do EWS e operações do EWS para trabalhar com contatos**

|**Se você quiser...**|**Usar este método de API gerenciada do EWS**|**Use esta operação do EWS**|
|:-----|:-----|:-----|
|Criar um novo contato  <br/> |Criar uma instância de um novo objeto de [contato](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) e usar [Contact. Save](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) <br/> |
|Copiar um contato  <br/> |[Contato. Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.copy%28v=exchg.80%29.aspx) <br/> |[CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|Mover um contato  <br/> |[Contato. move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.move%28v=exchg.80%29.aspx) <br/> |[MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|Atualizar um contato existente  <br/> |[Contact. bind](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) e [Contact. Update](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.update%28v=exchg.80%29.aspx) <br/> |[UpdateItem](https://msdn.microsoft.com/library/298fdd71-a83d-4407-9728-4f0a8e2d857c%28Office.15%29.aspx) <br/> |
|Excluir um contato  <br/> |[Contact. bind](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) e [Contact. Delete](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.delete%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
|Pesquisar um contato  <br/> |[ExchangeService. FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
|Pesquisar pessoas  <br/> |N/A  <br/> |[FindPeople](https://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |
|Expandir um grupo de distribuição  <br/> |[ExchangeService. Expand](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) <br/> |[ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) <br/> |
|Resolver um nome ambíguo  <br/> |[ExchangeService. ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |
|Obter uma pessoa  <br/> |N/A  <br/> |[Getpersona](https://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |
|Trabalhar com fotos de contato  <br/> |[Contact. SetContactPicture](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.setcontactpicture%28v=exchg.80%29.aspx), [Contact. GetContactPictureAttachment](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.getcontactpictureattachment%28v=exchg.80%29.aspx)ou [Contact. RemoveContactPicture](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.setcontactpicture%28v=exchg.80%29.aspx) <br/> |[GetUserPhoto](https://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) ou [GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/> |
   
## <a name="personas"></a>Personas
<a name="PEOPLESEARCH"> </a>

Até recentemente, os contatos geralmente eram armazenados em um único local, geralmente, em um cliente de email. Hoje, é mais comum armazenar contatos em vários locais diferentes, como em um telefone, em um site de rede social, em uma pasta de contatos em uma caixa de correio do Exchange ou em um serviço de diretório da organização. Com a proliferação de informações de contato, é possível que vários contatos que representem a mesma pessoa contenham informações diferentes; por exemplo, um contato pode incluir um número de telefone comercial e outro número de telefone pessoal, ou um contato armazenado em uma pasta de contatos pode ter um nome diferente do contato para a mesma pessoa que está armazenada em seu telefone.
  
No Exchange Online, no Exchange Online como parte do Office 365 e nas versões locais do Exchange a partir do Exchange 2013, os contatos de fontes diferentes que representam a mesma pessoa estão associados, de maneira semelhante à forma como as mensagens de email são agregadas às conversas, por meio de uma ID de link comum. Quando informações de contato agregadas são retornadas por um servidor Exchange, ela inclui um conjunto de atributos para cada contato, como uma pasta de origem, um nome de exibição, uma ID e uma ID de origem. A soma das propriedades e dos atributos retornados é conhecida como uma pessoa e o conjunto de propriedades retornado é referido como a [forma da pessoa](https://msdn.microsoft.com/library/61d87cd5-3270-40d1-bab7-d0d5bf938607%28Office.15%29.aspx).
  
Como as informações que compõem uma pessoa não são armazenadas em um único local e as informações podem ser alteradas a qualquer momento, uma pessoa só é criada quando você faz uma solicitação a um servidor do Exchange. Você usa a operação [FindPeople](https://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) EWS para fazer uma solicitação de pesquisa persona. Sua solicitação pode incluir uma ordem de classificação e pode ser filtrada de acordo com uma cadeia de caracteres de consulta para ajudá-lo a encontrar a ordenação e filtragem dos resultados. Por exemplo, você pode recuperar o nome de exibição e um conjunto de todos os endereços de email associados a um contato específico da pasta contatos, de uma conta do hotmail, de uma conta do LinkedIn e do serviço de diretório de uma empresa ou você pode recuperar um conjunto de todas as pessoas que têm endereços de mensagens instantâneas. A vinculação de contatos em personas é automática com base em um algoritmo que reconhece uma relação entre os contatos armazenados em vários dispositivos. 
  
> [!NOTE]
> A API gerenciada EWS não implementa essa funcionalidade. 
  
**Tabela 2. Operações do EWS para trabalhar com pessoas**

|**Nome da operação**|**Descrição**|
|:-----|:-----|
|[FindPeople](https://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |Retorna todas as personas disponíveis a partir de uma pasta de contatos especificada ou recupera contatos que correspondem a uma cadeia de caracteres de consulta especificada.  <br/> |
|[Getpersona](https://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |Retorna um conjunto de propriedades associadas a um persona específico, como todos os endereços de mensagens instantâneas ou nomes de exibição de uma ID persona especificada.  <br/> |
   
Você pode usar as operações **Getpersona** e **FindPeople** para recuperar com eficiência informações de contato de várias fontes. Como todos os itens relacionados a uma pessoa estão associados a um ID de link, você pode usar essas operações em uma ampla variedade de aplicativos que usam dados de contato. Estes são alguns exemplos: 
  
- Um aplicativo de telefone celular que usa a operação **Getpersonum** quando um usuário chama um contato e oferece números de telefone adicionais para chamar, se não houver uma resposta. 
    
- Um aplicativo que usa a operação **FindPeople** para verificar mensagens de caixa de entrada para endereços de email a fim de determinar se eles são encontrados em um persona existente. Os endereços que ainda não estão associados a um persona podem ser usados para criar clientes potenciais de vendas ou listar todas as comunicações recentes com a pessoa representada por esse persona. 
    
- [Um aplicativo de email para o Outlook](mail-apps-for-outlook-and-ews-in-exchange.md) que oferece Saudações diferentes com base em se a correspondência é formal ou informal. As saudações formais são fornecidas pelos nomes de exibição do serviço de diretório e de saudações informais provenientes do nome de exibição originado em contatos da rede social. 
    
## <a name="unified-contact-store"></a>Armazenamento de Contato Unificado
<a name="PEOPLESEARCH"> </a>

As pessoas não estão limitadas a um cliente de email. Se você estiver desenvolvendo um cliente de mensagens instantâneas, poderá fazer a si mesmo qualquer um ou todos os seguintes itens:
  
- Como posso provisionar aplicativos cliente do Lync com um conjunto padrão de itens de contato de IM?
    
- Como faço para gerenciar o contato IM e as listas de grupo?
    
- Como gerenciar o acesso de cliente do Lync personalizado para contatos de mensagens instantâneas e grupos de mensagens instantâneas?
    
O repositório unificado de contatos funciona em segundo plano no Exchange para agregar dados de contato do Exchange e de outras fontes em uma única entidade, ou persona. Embora as operações do EWS que você usa para acessar o repositório unificado de contatos sejam específicas para contatos de mensagens instantâneas, você pode usar o repositório unificado de contatos no Exchange para trabalhar com pessoas em todos os tipos de aplicativos. Tenha em mente que o repositório unificado de contatos não pode acessar dados de contato do AD DS.
  
Os contatos de mensagens instantâneas são armazenados em uma pasta oculta chamada QuickContacts. Você pode usar as operações **AddNewImContactToGroup** e **AddImContactToGroup** para adicionar contatos a grupos armazenados nessa pasta oculta. E, como você pode usar o repositório unificado de contatos para agrupar contatos de mensagens instantâneas, é possível acessar e atualizar grupos de contatos com mais facilidade. 
  
> [!NOTE]
> A API gerenciada EWS não implementa essa funcionalidade. 
  
**Tabela 3. Operações do EWS para acessar o repositório unificado de contatos**

|**Nome da operação**|**Descrição**|
|:-----|:-----|
|[AddNewImContactToGroup](https://msdn.microsoft.com/library/0cb5525f-faa3-48f1-9551-df55ffc26f46%28Office.15%29.aspx) <br/> |Adiciona um novo contato de mensagens instantâneas a um grupo de mensagens instantâneas, até um máximo de 1000 contatos.  <br/> |
|[AddImContactToGroup](https://msdn.microsoft.com/library/376acc42-2684-4596-aca1-82a4a10865c9%28Office.15%29.aspx) <br/> |Adiciona um contato de IM existente a um grupo de mensagens instantâneas, até um máximo de 1000 contatos.  <br/> |
|[AddImGroup](https://msdn.microsoft.com/library/6df6e504-b7c8-4773-b10f-ffa5defac229%28Office.15%29.aspx) <br/> |Adiciona um novo grupo de mensagens instantâneas, até um máximo de 64 grupos.  <br/> |
|[AddDistributionGroupToImList](https://msdn.microsoft.com/library/5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a%28Office.15%29.aspx) <br/> |Adiciona um novo grupo de distribuição a um grupo de mensagens instantâneas, até um máximo de 64 grupos.  <br/> |
|[GetImItemList](https://msdn.microsoft.com/library/e31d14e1-0c1f-4b69-98b7-157d59c13698%28Office.15%29.aspx) <br/> |Recupera uma lista de grupos de IM e pessoas de contato de mensagens instantâneas.  <br/> |
|[GetImItems](https://msdn.microsoft.com/library/51186691-46d2-4d5c-b8bc-4ee2bb20fbe7%28Office.15%29.aspx) <br/> |Recupera informações sobre grupos de mensagens instantâneas específicos e pessoas de contato de mensagens instantâneas.  <br/> |
|[RemoveContactFromImList](https://msdn.microsoft.com/library/28ec96c3-45af-48ff-9f17-718a527dc0ad%28Office.15%29.aspx) <br/> |Remove um contato de um grupo de mensagens instantâneas.  <br/> |
|[RemoveImContactFromGroup](https://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx) <br/> |Remove um contato de mensagens instantâneas de um grupo de mensagens instantâneas.  <br/> |
|[RemoveDistributionGroupFromImList](https://msdn.microsoft.com/library/252bddf2-98b6-4824-b548-2fba2bda5384%28Office.15%29.aspx) <br/> |Remove um grupo de distribuição de um grupo de mensagens instantâneas.  <br/> |
|[RemoveImGroup](https://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx) <br/> |Remove um grupo de mensagens instantâneas.  <br/> |
|[SetImGroup](https://msdn.microsoft.com/library/2d48aa07-8152-4c3d-a519-061253e80174%28Office.15%29.aspx) <br/> |Altera o nome de exibição de um grupo de mensagens instantâneas.  <br/> |
   
## <a name="in-this-section"></a>Nesta seção
<a name="PEOPLESEARCH"> </a>

- [Processar contatos em lotes usando o EWS no Exchange](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    
- [Resolver nomes ambíguos usando o EWS no Exchange 2013](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    
- [Obter fotos do usuário usando o EWS no Exchange](how-to-get-user-photos-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também
<a name="PEOPLESEARCH"> </a>

- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
    
- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)
    

