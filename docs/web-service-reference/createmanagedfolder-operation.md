---
title: Operação CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: 60a668a2-b4e9-4db9-ac76-9b181e47b302
description: A operação CreateManagedFolder cria uma pasta gerenciada no armazenamento do Exchange.
ms.openlocfilehash: 2c2af53dc5dbe1e6fcbc7f3b1174a856e51e4905
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751619"
---
# <a name="createmanagedfolder-operation"></a>Operação CreateManagedFolder

A operação CreateManagedFolder cria uma pasta gerenciada no armazenamento do Exchange.
  
## <a name="using-the-createmanagedfolder-operation"></a>Usando a operação CreateManagedFolder

A operação CreateManagedFolder adiciona uma pasta personalizada gerenciada à caixa de correio do usuário. Você pode usar o cmdlet do Shell de gerenciamento do Exchange **Get-ManagedFolder** para localizar pastas gerenciadas disponíveis para adicionar. Embora este cmdlet retorna pastas personalizadas gerenciadas e a pastas padrão gerenciadas, só gerenciadas personalizados pastas podem ser adicionadas. Pastas personalizadas gerenciadas são identificadas por tipo de pasta ManagedCustomFolder. O namespace System. DirectoryServices também inclui tipos que podem ser usados para descobrir os nomes das pastas gerenciadas disponíveis. 
  
> [!NOTE]
> Você não pode usar os serviços Web do Exchange para localizar os nomes das pastas gerenciadas disponíveis para adicionar uma caixa de correio. 
  
Você pode usar as operações FindFolder e GetFolder para acessar pastas gerenciadas. FindFolder é usado para pesquisar pastas em uma pasta pai especificado. Isso pode ser usado para que as pastas gerenciadas podem ser descobertas em uma pasta antes de tentar adicionar que uma duplicata gerenciado pasta personalizada no mesmo diretório. Para obter mais informações sobre uma pasta personalizada gerenciada, GetFolder é usada após a operação FindFolder.
  
## <a name="remarks"></a>Coment�rios

Para obter informações sobre como configurar a política de gerenciamento (MRM) de registros de mensagens, consulte [como criar uma diretiva de caixa de correio de pasta gerenciada](http://go.microsoft.com/fwlink/?LinkId=100975).
  
Para obter informações sobre como remover pastas personalizadas gerenciadas de uma caixa de correio, consulte [Remove-ManagedFolder](http://go.microsoft.com/fwlink/?LinkId=100976).
  
## <a name="createmanagedfolder-request-example"></a>Exemplo de solicitação CreateManagedFolder

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de CreateManagedFolder mostra como adicionar uma chamado pasta gerenciada de teste para uma caixa de correio de pasta gerenciada.
  
> [!NOTE]
> Você também pode usar o acesso de representante para adicionar pastas personalizadas gerenciadas. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateManagedFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderNames>
        <t:FolderName>Test Managed Folder</t:FolderName>
      </FolderNames>
    </CreateManagedFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Elementos de solicitação

Os seguintes elementos são usados na solicitação:
  
- [CreateManagedFolder](createmanagedfolder.md)
    
- [Nomes de pastas](foldernames.md)
    
- [FolderName](foldername.md)
    
Para localizar outras opções para a mensagem de solicitação da operação CreateManagedFolder, explore a hierarquia de esquema. Inicie o elemento [CreateManagedFolder](createmanagedfolder.md) . 
  
## <a name="successful-createmanagedfolder-response"></a>Resposta de CreateManagedFolder bem-sucedida

### <a name="description"></a>Descrição

O exemplo de código a seguir mostra uma resposta bem-sucedida a uma solicitação de CreateManagedFolder.
  
> [!NOTE]
> Os valores do atributo **Id** e **ChangeKey** foram diminuídos para preservar a legibilidade. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS0AdX=" ChangeKey="AACADA=="/>
            </t:Folder>
          </m:Folders>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedida

Os seguintes elementos são usados na resposta: 
  
- [CreateManagedFolderResponse](createmanagedfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Pastas](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
Para localizar outras opções para as mensagens de resposta da operação CreateManagedFolder, explore a hierarquia de esquema. Inicie o elemento [CreateManagedFolderResponse](createmanagedfolderresponse.md) . 
  
## <a name="createmanagedfolder-error-response"></a>Resposta de erro CreateManagedFolder

### <a name="description"></a>Descrição

O exemplo de código a seguir mostra uma resposta de erro a uma solicitação de CreateManagedFolder.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Error">
          <m:MessageText>A specified managed folder already exists in the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorManagedFolderAlreadyExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders/>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Elementos de resposta de erro

Os seguintes elementos são usados na resposta de erro:
  
- [CreateManagedFolderResponse](createmanagedfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Pastas](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>Confira também



[Operação GetFolder](getfolder-operation.md)
  
[Operação FindFolder](findfolder-operation.md)


[Localizando pastas](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Adicionando pastas gerenciadas](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

