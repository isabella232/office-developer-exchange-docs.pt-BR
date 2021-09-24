---
title: Operação CreateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateFolder
api_type:
- schema
ms.assetid: 6f6c334c-b190-4e55-8f0a-38f2a018d1b3
description: A operação CreateFolder cria pastas, pastas de calendário, pastas de contatos, pastas de tarefas e pastas de pesquisa.
ms.openlocfilehash: 1b6259ba15e31ee9976c08afa8971ead9a1d5b16
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515849"
---
# <a name="createfolder-operation"></a>Operação CreateFolder

A operação CreateFolder cria pastas, pastas de calendário, pastas de contatos, pastas de tarefas e pastas de pesquisa.
  
## <a name="createfolder-request-example"></a>Exemplo de solicitação CreateFolder

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação CreateFolder mostra como formar uma solicitação para criar duas novas pastas na raiz da caixa de correio.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ParentFolderId>
        <t:DistinguishedFolderId Id="msgfolderroot"/>
      </ParentFolderId>
      <Folders>
        <t:Folder>
          <t:DisplayName>Folder1</t:DisplayName>
        </t:Folder>
        <t:Folder>
          <t:DisplayName>Folder2</t:DisplayName>
        </t:Folder>
      </Folders>
    </CreateFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Elementos request

Os seguintes elementos são usados na solicitação:
  
- [CreateFolder](createfolder.md)
    
- [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [Pastas](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [DisplayName (cadeia de caracteres)](displayname-string.md)
    
> [!NOTE]
> O esquema que descreve esses elementos está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada. 
  
Para encontrar outras opções para a mensagem de solicitação da operação CreateFolder, explore a hierarquia de esquema. Comece no [elemento CreateFolder.](createfolder.md) 
  
> [!NOTE]
> Se você criar uma pasta de pesquisa com uma restrição usando a propriedade **calendar:Organizer,** uma chamada de pasta get subsequente retornará a restrição com a propriedade **message:from** em seu lugar. Essas duas propriedades mapeiam para a mesma propriedade MAPI subjacente. 
  
A operação CreateFolder dá suporte à criação de uma classe de pasta personalizada somente quando você cria a pasta usando um elemento de tipo de pasta genérico e desdopaco o **elemento FolderClass.** 
  
## <a name="successful-createfolder-response-example"></a>Exemplo de resposta CreateFolder bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CreateFolder. Neste exemplo, a resposta retorna os identificadores das novas pastas.
  
> [!NOTE]
> A ID da pasta e a chave de alteração foram reduzidas para preservar a capacidade de leitura. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn==" />
            </t:Folder>
          </m:Folders>
        </m:CreateFolderResponseMessage>
        <m:CreateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn==" />
            </t:Folder>
          </m:Folders>
        </m:CreateFolderResponseMessage>
      </m:ResponseMessages>
    </CreateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateFolderResponse](createfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateFolderResponseMessage](createfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Pastas](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
Para encontrar outras opções para a mensagem de resposta da operação CreateFolder, explore a hierarquia de esquema. Comece no [elemento CreateFolderResponse.](createfolderresponse.md) 
  
## <a name="createfolder-error-response"></a>Resposta de erro CreateFolder

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma solicitação CreateFolder.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateFolderResponseMessage ResponseClass="Error">
          <m:MessageText>A folder with the specified name already exists.</m:MessageText>
          <m:ResponseCode>ErrorFolderExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:CreateFolderResponseMessage>
      </m:ResponseMessages>
    </CreateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Elementos de resposta de erro

Os seguintes elementos são usados na resposta de erro:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateFolderResponse](createfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateFolderResponseMessage](createfolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Pastas](folders-ex15websvcsotherref.md)
    
Para encontrar outras opções para a mensagem de resposta de erro da operação CreateFolder, explore a hierarquia de esquema. Comece no [elemento CreateFolderResponse.](createfolderresponse.md) 
  
## <a name="see-also"></a>Confira também



[Operação FindItem](finditem-operation.md)
  
[Operação FindFolder](findfolder-operation.md)
  
 **CreateFolderType**


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Criando Pastas (Exchange Web Services)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

