---
title: Operação FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindFolder
api_type:
- schema
ms.assetid: 7a9855aa-06cc-45ba-ad2a-645c15b7d031
description: A operação FindFolder usa Exchange Web Services para encontrar subpastas de uma pasta identificada e retorna um conjunto de propriedades que descrevem o conjunto de subpastas.
ms.openlocfilehash: 8c2776a9d60244fe77b6012a09ffbad230d86f63
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518467"
---
# <a name="findfolder-operation"></a>Operação FindFolder

A **operação FindFolder** usa Exchange Web Services para encontrar subpastas de uma pasta identificada e retorna um conjunto de propriedades que descrevem o conjunto de subpastas. 
  
## <a name="remarks"></a>Comentários

FindFolder retorna apenas os primeiros 512 bytes de qualquer propriedade streamable. Para Unicode, ele retorna os primeiros 255 caracteres usando uma cadeia de caracteres Unicode terminada em nulo.
  
As consultas transnacionais profundas não podem ser executadas em pastas públicas.
  
Restrições são permitidas e devem usar apenas as propriedades da pasta, não as propriedades do item. A funcionalidade de classificação não está disponível para respostas **findFolder.** As consultas agrupadas não estão disponíveis para consultas **FindFolder.** 
  
 **Observação** A **operação FindFolder** também é usada para encontrar pastas gerenciadas. 
  
### <a name="soap-headers"></a>SOAP Headers

A **operação FindFolder** pode usar os headers SOAP listados e descritos na tabela a seguir. 
  
|**Header**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|Representação  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando.  <br/> |
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura RFC3066 a ser usada para acessar a caixa de correio.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação.  <br/> |
|TimeZoneContext  <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Identifica o fuso horário a ser usado para todas as respostas do servidor.  <br/> |
   
## <a name="findfolder-request-example"></a>Exemplo de solicitação FindFolder

### <a name="description"></a>Descrição

O exemplo a seguir de uma **solicitação FindFolder** mostra como formar uma solicitação para localizar todas as pastas localizadas em uma Caixa de Entrada. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

Usando o valor Padrão para [BaseShape](baseshape.md), a resposta retorna o nome da pasta, a ID da pasta, o número de subpastas, o número de pastas filho encontradas na pasta e a contagem de itens não lidos.
  
### <a name="request-elements"></a>Elementos request

Esta **solicitação FindFolder** inclui os seguintes elementos: 
  
- [FindFolder](findfolder.md)
    
- [FolderShape](foldershape.md)
    
- [BaseShape](baseshape.md)
    
- [ParentFolderIds](parentfolderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
 Para obter **elementos de solicitação FindFolder** adicionais, consulte o esquema. 
  
## <a name="findfolder-response-example"></a>Exemplo de resposta FindFolder

### <a name="description"></a>Descrição

O exemplo de corpo soap (Simple Object Access Protocol) a seguir mostra uma resposta bem-sucedida à **solicitação FindFolder.** A resposta contém os elementos retornados quando o valor Padrão para [BaseShape](baseshape.md) é usado. 
  
> [!NOTE]
> A ID da pasta e a chave de alteração foram reduzidas para preservar a capacidade de leitura. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Folders>
              <t:Folder>
                <t:FolderId Id="AQAnAH" ChangeKey="AQAAABY" />
                <t:DisplayName>TestFolder</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </FindFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a>Elementos de resposta

As propriedades retornadas na resposta são determinadas pela [BaseShape](baseshape.md) e [as AdditionalProperties](additionalproperties.md) se elas são usadas. Uma resposta **FindFolder** bem-sucedida inclui os seguintes elementos: 
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [FindFolderResponse](findfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [FindFolderResponseMessage](findfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md)
    
- [Pastas](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
- [DisplayName (cadeia de caracteres)](displayname-string.md)
    
- [TotalCount](totalcount.md)
    
- [ChildFolderCount](childfoldercount.md)
    
- [UnreadCount](unreadcount.md)
    
### <a name="comments"></a>Comentários

 **As respostas findFolder** a uma solicitação com a forma de resposta **AllProperties** não retornarão os elementos [TotalCount](totalcount.md) e [UnreadCount](unreadcount.md) para pesquisas de pasta pública. 
  
## <a name="findfolder-error-response-example"></a>Exemplo de resposta de erro findFolder

### <a name="description"></a>Descrição

O exemplo de corpo SOAP a seguir mostra uma resposta de erro que ocorre quando você pesquisa uma pasta identificada por um identificador de pasta malformada.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </FindFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Elementos de resposta de erro

A **resposta de erro FindFolder** inclui os seguintes elementos: 
  
- [FindFolderResponse](findfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="additional-information"></a>Informações Adicionais

- O elemento [DisplayName (cadeia de caracteres)](displayname-string.md) da pasta está sempre incluído na forma padrão. 
    
- O [elemento UnreadCount](unreadcount.md) está incluído nas pastas Tarefas e Anotações. 
    
- Use o **valor PropertyTag** de 0x672D com um tipo de propriedade **Integer** para identificar uma pasta gerenciada usando o [elemento ExtendedFieldURI.](extendedfielduri.md) 
    
## <a name="see-also"></a>Confira também



[Localizar Pastas](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

