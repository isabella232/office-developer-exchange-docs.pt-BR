---
title: Operação UpdateFolder
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateFolder
api_type:
- schema
ms.assetid: 3494c996-b834-4813-b1ca-d99642d8b4e7
description: 'A operação UpdateFolder é usada para modificar propriedades de um item existente no Exchange store. Cada operação UpdateFolder consiste no seguinte:'
ms.openlocfilehash: be8e39e13681cea34e312158c348c60a94374bec
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541760"
---
# <a name="updatefolder-operation"></a>Operação UpdateFolder

A operação UpdateFolder é usada para modificar propriedades de um item existente no Exchange store. Cada operação UpdateFolder consiste no seguinte:
  
- Um [elemento FolderId](folderid.md) que especifica uma pasta a ser atualizada. 
    
- Um caminho interno de um elemento na pasta, conforme especificado pela forma da pasta, que especifica os dados a ser atualizados.
    
- Uma pasta que contém o novo valor do campo atualizado, se a atualização não for uma exclusão.
    
## <a name="remarks"></a>Comentários

Três ações básicas de atualização podem ser executadas em um item. Essas ações estão listadas na tabela a seguir.
  
|**Action**|**Descrição**|
|:-----|:-----|
|Append  <br/> |A ação de anexação adiciona dados a uma propriedade existente. Ele preserva os dados que estão atualmente lá. Append não é aplicável a todas as propriedades.  <br/> |
|Set  <br/> |A ação set substitui os dados de uma propriedade se ela contiver dados ou criar a propriedade e definir seu valor se ele não existir. A ação set só é aplicável a propriedades que podem ser escritas.  <br/> |
|Excluir  <br/> |A ação excluir remove uma propriedade de uma pasta. Isso é diferente de defini-lo como um valor vazio. Quando concluída, a propriedade não existe para a pasta. Delete só é aplicável a propriedades que podem ser escritas.  <br/> |
   
## <a name="updatefolder-request-example"></a>Exemplo de solicitação UpdateFolder

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação UpdateFolder mostra como atualizar um nome de exibição de pasta. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="AScA" ChangeKey="GO3u/"/>
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:DisplayName"/>
              <t:Folder>
                <t:DisplayName>NewFolderName</t:DisplayName>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </FolderChanges>
    </UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

Este exemplo altera o nome de exibição da pasta para NewFolderName.
  
> [!NOTE]
> Os valores dos atributos **Id** e **ChangeKey** do [elemento FolderId](folderid.md) foram reduzidos para a capacidade de leitura. 
  
### <a name="request-elements"></a>Elementos request

Os seguintes elementos são usados na solicitação:
  
- [UpdateFolder](updatefolder.md)
    
- [FolderChanges](folderchanges.md)
    
- [FolderChange](folderchange.md)
    
- [FolderId](folderid.md)
    
- [Updates (Folder)](updates-folder.md)
    
- [SetFolderField](setfolderfield.md)
    
- [FieldURI](fielduri.md)
    
- [Folder](folder.md)
    
- [DisplayName (cadeia de caracteres)](displayname-string.md)
    
Consulte o esquema de elementos adicionais que você pode usar para formar uma solicitação UpdateFolder.
  
> [!NOTE]
> O local padrão do esquema está no diretório virtual do EWS no computador que tem a função de servidor de Acesso para Cliente instalada. 
  
## <a name="updatefolder-response-example"></a>Exemplo de resposta UpdateFolder

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida à solicitação UpdateFolder. Neste exemplo, a nova chave de alteração é retornada para refletir o status atualizado da pasta.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAlAFVz" ChangeKey="AQAAAB" />
            </t:Folder>
          </m:Folders>
        </m:UpdateFolderResponseMessage>
      </m:ResponseMessages>
    </UpdateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

> [!NOTE]
> A ID da pasta e a chave de alteração foram reduzidas para preservar a capacidade de leitura. 
  
A ID da pasta retornada na resposta representa a pasta atualizada.
  
### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateFolderResponse](updatefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateFolderResponseMessage](updatefolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Pastas](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
## <a name="updatefolder-error-response-example"></a>Exemplo de resposta de erro UpdateFolder

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma solicitação UpdateFolder.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The change key is invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidChangeKey</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:UpdateFolderResponseMessage>
      </m:ResponseMessages>
    </UpdateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

Este exemplo mostra uma resposta de erro causada por um atributo **ChangeKey** inválido na solicitação. 
  
### <a name="error-response-elements"></a>Elementos de resposta de erro

Os seguintes elementos são usados na resposta de erro:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateFolderResponse](updatefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateFolderResponseMessage](updatefolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Pastas](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

