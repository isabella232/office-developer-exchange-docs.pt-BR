---
title: Definir permissões de pasta para outro usuário usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7eb81676-a780-4c56-b4f2-c4ed2697107d
description: Saiba como definir níveis de permissão em uma pasta usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 5bf570612d6349628e7f3abf858daa33daa13745
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750830"
---
# <a name="set-folder-permissions-for-another-user-by-using-ews-in-exchange"></a>Definir permissões de pasta para outro usuário usando o EWS no Exchange

Saiba como definir níveis de permissão em uma pasta usando a API gerenciada de EWS ou EWS no Exchange.
  
Permissões de nível de pasta permitem que os usuários acessem uma ou mais pastas na caixa de correio de outro usuário. Permissões da pasta são semelhantes às Delegar acesso, mas diferem das seguintes maneiras: 
  
- Permissões da pasta não permitir que um usuário "Enviar em nome de" ou "Enviar como" outro usuário. Eles só pode ativar o acesso às pastas. Os usuários podem criar itens nessas pastas, mas eles não podem enviá-los.
    
- Você pode definir permissões de pasta em qualquer pasta na caixa de correio, mas você só pode adicionar um representante para as pastas de calendário, contatos, caixa de entrada, diário, anotações e tarefas.
    
- Você pode definir um número de [permissões em uma pasta específica](#bk_folderperms). Quando você adiciona um representante, você pode atribuir um dos [cinco níveis de permissão](delegate-access-and-ews-in-exchange.md#bk_delegateperms).
    
- Você pode definir permissões da pasta para anônimos e usuários de padrão. Você só pode conceder acesso de representante para uma conta habilitada para email.
    
Se você estiver familiarizado com as entradas de controle de acesso (ACEs) e controle de acesso discricionário listas (DACLs), você sabe que um usuário pode ter apenas um conjunto de permissões para cada pasta. Se você tentar adicionar um conjunto de permissões para um usuário e já tenham um conjunto de permissões, você receberá um erro. Quando você adicionar, remove ou atualizar permissões em uma pasta, você fazer a DACL atual, adicionar ou remove qualquer ACEs e envie a DACL atualizada. Não é possível adicionar vários ACEs para o mesmo usuário. Quando você atualizar permissões usando a API gerenciada de EWS, você precisa remover ACE do usuário atual e, em seguida, adicionar seu ACE nova à coleção. Se você estiver usando o EWS, apenas substitua o conjunto de ACEs anterior com as novas.
  
Se você estiver fazendo várias alterações de permissão para uma única pasta, você pode lote adições, remoções ou atualizações — apenas Observe que você não pode atualizações do usuário em várias pastas de lote. Uma chamada é necessário para obter as permissões em uma única pasta e uma segunda chamada é necessária para atualizar as permissões dessa pasta. Quando você adicionar, remove ou atualizar as permissões de usuário, você deve usar o mesmo método de duas chamadas ou operações para cada tarefa.
  
**Tabela 1. Métodos de API gerenciada de EWS e operações de EWS para configurar permissões de pasta**

|Se você quiser …|Use este método de API gerenciada de EWS …|Use essa operação EWS …|
|:-----|:-----|:-----|
|Habilitar, remover ou atualizar as permissões de pasta  <br/> |[Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) seguido [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) <br/> |[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) seguido [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|Crie uma pasta e definir permissões de pasta  <br/> |[Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
   
## <a name="folder-permissions"></a>Permissões de pasta
<a name="bk_folderperms"> </a>

Há algumas opções que diz respeito à definição de permissões de pasta em uma pasta específica. Você pode definir um nível de permissão em uma pasta para cada usuário, que adiciona um conjunto de permissões individuais predefinidos à DACL, ou você pode definir permissões individuais em uma pasta — mas não é possível misturar e corresponder.
  
As seguintes permissões individuais estão disponíveis:
  
- Pode criar
- Pode criar subpastas    
- É o proprietário da pasta    
- Pasta está visível    
- É o contato da pasta    
- Editar itens    
- Excluir itens    
- Ler itens
    
Além disso, os seguintes níveis de permissão estão disponíveis, que definem um subconjunto de permissões individuais e valores, conforme mostrado na tabela 2:
  
- None    
- Proprietário    
- PublishingEditor    
- Editor    
- PublishingAuthor    
- Autor    
- NoneditingAuthor    
- Reviewer    
- Colaborador   
- Personalizado - este valor não pode ser definido pelo aplicativo. O servidor define esse valor se o aplicativo inclui uma coleção personalizada de permissões individuais.    
- FreeBusyTimeOnly - isso pode apenas ser definida em pastas de calendário.   
- FreeBusyTimeAndSubjectAndLocation - isso pode apenas ser definida em pastas de calendário.
    
A tabela a seguir mostra quais permissões individuais são aplicadas por padrão, com base no nível de permissão.
  
**Tabela 2. Permissões individuais por nível de permissão**

|Nível da permissão|Pode criar itens|Pode criar subpastas|É o proprietário da pasta|Pasta está visível|É o contato da pasta|Editar itens|Excluir itens|Pode ler itens|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|None  <br/> |False  <br/> |False  <br/> |False  <br/> |False  <br/> |False  <br/> |Nenhum  <br/> |Nenhum  <br/> |Nenhum  <br/> |
|Proprietário  <br/> |Verdadeiro  <br/> |Verdadeiro  <br/> |Verdadeiro  <br/> |Verdadeiro  <br/> |Verdadeiro  <br/> |Todos  <br/> |Todos  <br/> |FullDetails  <br/> |
|PublishingEditor  <br/> |Verdadeiro  <br/> |True  <br/> |False  <br/> |True  <br/> |False  <br/> |Todos  <br/> |Todos  <br/> |FullDetails  <br/> |
|Editor  <br/> |True  <br/> |False  <br/> |False  <br/> |True  <br/> |False  <br/> |Todos  <br/> |Todos  <br/> |FullDetails  <br/> |
|PublishingAuthor  <br/> |Verdadeiro  <br/> |True  <br/> |False  <br/> |True  <br/> |False  <br/> |Pertencentes  <br/> |Pertencentes  <br/> |FullDetails  <br/> |
|Autor  <br/> |True  <br/> |False  <br/> |False  <br/> |True  <br/> |False  <br/> |Pertencentes  <br/> |Pertencentes  <br/> |FullDetails  <br/> |
|NoneditingAuthor  <br/> |True  <br/> |False  <br/> |False  <br/> |True  <br/> |False  <br/> |None  <br/> |Pertencentes  <br/> |FullDetails  <br/> |
|Reviewer  <br/> |False  <br/> |False  <br/> |False  <br/> |True  <br/> |False  <br/> |Nenhum  <br/> |Nenhum  <br/> |FullDetails  <br/> |
|Colaborador  <br/> |True  <br/> |False  <br/> |False  <br/> |True  <br/> |False  <br/> |Nenhum  <br/> |Nenhum  <br/> |Nenhum  <br/> |
   
Se você especificar um nível de permissão não personalizadas na solicitação de permissões de nível de pasta, você não precisará especificar as configurações de permissão individual. Se você especificar uma permissão individual ao definir um nível de permissão, será retornado um erro **ErrorInvalidPermissionSettings** na resposta. 
  
## <a name="adding-folder-permissions-by-using-the-ews-managed-api"></a>Adicionar permissões de pasta usando a API gerenciada de EWS
<a name="bk_enableewsma"> </a>

O exemplo de código a seguir mostra como usar a API gerenciada de EWS para: 
  
- Crie um novo objeto de [FolderPermission](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) para o novo usuário. 
    
- Obtenha as permissões atuais de uma pasta usando o método [vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) . 
    
- Adicione o novo **FolderPermissions** à propriedade [Folder.Permissions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) . 
    
- Chame o método [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) para salvar as novas permissões no servidor. 
    
Este exemplo supõe que esse **serviço** é um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o proprietário da caixa de correio e que o usuário foi autenticado com um servidor Exchange. 
  
```cs
static void EnableFolderPermissions(ExchangeService service)
{
    // Create a property set to use for folder binding.
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.Permissions);
    // Specify the SMTP address of the new user and the folder permissions level.
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
    
    // Bind to the folder and get the current permissions. 
    // This call results in a GetFolder call to EWS.
    Folder sentItemsFolder = Folder.Bind(service, WellKnownFolderName.SentItems, propSet);
 
    // Add the permissions for the new user to the Sent Items DACL.
    sentItemsFolder.Permissions.Add(fldperm);
    // This call results in a UpdateFolder call to EWS.
    sentItemsFolder.Update();
}
```

A linha de código a seguir especifica o nível de permissão.
  
```cs
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
```

Se você quiser usar o nível de permissão personalizado, use este código.
  
```cs
FolderPermission fldperm = new FolderPermission();
fldperm.UserId = "sadie@Contoso1000.onmicrosoft.com";
fldperm.CanCreateItems = true;
fldperm.CanCreateSubFolders = true;
…
```

Você pode definir qualquer uma ou todas as [Propriedades de FolderPermission](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) de gravável quando você cria um objeto **FolderPermission** com um nível de permissão personalizados. No entanto, observe que o [FolderPermissionLevel](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) nunca explicitamente estiver definido como **personalizada** pelo aplicativo. O **FolderPermissionLevel** é definido como o sinalizador somente quando você cria um objeto **FolderPermission** e definir permissões individuais. 
  
## <a name="adding-folder-permissions-by-using-ews"></a>Adicionando permissões da pasta usando o EWS
<a name="bk_enableews"> </a>

Os seguintes exemplos de código do EWS mostram como adicionar permissões a uma pasta específica por recuperar as permissões atuais e, em seguida, enviar uma lista das novas permissões.
  
A primeira etapa é enviar uma solicitação de [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , onde o valor de [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) Especifica a pasta na qual deseja adicionar permissões (a pasta Itens enviados neste exemplo) e o valor de [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) inclui a pasta: PermissionSet. Essa solicitação irá recuperar as configurações de permissão para a pasta especificada. 
  
Isso também é a solicitação XML que o EWS Managed API envia quando você chama o método **ligar** para [Adicionar permissões da pasta](#bk_enableewsma).
  
```XML
  <?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:GetFolder>
        <m:FolderShape>
          <t:BaseShape>IdOnly</t:BaseShape>
          <t:AdditionalProperties>
            <t:FieldURI FieldURI="folder:PermissionSet" />
          </t:AdditionalProperties>
        </m:FolderShape>
        <m:FolderIds>
          <t:DistinguishedFolderId Id="sentitems" />
        </m:FolderIds>
      </m:GetFolder>
    </soap:Body>
  </soap:Envelope>
```

O servidor responde à solicitação **GetFolder** com uma mensagem de [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a pasta foi recuperada com êxito. Os valores [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) e [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) foram diminuídos para melhorar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="CgAAAA=="
                          ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd1" />
              <t:PermissionSet>
                <t:Permissions>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Default</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                </t:Permissions>
              </t:PermissionSet>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

Em seguida, use a operação de **UpdateFolder** para enviar o atualizados [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx), que inclui a [permissão](http://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) para o novo usuário. Observe que incluindo o elemento [SetFolderField](http://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) para a pasta respectivo na operação [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) substituirá todas as definições de permissão na pasta. Da mesma forma, incluindo a opção [DeleteFolderField](http://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) da operação **UpdateFolder** excluirá também todas as definições de permissão na pasta. 
  
Isso também é a solicitação XML que o EWS Managed API envia ao chamar o método **Update** para [Adicionar permissões da pasta](#bk_enableewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="CgAAAA=="
                      ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd1" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:PermissionSet" />
              <t:Folder>
                <t:PermissionSet>
                  <t:Permissions>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Default</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
                      </t:UserId>
                      <t:PermissionLevel>Editor</t:PermissionLevel>
                    </t:Permission>
                  </t:Permissions>
                </t:PermissionSet>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

A linha de código a seguir especifica o nível de permissão.
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
    </t:UserId>
    <t:PermissionLevel>Editor</t:PermissionLevel>
</t:Permission>
```

Se você quiser usar o nível de permissão personalizado, use este código.
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress> sadie@contoso.com </t:PrimarySmtpAddress>
    </t:UserId>
    <t:CanCreateItems>true</t:CanCreateItems>
    <t:CanCreateSubFolders>true</t:CanCreateSubFolders>
    <t:IsFolderOwner>false</t:IsFolderOwner>
    <t:IsFolderVisible>false</t:IsFolderVisible>
    <t:IsFolderContact>false</t:IsFolderContact>
    <t:EditItems>None</t:EditItems>
    <t:DeleteItems>None</t:DeleteItems>
    <t:ReadItems>None</t:ReadItems>
    <t:PermissionLevel>Custom</t:PermissionLevel>
</t:Permission>
```

O servidor responde à solicitação **UpdateFolder** com uma mensagem de [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a pasta foi atualizada com êxito.
  
## <a name="removing-folder-permissions-by-using-the-ews-managed-api"></a>Remover permissões de pasta usando a API gerenciada de EWS
<a name="bk_removeewsma"> </a>

O exemplo de código a seguir mostra como usar a API gerenciada de EWS para remover todas as permissões de usuário em uma pasta específica, exceto para o padrão e permissões anônimas, por:
  
1. Obtendo as permissões atuais de uma pasta usando o método **vincular** . 
    
2. Iterar através da coleção de **permissões** e remover permissões para usuários individuais. 
    
3. Chamar o método **Update** para salvar as alterações. 
    
Este exemplo remove todas as permissões de usuário em uma pasta. Se desejar modificar este exemplo para remover permissões somente para um usuário específico, altere a seguinte linha de código para identificar o nome de exibição ou o endereço SMTP do usuário.
  
```cs
if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
```

Este exemplo supõe que esse **serviço** é um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o proprietário da caixa de correio e que o usuário foi autenticado com um servidor Exchange. 
  
```cs
static void RemoveFolderPermissions(ExchangeService service)
{
    // Create a property set to use for folder binding.
    PropertySet propSet = new PropertySet(BasePropertySet.FirstClassProperties, FolderSchema.Permissions);
    // Bind to the folder and get the current permissions. 
    // This call results in a GetFolder call to EWS.
    Folder sentItemsFolder = Folder.Bind(service, new FolderId(WellKnownFolderName.SentItems, "primary@contoso.com"), propSet);
    // Iterate through the collection of permissions and remove permissions for any 
    // user with a display name or SMTP address. This leaves the anonymous and 
    // default user permissions unchanged. 
    if (sentItemsFolder.Permissions.Count != 0)
    {
        for (int t = 0; t < sentItemsFolder.Permissions.Count; t++)
        {
            // Find any permissions associated with the specified user and remove them from the DACL
            if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
            {
                sentItemsFolder.Permissions.Remove(sentItemsFolder.Permissions[t]);
            }
        }
    }
    // This call results in an UpdateFolder call to EWS.
    sentItemsFolder.Update();
}
```

## <a name="removing-folder-permissions-by-using-ews"></a>Removendo permissões da pasta usando o EWS
<a name="bk_removeews"> </a>

Os seguintes exemplos de código do EWS mostram como remover todas as permissões de usuário em uma pasta específica, exceto para o padrão e permissões anônimas.
  
Primeiro, envie uma solicitação de [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) onde o valor de [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) Especifica a pasta na qual deseja remover permissões (a pasta Itens enviados neste exemplo) e o valor de [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) inclui a pasta: PermissionSet. Essa solicitação irá recuperar o [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) para a pasta especificada. 
  
Isso também é a solicitação XML que o EWS Managed API envia quando você chama o método **ligar** para [Remover permissões de pasta](#bk_removeewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:PermissionSet" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="drafts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **GetFolder** com uma mensagem de [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a pasta foi recuperada com êxito. Os valores dos elementos **FolderId** e **ParentFolderId** foram diminuídos para melhorar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="EAAAAA=="
                          ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd5" />
              <t:ParentFolderId Id="CQAAAA=="
                                ChangeKey="AQAAAA==" />
              <t:FolderClass>IPF.Note</t:FolderClass>
              <t:DisplayName>Drafts</t:DisplayName>
              <t:TotalCount>0</t:TotalCount>
              <t:ChildFolderCount>0</t:ChildFolderCount>
              <t:EffectiveRights>
                <t:CreateAssociated>true</t:CreateAssociated>
                <t:CreateContents>true</t:CreateContents>
                <t:CreateHierarchy>true</t:CreateHierarchy>
                <t:Delete>true</t:Delete>
                <t:Modify>true</t:Modify>
                <t:Read>true</t:Read>
                <t:ViewPrivateItems>true</t:ViewPrivateItems>
              </t:EffectiveRights>
              <t:PermissionSet>
                <t:Permissions>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Default</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:SID>S-1-5-21-1337771579-694202782-848329751-1535223</t:SID>
                      <t:PrimarySmtpAddress>sadie@Contoso.com</t:PrimarySmtpAddress>
                      <t:DisplayName>Sadie Daniels</t:DisplayName>
                    </t:UserId>
                    <t:CanCreateItems>true</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>true</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>All</t:EditItems>
                    <t:DeleteItems>All</t:DeleteItems>
                    <t:ReadItems>FullDetails</t:ReadItems>
                    <t:PermissionLevel>Editor</t:PermissionLevel>
                  </t:Permission>
                </t:Permissions>
              </t:PermissionSet>
              <t:UnreadCount>0</t:UnreadCount>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

Em seguida, use a operação de **UpdateFolder** para enviar o atualizados **PermissionSet**, que não inclui a **permissão** para o usuário removido. 
  
Isso também é a solicitação XML que o EWS Managed API envia ao chamar o método **Update** para [Remover permissões de pasta](#bk_removeewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="EAAAAA=="
                      ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd5" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:PermissionSet" />
              <t:Folder>
                <t:PermissionSet>
                  <t:Permissions>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Default</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                  </t:Permissions>
                </t:PermissionSet>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **UpdateFolder** com uma mensagem de **UpdateFolderResponse** que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica se a atualização foi bem-sucedida.
  
## <a name="updating-folder-permissions-by-using-the-ews-managed-api"></a>Atualizando permissões de pasta usando a API gerenciada de EWS
<a name="bk_updateewsma"> </a>

Você também pode atualizar as permissões da pasta para uma pasta específica usando a API gerenciada de EWS. Para atualizar as permissões: 
  
1. [Remover as permissões de pasta](#bk_removeewsma) para as permissões desatualizadas, mas não chamar o método **Update** (ainda). 
    
2. [Adicionar permissões de pasta para os usuários novos ou alterados](#bk_enableewsma).
    
3. Chame o método **Update** para salvar as alterações. 
    
Se você tentar adicionar dois conjuntos de permissões para o mesmo usuário, você receberá um erro de **ServiceResponseException** com a seguinte descrição: "o conjunto de permissões especificado contém UserIds duplicados". Nesse caso, remova as permissões atuais da coleção **Permission** e adicione novas permissões ao conjunto de **permissão** . 
  
## <a name="updating-folder-permissions-by-using-ews"></a>Atualizando permissões de pasta usando o EWS
<a name="bk_updateews"> </a>

Você também pode atualizar as permissões da pasta para pastas específicas usando o EWS combinando o processo de adição e a remoção. Para atualizar as permissões: 
  
1. Recupere as permissões da pasta atual usando a operação **GetFolder** . 
    
2. Envie uma lista atualizada de permissões usando a operação **UpdateFolder** . 
    
Essas são as mesmas operações de dois, que você pode usar para [Habilitar](#bk_enableews) ou [Remover o acesso](#bk_removeews) usando o EWS. A única diferença é que quando você recebe a resposta **GetFolder** , ele conterá uma **permissão** definido para o usuário. Simplesmente substituir esse elemento de **permissão** existente com o novo elemento de **permissão** e envie a operação **UpdateFolder** com o novo valor de **permissão** ou valores. 
  
Se você tentar adicionar dois conjuntos de permissões para o mesmo usuário, você receberá um valor de **ResponseCode** de **ErrorDuplicateUserIdsSpecified**. Nesse caso, remova o valor de permissão desatualizado para o usuário da solicitação e tente novamente a solicitação.

## <a name="next-steps"></a>Próximas etapas

Depois de conceder uma permissão de usuário para uma pasta específica, o usuário pode acessar a pasta como um representante. For more information, see:
  
- [Email de acesso como um representante, usando o EWS no Exchange](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Acessar um calendário como um representante, usando o EWS no Exchange](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Contatos de acesso como um representante, usando o EWS no Exchange](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Acesso de representante e EWS no Exchange](delegate-access-and-ews-in-exchange.md)   
- [Adicionar e remover representantes usando o EWS no Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [Pastas e itens no EWS no Exchange](folders-and-items-in-ews-in-exchange.md)
    

