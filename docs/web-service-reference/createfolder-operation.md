---
title: Operação CreateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolder
api_type:
- schema
ms.assetid: 6f6c334c-b190-4e55-8f0a-38f2a018d1b3
description: A operação CreateFolder cria pastas, pastas de calendário, pastas de contatos, pastas de tarefas e pastas de pesquisa.
ms.openlocfilehash: 125a6d212e5eaf85ace71c048de809f3a05ba9b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457547"
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

### <a name="request-elements"></a>Elementos Request

Os seguintes elementos são usados na solicitação:
  
- [CreateFolder](createfolder.md)
    
- [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [Pastas](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [DisplayName (cadeia de caracteres)](displayname-string.md)
    
> [!NOTE]
> O esquema que descreve esses elementos está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de acesso para Cliente instalada. 
  
Para encontrar outras opções para a mensagem de solicitação da operação CreateFolder, explore a hierarquia do esquema. Inicie no elemento [CreateFolder](createfolder.md) . 
  
> [!NOTE]
> Se você criar uma pasta de pesquisa com uma restrição usando a propriedade **calendário: organizador** , uma chamada de pasta Get subsequente retornará a restrição com a propriedade **Message: from** em seu lugar. Essas duas propriedades são mapeadas para a mesma propriedade MAPI subjacente. 
  
A operação CreateFolder oferece suporte à criação de uma classe de pasta personalizada somente quando você cria a pasta usando um elemento de tipo de pasta genérico e define o elemento **FolderClass** . 
  
## <a name="successful-createfolder-response-example"></a>Exemplo de resposta CreateFolder bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CreateFolder. Neste exemplo, a resposta retorna os identificadores das novas pastas.
  
> [!NOTE]
> A ID da pasta e a chave de alteração foram reduzidas para preservar a legibilidade. 
  
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
    
Para encontrar outras opções para a mensagem de resposta da operação CreateFolder, explore a hierarquia do esquema. Inicie no elemento [CreateFolderResponse](createfolderresponse.md) . 
  
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
    
Para encontrar outras opções para a mensagem de resposta de erro da operação CreateFolder, explore a hierarquia de esquema. Inicie no elemento [CreateFolderResponse](createfolderresponse.md) . 
  
## <a name="see-also"></a>Também consulte



[Operação FindItem](finditem-operation.md)
  
[Operação FindFolder](findfolder-operation.md)
  
 **CreateFolderType**


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Criando pastas (serviços Web do Exchange)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

