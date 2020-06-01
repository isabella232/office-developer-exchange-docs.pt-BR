---
title: Definir permissões de pasta para outro usuário usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7eb81676-a780-4c56-b4f2-c4ed2697107d
description: Saiba como definir níveis de permissão em uma pasta usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: e25f1a49a430e8c95829d404fa53451b76cab167
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455867"
---
# <a name="set-folder-permissions-for-another-user-by-using-ews-in-exchange"></a>Definir permissões de pasta para outro usuário usando o EWS no Exchange

Saiba como definir níveis de permissão em uma pasta usando a API gerenciada do EWS ou o EWS no Exchange.
  
As permissões no nível de pasta permitem que os usuários acessem uma ou mais pastas na caixa de correio de outro usuário. As permissões de pasta são semelhantes ao acesso de delegação, mas diferem das seguintes maneiras: 
  
- As permissões de pasta não permitem que o usuário "enviar em nome de" ou "enviar como" outro usuário. Eles só habilitam o acesso a pastas. Os usuários podem criar itens nessas pastas, mas não podem enviá-los.
    
- Você pode definir permissões de pasta em qualquer pasta da caixa de correio, mas só pode adicionar um representante às pastas calendário, contatos, caixa de entrada, diário, anotações e tarefas.
    
- Você pode definir várias [permissões em uma pasta específica](#bk_folderperms). Ao adicionar um representante, você pode atribuir um apenas [cinco níveis de permissão](delegate-access-and-ews-in-exchange.md#bk_delegateperms).
    
- Você pode definir permissões de pasta para usuários anônimos e padrão. Você só pode conceder acesso de representante a uma conta habilitada para email.
    
Se você estiver familiarizado com as entradas de controle de acesso (ACEs) e listas de controle de acesso discricional (DACLs), saberá que um usuário só pode ter um conjunto de permissões para cada pasta. Se você tentar adicionar um conjunto de permissões para um usuário e ele já tiver um conjunto de permissões, você receberá um erro. Ao adicionar, remover ou atualizar permissões em uma pasta, você obtém a DACL atual, adiciona ou remove quaisquer ACEs e, em seguida, envia a DACL atualizada. Você não pode adicionar várias ACEs para o mesmo usuário. Ao atualizar permissões usando a API gerenciada do EWS, você precisa remover a ACE atual do usuário e, em seguida, adicionar sua nova ACE à coleção. Se você estiver usando o EWS, basta substituir o conjunto anterior de ACEs com as novas.
  
Se você estiver fazendo várias alterações de permissão em uma única pasta, poderá realizar adições, remoções ou atualizações em lote, apenas Observe que não é possível colocar em lote as atualizações do usuário em várias pastas. Uma chamada é necessária para obter as permissões em uma única pasta e uma segunda chamada é necessária para atualizar as permissões nessa pasta. Ao adicionar, remover ou atualizar permissões de usuário, você usa as mesmas duas chamadas de método ou operações para cada tarefa.
  
**Tabela 1. Métodos da API gerenciada do EWS e operações do EWS para definir permissões de pasta**

|Se você quiser...|Use este método de API gerenciada do EWS...|Use esta operação do EWS...|
|:-----|:-----|:-----|
|Habilitar, remover ou atualizar permissões de pasta  <br/> |[Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) seguido por [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) <br/> |[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) seguido por [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|Criar uma pasta e definir permissões de pasta  <br/> |[Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
   
## <a name="folder-permissions"></a>Permissões de pastas
<a name="bk_folderperms"> </a>

Há algumas opções em relação à definição de permissões de pasta em uma pasta específica. Você pode definir um nível de permissão em uma pasta para cada usuário, que adiciona um conjunto de permissões individuais predefinidas à DACL ou pode definir permissões individuais em uma pasta, mas não é possível misturar e corresponder.
  
As seguintes permissões individuais estão disponíveis:
  
- Pode criar
- Pode criar subpastas    
- É proprietário da pasta    
- A pasta é visível    
- É o contato da pasta    
- Editar itens    
- Excluir itens    
- Ler itens
    
Além disso, os seguintes níveis de permissão estão disponíveis, que definem um subconjunto de permissões e valores individuais, conforme mostrado na tabela 2:
  
- Nenhum    
- Proprietário    
- Publishingeditorcreateitems    
- Editor    
- Publishingauthorcreateitems    
- Autor    
- Noneditingauthorcreateitems    
- Revisor    
- Colaborador   
- Custom-este valor não pode ser definido pelo aplicativo. O servidor define esse valor se o aplicativo incluir uma coleção personalizada de permissões individuais.    
- FreeBusyTimeOnly-isso só pode ser definido em pastas de calendário.   
- FreeBusyTimeAndSubjectAndLocation-isso só pode ser definido em pastas de calendário.
    
A tabela a seguir mostra quais permissões individuais são aplicadas por padrão com base no nível de permissão.
  
**Tabela 2. Permissões individuais por nível de permissão**

|Nível da permissão|Pode criar itens|Pode criar subpastas|É proprietário da pasta|A pasta é visível|É o contato da pasta|Editar itens|Excluir itens|Pode ler itens|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Nenhum  <br/> |Falso  <br/> |Falso  <br/> |Falso  <br/> |Falso  <br/> |Falso  <br/> |Nenhum  <br/> |Nenhum  <br/> |Nenhum  <br/> |
|Proprietário  <br/> |Verdadeiro  <br/> |Verdadeiro  <br/> |Verdadeiro  <br/> |Verdadeiro  <br/> |Verdadeiro  <br/> |Todos  <br/> |Todos  <br/> |FullDetails  <br/> |
|Publishingeditorcreateitems  <br/> |Verdadeiro  <br/> |Verdadeiro  <br/> |Falso  <br/> |Verdadeiro  <br/> |Falso  <br/> |Todos  <br/> |Todos  <br/> |FullDetails  <br/> |
|Editor  <br/> |Verdadeiro  <br/> |Falso  <br/> |Falso  <br/> |Verdadeiro  <br/> |Falso  <br/> |Todos  <br/> |Todos  <br/> |FullDetails  <br/> |
|Publishingauthorcreateitems  <br/> |Verdadeiro  <br/> |Verdadeiro  <br/> |Falso  <br/> |Verdadeiro  <br/> |Falso  <br/> |Possuir  <br/> |Possuir  <br/> |FullDetails  <br/> |
|Autor  <br/> |Verdadeiro  <br/> |Falso  <br/> |Falso  <br/> |Verdadeiro  <br/> |Falso  <br/> |Possuir  <br/> |Possuir  <br/> |FullDetails  <br/> |
|Noneditingauthorcreateitems  <br/> |Verdadeiro  <br/> |Falso  <br/> |Falso  <br/> |Verdadeiro  <br/> |Falso  <br/> |Nenhum  <br/> |Possuir  <br/> |FullDetails  <br/> |
|Revisor  <br/> |Falso  <br/> |Falso  <br/> |Falso  <br/> |Verdadeiro  <br/> |Falso  <br/> |Nenhum  <br/> |Nenhum  <br/> |FullDetails  <br/> |
|Colaborador  <br/> |Verdadeiro  <br/> |Falso  <br/> |Falso  <br/> |Verdadeiro  <br/> |Falso  <br/> |Nenhum  <br/> |Nenhum  <br/> |Nenhum  <br/> |
   
Se você especificar um nível de permissão não personalizado na solicitação de permissões de nível de pasta, não será necessário especificar as configurações de permissão individuais. Se você especificar uma permissão individual ao definir um nível de permissão, um erro **ErrorInvalidPermissionSettings** será retornado na resposta. 
  
## <a name="adding-folder-permissions-by-using-the-ews-managed-api"></a>Adicionando permissões de pasta usando a API gerenciada do EWS
<a name="bk_enableewsma"> </a>

O exemplo de código a seguir mostra como usar a API gerenciada do EWS para: 
  
- Criar um novo objeto [FolderPermission](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) para o novo usuário. 
    
- Obtenha as permissões atuais para uma pasta usando o método [BIND](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) . 
    
- Adicione o novo **FolderPermissions** à propriedade [Folder. Permissions](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) . 
    
- Chame o método [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) para salvar as novas permissões no servidor. 
    
Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o proprietário da caixa de correio e que o usuário foi autenticado em um servidor Exchange. 
  
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

Se você quiser usar o nível de permissão personalizado, use este código em vez disso.
  
```cs
FolderPermission fldperm = new FolderPermission();
fldperm.UserId = "sadie@Contoso1000.onmicrosoft.com";
fldperm.CanCreateItems = true;
fldperm.CanCreateSubFolders = true;
…
```

Você pode definir qualquer uma ou todas as [Propriedades FolderPermission](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) graváveis ao criar um objeto **FolderPermission** com um nível de permissão personalizado. Observe, no entanto, que o [FolderPermissionLevel](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) nunca é explicitamente definido como **personalizado** pelo aplicativo. **FolderPermissionLevel** é definido como Custom somente quando você cria um objeto **FolderPermission** e define permissões individuais. 
  
## <a name="adding-folder-permissions-by-using-ews"></a>Adicionando permissões de pasta usando EWS
<a name="bk_enableews"> </a>

Os exemplos de código do EWS a seguir mostram como adicionar permissões a uma pasta específica, recuperando as permissões atuais e, em seguida, enviando uma lista de novas permissões.
  
A primeira etapa é enviar uma solicitação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , em que o valor [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) especifica a pasta na qual adicionar permissões (a pasta Itens enviados neste exemplo) e o valor de [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) inclui a pasta: PermissionSet. Essa solicitação irá recuperar as configurações de permissão para a pasta especificada. 
  
Essa é também a solicitação XML que a API gerenciada do EWS envia quando você chama o método **BIND** para [adicionar permissões de pasta](#bk_enableewsma).
  
```XML
  <?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                 xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

O servidor responde à solicitação **GetFolder** com uma mensagem [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a pasta foi recuperada com êxito. Os valores [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) e [ParentFolderId](https://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) foram reduzidos para facilitar a leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Em seguida, use a operação **UpdateFolder** para enviar o [PermissionSet](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx)atualizado, que inclui a [permissão](https://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) para o novo usuário. Observe que, incluindo o elemento [Setfolderfield](https://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) da respectiva pasta na operação [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) substituirá todas as configurações de permissão na pasta. Da mesma forma, incluindo a opção [DeleteFolderField](https://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) da operação **UpdateFolder** também excluirá todas as configurações de permissão na pasta. 
  
Essa é também a solicitação XML que a API gerenciada do EWS envia quando você chama o método **Update** para [adicionar permissões de pasta](#bk_enableewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Se você quiser usar o nível de permissão personalizado, use este código em vez disso.
  
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

O servidor responde à solicitação **UpdateFolder** com uma mensagem [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a pasta foi atualizada com êxito.
  
## <a name="removing-folder-permissions-by-using-the-ews-managed-api"></a>Removendo permissões de pasta usando a API gerenciada do EWS
<a name="bk_removeewsma"> </a>

O exemplo de código a seguir mostra como usar a API gerenciada do EWS para remover todas as permissões de usuário em uma pasta específica, exceto as permissões padrão e anônimas, por:
  
1. Obtendo as permissões atuais para uma pasta usando o método **BIND** . 
    
2. Iterar pela coleção **Permissions** e remover permissões para usuários individuais. 
    
3. Chamar o método **Update** para salvar as alterações. 
    
Este exemplo remove todas as permissões de usuário em uma pasta. Se você deseja modificar este exemplo para remover permissões somente para um usuário específico, altere a linha de código a seguir para identificar o nome de exibição ou o endereço SMTP do usuário.
  
```cs
if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
```

Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o proprietário da caixa de correio e que o usuário foi autenticado em um servidor Exchange. 
  
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

## <a name="removing-folder-permissions-by-using-ews"></a>Removendo permissões de pasta usando EWS
<a name="bk_removeews"> </a>

Os exemplos de código do EWS a seguir mostram como remover todas as permissões de usuário em uma pasta específica, exceto as permissões padrão e anônimas.
  
Primeiro, envie uma solicitação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) onde o valor [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) especifica a pasta na qual as permissões serão removidas (a pasta Itens enviados neste exemplo) e o valor [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) inclui Folder: PermissionSet. Essa solicitação recuperará o [PermissionSet](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) para a pasta especificada. 
  
Essa é também a solicitação XML que a API gerenciada do EWS envia quando você chama o método **BIND** para [remover permissões de pasta](#bk_removeewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

O servidor responde à solicitação **GetFolder** com uma mensagem [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a pasta foi recuperada com êxito. Os valores dos elementos **FolderId** e **ParentFolderId** foram reduzidos para facilitar a leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Em seguida, use a operação **UpdateFolder** para enviar o **PermissionSet**atualizado, que não inclui a **permissão** para o usuário removido. 
  
Essa é também a solicitação XML que a API gerenciada do EWS envia quando você chama o método **Update** para [remover as permissões de pasta](#bk_removeewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

O servidor responde à solicitação **UpdateFolder** com uma mensagem **UpdateFolderResponse** que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a atualização foi bem-sucedida.
  
## <a name="updating-folder-permissions-by-using-the-ews-managed-api"></a>Atualizando permissões de pasta usando a API gerenciada do EWS
<a name="bk_updateewsma"> </a>

Você também pode atualizar as permissões de pasta de uma pasta específica usando a API gerenciada do EWS. Para atualizar as permissões: 
  
1. [Remova as permissões de pasta](#bk_removeewsma) para as permissões desatualizadas, mas não chame o método **Update** (ainda). 
    
2. [Adicione permissões de pasta para os usuários novos ou alterados](#bk_enableewsma).
    
3. Chame o método **Update** para salvar as alterações. 
    
Se você tentar adicionar dois conjuntos de permissões para o mesmo usuário, receberá **um erro de** ServiceDescription com a seguinte descrição: "o conjunto de permissões especificado contém userids duplicados". Nesse caso, remova as permissões atuais da coleção **Permission** e, em seguida, adicione as novas permissões à coleção **Permission** . 
  
## <a name="updating-folder-permissions-by-using-ews"></a>Atualizando permissões de pasta usando EWS
<a name="bk_updateews"> </a>

Você também pode atualizar as permissões de pasta para pastas específicas usando o EWS, combinando o processo de remoção e adição. Para atualizar as permissões: 
  
1. Recupere as permissões atuais da pasta usando a operação **GetFolder** . 
    
2. Envie uma lista atualizada de permissões usando a operação **UpdateFolder** . 
    
Essas são as mesmas duas operações que você usa para [habilitar](#bk_enableews) ou [remover o acesso](#bk_removeews) usando o EWS. A única diferença é que, quando você recebe a resposta **GetFolder** , ele conterá um conjunto de **permissões** para User. Basta substituir esse elemento de **permissão** existente pelo novo elemento **Permission** e, em seguida, enviar a operação **UpdateFolder** com o novo valor de **permissão** ou valores. 
  
Se você tentar adicionar dois conjuntos de permissões para o mesmo usuário, receberá um valor de **ResponseCode** de **ErrorDuplicateUserIdsSpecified**. Nesse caso, remova o valor de permissão desatualizado para o usuário da solicitação e repita a solicitação.

## <a name="next-steps"></a>Próximas etapas

Depois de conceder a um usuário permissão para uma pasta específica, o usuário pode acessar a pasta como um representante. Para saber mais, confira:
  
- [Acessar email como um representante usando o EWS no Exchange](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Acessar um calendário como um representante usando o EWS no Exchange](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Acessar contatos como um representante usando o EWS no Exchange](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Também consulte

- [Acesso de representante e EWS no Exchange](delegate-access-and-ews-in-exchange.md)   
- [Adicionar e remover representantes usando o EWS no Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [Pastas e itens no EWS no Exchange](folders-and-items-in-ews-in-exchange.md)
    

