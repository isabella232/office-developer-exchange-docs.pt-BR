---
title: Operação UpdateFolder
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolder
api_type:
- schema
ms.assetid: 3494c996-b834-4813-b1ca-d99642d8b4e7
description: 'A operação UpdateFolder é usada para modificar as propriedades de um item existente no armazenamento do Exchange. Cada operação UpdateFolder consiste no seguinte:'
ms.openlocfilehash: b33937bb09f0dcbe3d3ed61bbf5233423f320d9c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837884"
---
# <a name="updatefolder-operation"></a>Operação UpdateFolder

A operação UpdateFolder é usada para modificar as propriedades de um item existente no armazenamento do Exchange. Cada operação UpdateFolder consiste no seguinte:
  
- Um elemento de [FolderId](folderid.md) que especifica uma pasta a ser atualizado. 
    
- Um caminho interno de um elemento na pasta, conforme especificado pela forma pasta, que especifica os dados para atualizar.
    
- Uma pasta que contém o novo valor do campo atualizado, se a atualização não for uma exclusão.
    
## <a name="remarks"></a>Coment�rios

Três ações de atualização básica podem ser executadas em um item. Essas ações são listadas na tabela a seguir.
  
|**Action**|**Descrição**|
|:-----|:-----|
|Acréscimo  <br/> |A ação append adiciona dados a uma propriedade existente. Preserva os dados que está atualmente lá. Acrescentar não é aplicável a todas as propriedades.  <br/> |
|Conjunto  <br/> |A ação set substitui os dados de uma propriedade se ele contém dados, ou cria a propriedade e define seu valor, se não existir. A ação set só é aplicável às propriedades graváveis.  <br/> |
|Excluir  <br/> |A ação Excluir remove uma propriedade de uma pasta. Isso é diferente de defini-la como um valor vazio. Quando concluir, a propriedade não existe para a pasta. Excluir só é aplicável às propriedades graváveis.  <br/> |
   
## <a name="updatefolder-request-example"></a>Exemplo de solicitação UpdateFolder

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de UpdateFolder mostra como atualizar um nome de exibição da pasta. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a>Comments

Este exemplo altera o nome de exibição da pasta para novonomedepasta.
  
> [!NOTE]
> Os valores de **Id** e **ChangeKey** atributos do elemento [FolderId](folderid.md) foram diminuídos para melhorar a legibilidade. 
  
### <a name="request-elements"></a>Elementos de solicitação

Os seguintes elementos são usados na solicitação:
  
- [UpdateFolder](updatefolder.md)
    
- [FolderChanges](folderchanges.md)
    
- [FolderChange](folderchange.md)
    
- [FolderId](folderid.md)
    
- [Atualizações (Item)](updates-item.md)
    
- [SetFolderField](setfolderfield.md)
    
- [FieldURI](fielduri.md)
    
- [Folder](folder.md)
    
- [DisplayName (string)](displayname-string.md)
    
Consulte o esquema de elementos adicionais que você pode usar para formar uma solicitação UpdateFolder.
  
> [!NOTE]
> O local padrão do esquema está no diretório virtual EWS no computador que possui a função de servidor acesso para cliente instalada. 
  
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
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a>Comments

> [!NOTE]
> A ID de pasta e a chave de alteração tem sido reduzidas para preservar a legibilidade. 
  
O ID da pasta que é retornado na resposta representa a pasta atualizada.
  
### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedida

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

O exemplo a seguir mostra uma resposta de erro a uma solicitação de UpdateFolder.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a>Comments

Este exemplo mostra uma resposta de erro é gerada por um atributo **ChangeKey** inválido na solicitação. 
  
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

