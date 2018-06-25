---
title: Acesso de representante e EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 240d1776-7adc-46cd-9099-88ffeba0a8aa
description: Descubra como usar a API gerenciada de EWS e EWS no Exchange para fornecer acesso de representante para caixas de correio dos usuários.
ms.openlocfilehash: 0416ed1889a7c235a35cb49290d39d3ccfc28c49
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750664"
---
# <a name="delegate-access-and-ews-in-exchange"></a>Acesso de representante e EWS no Exchange

Descubra como usar a API gerenciada de EWS e EWS no Exchange para fornecer acesso de representante para caixas de correio dos usuários.
  
Você pode permitir que os usuários acessem caixas de correio de outros usuários em uma destas três formas: 
  
- Adicionando representantes e especificando permissões para cada delegado.
    
- Modificando permissões da pasta diretamente.
    
- Usando representação.
    
Permissões de pasta e delegação são recomendadas quando somente você está concedendo acesso para alguns usuários, porque você precisou para adicionar permissões individualmente para cada caixa de correio. Representação é a melhor escolha quando você está lidando com as quantidades de caixas de correio, pois você pode facilmente habilitar uma conta de serviço acessar cada caixa de correio em um banco de dados. A Figura 1 mostra algumas das diferenças entre cada tipo de acesso.
  
**Figura 1. Maneiras de acessar caixas de correio de outros usuários**

![Diagrama que mostra tipos de acesso de caixa de correio, a relação entre proprietários de caixa de correio e o representante para cada tipo e o tipo de permissão. Permissões Enviar em nome de para permissões de delegação e/ou pastas. Permissões Enviar como para representação.](media/Ex15_Delegate_Overview.png)
  
Quando se trata de enviar um email ou agendar reuniões, delegados podem receber permissões "Enviar em nome de", para que o destinatário de um email ou uma solicitação de reunião que foi enviada por um representante veja " *Delegar* em nome do *proprietário da caixa de correio* " quando eles receiv f a solicitação de reunião ou de email no Outlook. Incluindo o texto "Enviar em nome de" é um detalhe da implementação de cliente - e podem ser criado usando o "from" e "remetente" valores. O valor "de" indica o proprietário da caixa de correio e o valor de "remetente" indica que o delegado que enviou um email. Se uma conta de serviço representando um usuário envia um email ou agenda uma reunião para o proprietário da caixa de correio, a mensagem é "enviada como" o proprietário da caixa de correio. Não há um meio para o destinatário saber que o email foi enviado pela conta de serviço. Os usuários que são concedidos com permissões de pasta e não o acesso de representante não são capazes de "Enviar como" ou "Enviar em nome de" de um proprietário de caixa de correio. Eles têm acesso às pastas de caixa de correio e podem ser capazes de criar itens nas pastas, mas não podem enviar os itens. 
  
Quando ele é adequado modificar as permissões da pasta diretamente? Em geral, quando você deseja fornecer um acesso de usuário para uma pasta, mas não deseja conceder ao usuário permissões "Enviar em nome de", quando seus requisitos de permissões não forem mapeados para os valores de enumeração [DelegateFolderPermissionLevel](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) EWS Managed API ou o [PermissionLevel](http://msdn.microsoft.com/library/87978600-3523-451e-a725-ef092c543e2a%28Office.15%29.aspx) Valores de elemento do EWS, ou quando você deseja fornecer um acesso de usuário para uma única pasta personalizada. 
  
Se você precisar modificar permissões de pasta para atingir seu objetivo e não é necessário adicionar um representante (ou seja, se você não precisará permissões "Enviar em nome de"), consulte [definir permissões da pasta para outro usuário usando o EWS no Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md). 
  
Observe que você também pode usar [o Outlook](http://office.microsoft.com/en-us/outlook-help/allow-someone-else-to-manage-your-mail-and-calendar-HA102749417.aspx) ou o [Exchange Server PowerShell (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) para configurar o acesso de representante. 
  
## <a name="how-does-delegate-access-work"></a>Como delegar acesso trabalho?

Acesso de representante permite que os usuários acessem algumas ou todas as pastas do proprietário da caixa de correio e agir em nome do proprietário da caixa de correio. O proprietário da caixa de correio pode ser um usuário ou um recurso, como uma sala de conferência. Por exemplo, um recepcionista pode receber permissões de representante à pasta de calendário de uma sala de conferência, lidar com as solicitações de reserva. Você pode usar a API gerenciada de EWS ou o EWS para permitir que o proprietário da caixa de correio ou um administrador adicione um representante, especifique quais pastas delegado pode acessar e especifique permissões para essa pasta. Os representantes podem conceder acesso às seguintes pastas: 
  
- Calendário
    
- Tarefas
    
- Caixa de Entrada
    
- Contatos
    
- Observações
    
- Diário
    
Quando um usuário tem acesso de representante a uma ou mais dessas pastas, eles podem criar, obter, atualizar, excluir, copiar e procurar itens na pasta e todas as pastas filho, dependendo das [permissões](#bk_delegateperms) definidas na pasta. A maneira na qual o aplicativo executa essas ações depende se é necessário acesso de [explícitas](#bk_explicit) ou [implícitas](#bk_implicit) . 
  
## <a name="delegate-permissions"></a>Delegar permissões
<a name="bk_delegateperms"> </a>

Quando um administrador ou o proprietário da caixa de correio adiciona um representante para uma caixa de correio, eles também podem definir o nível de permissão para uma ou mais pastas. Se um nível de permissão não estiver definido para uma pasta, o valor de permissão padrão como nenhum. Vários usuários podem ter o mesmo nível de permissão em uma pasta e os usuários podem ter diferentes níveis de permissão para pastas diferentes. Se você estiver usando o EWS Managed API, use a propriedade [DelegateUser.Permissions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.delegateuser.permissions%28v=exchg.80%29.aspx) , que contém um dos valores de enumeração [DelegateFolderPermissionLevel](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) para cada pasta, para definir permissões de representante em pastas. Se você estiver usando o EWS, use o elemento [DelegatePermissions](http://msdn.microsoft.com/library/292badc7-bab3-4368-9d7c-9a8b7edb279b%28Office.15%29.aspx) para definir permissões de representante e o elemento de [PermissionLevel](http://msdn.microsoft.com/library/87978600-3523-451e-a725-ef092c543e2a%28Office.15%29.aspx) para definir o nível de permissão. 
  
**Tabela 2. Níveis de permissão de representante**

|**Nível de permissão**|**Descrição**|
|:-----|:-----|
|None  <br/> |Este é o valor padrão para todas as pastas.  <br/> |
|Autor  <br/> |Um representante pode ler e criar itens, modificar e excluir itens que criam por eles. Por exemplo, um representante pode criar solicitações de tarefa e solicitações de reunião diretamente na pasta de calendário ou de tarefa do proprietário da caixa de correio e, em seguida, enviar esses itens em nome do proprietário da caixa de correio.  <br/> |
|Editor  <br/> |Um representante pode fazer tudo um autor pode fazer e também modificar e excluir os itens que o proprietário da caixa de correio criado.  <br/> |
|Reviewer  <br/> |Um representante pode ler itens; Por exemplo, um representante com essa permissão pode ler mensagens na caixa de entrada de outra pessoa.  <br/> |
|Personalizado  <br/> |O proprietário da caixa de correio tiver concedido a um conjunto de permissões personalizado ao delegado.  <br/> |
   
A propriedade [DelgateUser.ViewPrivateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.delegateuser.viewprivateitems%28v=exchg.80%29.aspx) EWS Managed API e o elemento do EWS [ViewPrivateItems](http://msdn.microsoft.com/library/80b949ac-440c-4a01-b428-ebafb5b1b802%28Office.15%29.aspx) é uma configuração global que afeta pastas de todas as caixas de correio do proprietário, incluindo todos os email, contatos, calendário, tarefas, notas e pastas de diário. Você não pode permitir o acesso aos itens particulares no apenas uma pasta. 
  
## <a name="explicit-access"></a>Acesso explícitos
<a name="bk_explicit"> </a>

Acesso explícito simplesmente colocar é a maneira de entrada para os representantes para executar ações em itens ou pastas de um proprietário de caixa de correio. Acesso explícitos recebe a um delegado quando eles incluem o nome da pasta conhecido para a pasta do proprietário de uma caixa de correio, juntamente com o endereço de SMTP do proprietário da caixa de correio em uma solicitação ao servidor. O acesso é explícito porque a solicitação do representante explicitamente afirma que o contexto para o método ou a operação é a caixa de correio do proprietário da caixa de correio e não caixa de correio do representante.
  
Acesso explícitos define o contexto de todos os métodos ou operações executadas em pastas ou itens no futuro. Todas as identificações de item e pasta retornadas quando o acesso explícitos é definido exclusivamente se identificam como pertencentes ao proprietário da caixa de correio (embora não em qualquer formato legíveis humano). Dessa forma, o aplicativo não precisa especificar o endereço de SMTP do proprietário da caixa de correio repetidamente; o contexto fica oculto nos identificadores. Depois que um item ou pasta for identificada, um representante realmente usa [acesso implícito](#bk_implicit) para modificar o item. A figura a seguir mostra o processo de obtenção de acesso explícito e implícito. 
  
**Figura 2. Solicitando acesso explícito e implícito para um item ou pasta**

![Um diagrama que mostra o aplicativo enviando uma solicitação de acesso explícito, uma resposta do servidor e, em seguida, uma solicitação de acesso implícito e uma resposta do servidor.](media/Ex15_Delegate_ExplictImplicit.png)
  
Você pode definir o acesso explícitos em diversos cenários. Basicamente, sempre que você está enviando um ID de pasta em um método ou a operação, você pode definir acesso explícitos. Isso pode incluir a localização de pastas, Localizando compromissos, obtendo itens, localizar conversas e assim por diante.
  
### <a name="explicit-access-and-the-ews-managed-api"></a>Acesso explícito e a API gerenciada de EWS
<a name="bk_explicitewsma"> </a>

É possível iniciar o acesso de representante explícitas usando qualquer um dos seguintes métodos sobrecarregados que recebem um parâmetro de entrada [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) para identificar a pasta de destino: 
  
- [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx)
    
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx)
    
- [ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- E muito mais!
    
Você pode usar o parâmetro **FolderId** em cada um desses métodos para identificar a pasta de destino do proprietário da caixa de correio, da seguinte maneira. 
  
```cs
new FolderId(WellKnownFolderName.Calendar, "primary@contoso.com");
```

Por exemplo, para associar a pasta de calendário, o **FolderId** neste método **vincular** Especifica o nome da pasta conhecido e endereço de SMTP do proprietário da caixa de correio. 
  
```cs
CalendarFolder calendar = CalendarFolder.Bind(service, new FolderId(WellKnownFolderName.Calendar, "primary@contoso.com"), new PropertySet());
```

Especificando o nome da pasta conhecido e o endereço SMTP, o representante pode vincular a pasta de calendário do proprietário da caixa de correio — ganhando explícito acesso à pasta. Todas as solicitações subsequentes para [acesso implícito](#bk_implicit) a itens na pasta depois contam com o contexto retornado no item identificações e pasta. Basicamente, os identificadores contêm o contexto para as chamadas de acesso de representante implícitas. Ou, para recuperar a ID de item de um item que atenda a critérios específicos, use o seguinte. 
  
```cs
FindItemsResults<Item> results = service.FindItems(new FolderId(WellKnownFolderName.Calendar, "primary@contoso.com"), filter, view);
```

Nesse caso a ID do item é retornada e, em seguida, o representante pode use acesso implícito para fazer alterações no item usando a ID do item.
  
Você não precisa iniciar acesso explícitos novamente até que você precise de uma ID de item ou uma ID de pasta que não podem ser acessados via o acesso explícitos existente. 
  
### <a name="explicit-access-and-ews"></a>Acesso explícitos e EWS
<a name="bk_explicitewsma"> </a>

Você pode iniciar o acesso explícitos usando as operações [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx), [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)ou [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) . Essas operações fornecem a opção de usar o elemento [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) para identificar a pasta de destino. O elemento **DistinguishedFolderId** tem um elemento filho opcionais único, o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) . O elemento de **caixa de correio** , quando usado como um filho do elemento **DistinguishedFolderId** , especifica o representante acessar a caixa de correio. Se o usuário chamador tiver permissão para acessar a pasta do proprietário da caixa de correio, a resposta conterá uma coleção de identificadores aos itens ou pastas nessa caixa de correio. Os identificadores de item e pasta que são retornados na resposta podem ser usados para acesso de representante implícita. 
  
## <a name="implicit-access"></a>Acesso implícito
<a name="bk_implicit"> </a>

Acesso implícito é usado depois que um representante recuperou a ID de um item ou a pasta na caixa de correio do proprietário da caixa de correio e o delegado deseja atualizar, excluir ou copiar o item. Quando o delegado usa esse ID de item ou uma pasta em uma solicitação, as alterações são feitas para o item da caixa de correio do proprietário da caixa de correio. O representante não precisa incluir o endereço de SMTP do proprietário da caixa de correio. 
  
Por exemplo, quando um delegado tem a identificação de uma das pastas do proprietário da caixa de correio, o delegado pode executar uma operação **FindItem** dessa pasta usando o ID de pasta, sem explicitamente que identifica a caixa de correio do proprietário da caixa de correio. Nesse momento, o representante pode executar ações na pasta do proprietário da caixa de correio usando os IDs que são retornados nas respostas. 
  
### <a name="implicit-access-and-the-ews-managed-api"></a>Acesso implícito e a API gerenciada de EWS

Se uma ID de item foi recuperada pelo método [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , a ID do item que pode ser usada em uma chamada de método [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) subsequente para vincular ao item. Você pode chamar o método [Item.Update](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx), [item](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)ou [Item.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) — ou qualquer chamada de método que requer uma ID de item — conforme necessário para concluir a tarefa. Desde que o delegado tem permissões apropriadas para a pasta que contém o item (e, se aplicável, a pasta o item está mudando para), o representante pode fazer alterações de acordo com seus níveis de permissão. 
  
### <a name="implicit-access-and-ews"></a>Acesso implícito e EWS

Se uma ID de item foi recuperada pela operação de [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , a ID do item que pode ser usada em operações de [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) subsequentes para vincular ao item. Você pode chamar a operação [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx), [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)ou [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) — ou qualquer operação que exija uma ID de item — conforme necessário para concluir a tarefa. Desde que o delegado tem permissões apropriadas para a pasta que contém o item (e, se aplicável, a pasta o item está mudando para), o representante pode fazer alterações de acordo com seus níveis de permissão. 
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_implicit"> </a>

- [Adicionar e remover representantes usando o EWS no Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
    
- [Acessar um calendário como um representante, usando o EWS no Exchange](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Contatos de acesso como um representante, usando o EWS no Exchange](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Email de acesso como um representante, usando o EWS no Exchange](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Definir permissões de pasta para outro usuário usando o EWS no Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
    
- [Tratando erros relacionados a delegação no EWS no Exchange](handling-delegation-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Permitir que outra pessoa gerencie seu email e calendário](http://office.microsoft.com/en-us/outlook-help/allow-someone-else-to-manage-your-mail-and-calendar-HA102749417.aspx)
    
- [Adicionar-MailboxPermission](http://technet.microsoft.com/en-us/library/bb124097%28v=exchg.150%29.aspx)
    

