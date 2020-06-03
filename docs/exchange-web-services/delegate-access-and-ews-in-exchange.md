---
title: Acesso de representante e EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 240d1776-7adc-46cd-9099-88ffeba0a8aa
description: Descubra como usar a API gerenciada do EWS e o EWS no Exchange para fornecer acesso de representante às caixas de correio dos usuários.
localization_priority: Priority
ms.openlocfilehash: 4223d625213a3f71726ec5b8d3f09f9e2e7e7e51
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528451"
---
# <a name="delegate-access-and-ews-in-exchange"></a>Acesso de representante e EWS no Exchange

Descubra como usar a API gerenciada do EWS e o EWS no Exchange para fornecer acesso de representante às caixas de correio dos usuários.
  
Você pode permitir que os usuários acessem caixas de correio de outros usuários de uma destas três maneiras: 
  
- Adicionando delegados e especificando permissões para cada representante.
    
- Modificando as permissões de pasta diretamente.
    
- Usando a representação.
    
As permissões de delegação e de pasta são melhores quando você só concede acesso a alguns usuários, pois você precisa adicionar permissões individualmente a cada caixa de correio. A representação é a melhor opção quando você está lidando com quantidades de caixas de correio, porque você pode facilmente habilitar uma conta de serviço para acessar cada caixa de correio em um banco de dados. A Figura 1 mostra algumas das diferenças entre cada tipo de acesso.
  
**Figura 1. Maneiras de acessar caixas de correio de outros usuários**

![Diagrama que mostra tipos de acesso de caixa de correio, a relação entre proprietários de caixa de correio e o representante para cada tipo e o tipo de permissão. Permissões Enviar em nome de para permissões de delegação e/ou pastas. Permissões Enviar como para representação.](media/Ex15_Delegate_Overview.png)
  
Quando se trata de enviar emails ou agendar reuniões, os representantes podem receber permissões "enviar em nome de", portanto, o destinatário de um email ou uma solicitação de reunião enviada por um representante verá " *delegar* em nome do *proprietário da caixa de correio* " quando receber a solicitação de email ou de reunião no Outlook. Incluir o texto "enviar em nome de" é um detalhe de implementação do cliente e pode ser criado usando os valores "de" e "Sender". O valor "from" indica o proprietário da caixa de correio e o valor "Sender" indica o representante que enviou o email. Se uma conta de serviço representando um usuário enviar um email ou agendar uma reunião para o proprietário da caixa de correio, a mensagem será "enviada como" o proprietário da caixa de correio. Não é possível que o destinatário saiba que o email foi enviado pela conta de serviço. Os usuários que recebem permissões de pasta e não o acesso de representante não podem "enviar como" ou "enviar em nome de" de um proprietário de caixa de correio. Eles têm acesso às pastas da caixa de correio e podem ser capazes de criar itens nas pastas, mas não podem enviar os itens. 
  
Quando é apropriado modificar as permissões de pasta diretamente? Em geral, quando você deseja fornecer um acesso de usuário a uma pasta, mas não deseja conceder as permissões "enviar em nome de" do usuário, quando os requisitos de permissões não mapeiam os valores de enumeração da API gerenciada do EWS [DelegateFolderPermissionLevel](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) ou os valores do elemento do [PermissionLevel](https://msdn.microsoft.com/library/87978600-3523-451e-a725-ef092c543e2a%28Office.15%29.aspx) EWS, ou quando você deseja fornecer acesso de usuário a uma única pasta personalizada. 
  
Se você só precisa modificar as permissões de pasta para atingir sua meta e não precisa adicionar um representante (ou seja, não é necessário ter permissões "enviar em nome de"), confira [definir permissões de pasta para outro usuário usando o EWS no Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md). 

Observe que você também pode usar o [Outlook](https://office.microsoft.com/outlook-help/allow-someone-else-to-manage-your-mail-and-calendar-HA102749417.aspx) ou o [PowerShell do Exchange Server (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) para configurar o acesso de representante. 

  
## <a name="how-does-delegate-access-work"></a>Como o acesso de representante funciona?

O acesso de representante permite que os usuários acessem algumas ou todas as pastas do proprietário da caixa de correio e atue em nome do proprietário da caixa de correio. O proprietário da caixa de correio pode ser um usuário ou um recurso, como uma sala de conferência. Por exemplo, uma recepcionista pode ser concedida permissões de representante para a pasta calendário de uma sala de conferência, para lidar com solicitações de reserva. Você pode usar a API gerenciada do EWS ou o EWS para permitir que o proprietário da caixa de correio ou um administrador adicione um representante, especifique quais pastas o representante pode acessar e, em seguida, especifique permissões para essa pasta. Os representantes podem ter acesso às seguintes pastas: 
  
- Calendário
    
- Tarefas
    
- Caixa de Entrada
    
- Contatos
    
- Observações
    
- Diário
    
Quando um usuário tem acesso de representante a uma ou mais dessas pastas, ele pode criar, obter, atualizar, excluir, copiar e pesquisar itens nessa pasta e em todas as pastas filhas, dependendo das [permissões](#bk_delegateperms) definidas na pasta. A maneira na qual o aplicativo executa essas ações depende se o acesso [explícito](#bk_explicit) ou [implícito](#bk_implicit) é necessário. 
  
## <a name="delegate-permissions"></a>Delegar permissões
<a name="bk_delegateperms"> </a>

Quando um administrador ou proprietário de caixa de correio adiciona um representante a uma caixa de correio, ele também pode definir o nível de permissão para uma ou mais pastas. Se um nível de permissão não for definido para uma pasta, o valor de permissão padrão será nenhum. Vários usuários podem ter o mesmo nível de permissão em uma pasta, e os usuários podem ter diferentes níveis de permissão para pastas diferentes. Se você estiver usando a API gerenciada do EWS, use a propriedade [DelegateUser. Permissions](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegateuser.permissions%28v=exchg.80%29.aspx) , que contém um dos valores de enumeração [DelegateFolderPermissionLevel](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) para cada pasta, para definir permissões de representante em pastas. Se você estiver usando o EWS, use o elemento [DelegatePermissions](https://msdn.microsoft.com/library/292badc7-bab3-4368-9d7c-9a8b7edb279b%28Office.15%29.aspx) para definir permissões de representante e o elemento [PermissionLevel](https://msdn.microsoft.com/library/87978600-3523-451e-a725-ef092c543e2a%28Office.15%29.aspx) para definir o nível de permissão. 
  
**Tabela 2. Delegar níveis de permissão**

|**Nível de permissão**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |Este é o valor padrão para todas as pastas.  <br/> |
|Autor  <br/> |Um representante pode ler e criar itens, e modificar e excluir itens criados por eles. Por exemplo, um representante pode criar solicitações de tarefa e solicitações de reunião diretamente na pasta de tarefas ou calendário do proprietário da caixa de correio e, em seguida, enviar um item no nome do proprietário da caixa de correio.  <br/> |
|Editor  <br/> |Um representante pode fazer tudo o que um autor pode fazer e também modificar e excluir os itens que o proprietário da caixa de correio criou.  <br/> |
|Revisor  <br/> |Um representante pode ler itens; por exemplo, um representante com permissão de revisor pode ler mensagens na caixa de entrada de outra pessoa.  <br/> |
|Personalizado  <br/> |O proprietário da caixa de correio concedeu um conjunto personalizado de permissões para o representante.  <br/> |
   
A propriedade API gerenciada do EWS do [DelgateUser. ViewPrivateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegateuser.viewprivateitems%28v=exchg.80%29.aspx) e o elemento [ViewPrivateItems](https://msdn.microsoft.com/library/80b949ac-440c-4a01-b428-ebafb5b1b802%28Office.15%29.aspx) EWS é uma configuração global que afeta todas as pastas do proprietário da caixa de correio, incluindo todos os emails, contatos, calendário, tarefas, anotações e pastas de diário. Você não pode permitir o acesso a itens privados em apenas uma pasta. 
  
## <a name="explicit-access"></a>Acesso explícito
<a name="bk_explicit"> </a>

Simplificando, o acesso explícito é a forma de entrada para que os representantes executem ações em pastas ou itens de um proprietário de caixa de correio. O acesso explícito é concedido a um representante quando ele inclui o nome de pasta conhecido para uma pasta do proprietário da caixa de correio junto com o endereço SMTP do proprietário da caixa de correio em uma solicitação para o servidor. O acesso é explícito porque a solicitação do representante declara explicitamente que o contexto para o método ou operação é a caixa de correio do proprietário da caixa de correio, e não a caixa de correio do representante.
  
Acesso explícito define o contexto de todos os métodos ou operações executados nas pastas ou itens que estão sendo movidos para frente. Todas as IDs de item e de pasta retornadas quando o acesso explícito é definido exclusivamente como pertencente ao proprietário da caixa de correio (embora não esteja em qualquer formato legível por pessoas). Dessa forma, o aplicativo não precisará especificar o endereço SMTP do proprietário da caixa de correio novamente; o contexto está oculto nos identificadores. Depois que um item ou pasta é identificado, um representante realmente usa [acesso implícito](#bk_implicit) para modificar o item. A figura a seguir mostra o processo de obter acesso explícito e implícito. 
  
**Figura 2. Solicitar acesso explícito e implícito a um item ou pasta**

![Um diagrama que mostra o aplicativo enviando uma solicitação de acesso explícito, uma resposta do servidor e, em seguida, uma solicitação de acesso implícito e uma resposta do servidor.](media/Ex15_Delegate_ExplictImplicit.png)
  
Você pode definir o acesso explícito em vários cenários diferentes. Essencialmente, sempre que você estiver enviando uma ID de pasta em um método ou operação, poderá definir acesso explícito. Isso pode incluir a localização de pastas, a localização de compromissos, a recebimento de itens, a localização de conversas e assim por diante.
  
### <a name="explicit-access-and-the-ews-managed-api"></a>Acesso explícito e a API gerenciada do EWS
<a name="bk_explicitewsma"> </a>

Você pode iniciar o acesso de representante explícito usando qualquer um dos seguintes métodos sobrecarregados que usam um parâmetro de entrada [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) para identificar a pasta de destino: 
  
- [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx)
    
- [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [ExchangeService. FindAppointments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx)
    
- [ExchangeService. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- E muito mais!
    
Você pode usar o parâmetro **FolderId** em cada um destes métodos para identificar a pasta de destino do proprietário da caixa de correio, da seguinte maneira. 
  
```cs
new FolderId(WellKnownFolderName.Calendar, "primary@contoso.com");
```

Por exemplo, para associar à pasta calendário, o **FolderId** neste método **BIND** especifica o nome da pasta bem conhecido e o endereço SMTP do proprietário da caixa de correio. 
  
```cs
CalendarFolder calendar = CalendarFolder.Bind(service, new FolderId(WellKnownFolderName.Calendar, "primary@contoso.com"), new PropertySet());
```

Ao especificar o nome de pasta conhecido e o endereço SMTP, o representante pode associar-se à pasta calendário do proprietário da caixa de correio — obtendo acesso explícito à pasta. Todas as solicitações subsequentes para [acesso implícito](#bk_implicit) a itens na pasta dependem do contexto retornado nas IDs de item e IDs de pasta. Essencialmente, os identificadores contêm o contexto para as chamadas de acesso de representante implícito. Ou, para recuperar a ID do item de um item que atenda a critérios específicos, use o seguinte. 
  
```cs
FindItemsResults<Item> results = service.FindItems(new FolderId(WellKnownFolderName.Calendar, "primary@contoso.com"), filter, view);
```

Nesse caso, a ID do item é retornada e, em seguida, o representante pode usar o acesso implícito para fazer alterações no item usando a ID do item.
  
Não é necessário iniciar o acesso explícito novamente até que você exija uma ID de item ou uma ID de pasta que você não tenha acesso por meio do acesso explícito existente. 
  
### <a name="explicit-access-and-ews"></a>Acesso explícito e EWS
<a name="bk_explicitewsma"> </a>

Você pode iniciar o acesso explícito usando as operações [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx), [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)ou [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) . Essas operações oferecem a opção de usar o elemento [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) para identificar a pasta de destino. O elemento **DistinguishedFolderId** tem um único elemento filho opcional, o elemento [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) . O elemento **Mailbox** , quando usado como um filho do elemento **DistinguishedFolderId** , especifica a caixa de correio para o representante acessar. Se o usuário de chamada tiver permissão para acessar a pasta do proprietário da caixa de correio, a resposta conterá uma coleção de identificadores para itens ou pastas nessa caixa de correio. Os identificadores de item e de pasta retornados na resposta podem ser usados para acesso de representante implícito. 
  
## <a name="implicit-access"></a>Acesso implícito
<a name="bk_implicit"> </a>

O acesso implícito é usado depois que um representante recupera a ID de um item ou pasta na caixa de correio do proprietário da caixa de correio e o representante deseja atualizar, excluir ou copiar o item. Quando o representante usa esse item ou ID de pasta em uma solicitação, as alterações são feitas no item na caixa de correio do proprietário da caixa de correio. O representante não precisa incluir o endereço SMTP do proprietário da caixa de correio. 
  
Por exemplo, quando um representante tem a ID de uma das pastas do proprietário da caixa de correio, o representante pode executar uma operação **FindItem** nessa pasta usando a ID de pasta, sem identificar explicitamente a caixa de correio do proprietário da caixa de correio. Nesse ponto, o representante pode executar ações na pasta do proprietário da caixa de correio usando as IDs que são retornadas nas respostas. 
  
### <a name="implicit-access-and-the-ews-managed-api"></a>Acesso implícito e a API gerenciada do EWS

Se uma ID de item foi recuperada pelo método [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , essa ID de item pode ser usada em uma chamada de método [Item subsequente. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) para associar ao item. Você pode então chamar o método [Item. Update](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx), [Item. Delete](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)ou [Item. Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) — ou qualquer chamada de método que exija uma ID de item, conforme necessário para concluir a tarefa. Contanto que o representante tenha permissões apropriadas para a pasta que contém o item (e, se aplicável, a pasta para a qual o item está se movendo), o representante pode fazer alterações de acordo com seus níveis de permissão. 
  
### <a name="implicit-access-and-ews"></a>Acesso implícito e EWS

Se uma ID de item foi recuperada pela operação [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , essa ID de item pode ser usada em operações subsequentes do [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) para vincular ao item. Você pode então chamar a operação [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx), [DeleteItem](../web-service-reference/deleteitem-operation.md)ou [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) — ou qualquer operação que exija uma ID de item, conforme necessário para concluir a tarefa. Contanto que o representante tenha permissões apropriadas para a pasta que contém o item (e, se aplicável, a pasta para a qual o item está se movendo), o representante pode fazer alterações de acordo com seus níveis de permissão. 
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_implicit"> </a>

- [Adicionar e remover representantes usando o EWS no Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
    
- [Acessar um calendário como um representante usando o EWS no Exchange](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Acessar contatos como um representante usando o EWS no Exchange](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Acessar email como um representante usando o EWS no Exchange](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Definir permissões de pasta para outro usuário usando o EWS no Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
    
- [Como lidar com erros relacionados à delegação no EWS no Exchange](handling-delegation-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)

- [Permitir que outra pessoa Gerencie seu email e calendário](https://office.microsoft.com/outlook-help/allow-someone-else-to-manage-your-mail-and-calendar-HA102749417.aspx)  

- [Add-MailboxPermission](https://technet.microsoft.com/library/bb124097%28v=exchg.150%29.aspx)
    