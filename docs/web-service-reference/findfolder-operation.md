---
title: Operação FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolder
api_type:
- schema
ms.assetid: 7a9855aa-06cc-45ba-ad2a-645c15b7d031
description: A operação FindFolder usa os serviços Web do Exchange para localizar subpastas de uma pasta identificada e retorna um conjunto de propriedades que descrevem o conjunto de subpastas.
ms.openlocfilehash: f1cc199bdaf684d8d74687ed7f064eb66fee48ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462581"
---
# <a name="findfolder-operation"></a>Operação FindFolder

A operação **FindFolder** usa os serviços Web do Exchange para localizar subpastas de uma pasta identificada e retorna um conjunto de propriedades que descrevem o conjunto de subpastas. 
  
## <a name="remarks"></a>Comentários

FindFolder retorna apenas os primeiros 512 bytes de qualquer propriedade streamable. Para Unicode, ele retorna os primeiros 255 caracteres usando uma cadeia de caracteres Unicode terminada em nulo.
  
Consultas de passagem profunda não podem ser realizadas em pastas públicas.
  
As restrições são permitidas e devem usar apenas as propriedades da pasta, não as propriedades do item. A funcionalidade de classificação não está disponível para respostas **FindFolder** . As consultas agrupadas não estão disponíveis para consultas do **FindFolder** . 
  
 **Observação** A operação **FindFolder** também é usada para localizar pastas gerenciadas. 
  
### <a name="soap-headers"></a>Cabeçalhos SOAP

A operação **FindFolder** pode usar os cabeçalhos SOAP listados e descritos na tabela a seguir. 
  
|**Header**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|Representação  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando.  <br/> |
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura RFC3066 a ser usada para acessar a caixa de correio.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação.  <br/> |
|TimeZoneContext  <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Identifica o fuso horário a ser usado para todas as respostas do servidor.  <br/> |
   
## <a name="findfolder-request-example"></a>Exemplo de solicitação FindFolder

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação **FindFolder** mostra como formar uma solicitação para localizar todas as pastas localizadas em uma caixa de entrada. 
  
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

Usando o valor padrão para o [BaseShape](baseshape.md), a resposta retorna o nome da pasta, a ID da pasta, o número de subpastas, o número de pastas filhas encontradas na pasta e a contagem de itens não lidos.
  
### <a name="request-elements"></a>Elementos Request

Essa solicitação de **FindFolder** inclui os seguintes elementos: 
  
- [FindFolder](findfolder.md)
    
- [FolderShape](foldershape.md)
    
- [BaseShape](baseshape.md)
    
- [ParentFolderIds](parentfolderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
 Para obter outros elementos de solicitação do **FindFolder** , consulte o esquema. 
  
## <a name="findfolder-response-example"></a>Exemplo de resposta FindFolder

### <a name="description"></a>Descrição

O exemplo a seguir do corpo SOAP (Simple Object Access Protocol) mostra uma resposta bem-sucedida à solicitação **FindFolder** . A resposta contém os elementos que são retornados quando o valor padrão para [BaseShape](baseshape.md) é usado. 
  
> [!NOTE]
> A ID da pasta e a chave de alteração foram reduzidas para preservar a legibilidade. 
  
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

As propriedades que são retornadas na resposta são determinadas pelo [BaseShape](baseshape.md) e asproperties [adicionais](additionalproperties.md) se forem usadas. Uma resposta bem-sucedida do **FindFolder** inclui os seguintes elementos: 
  
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

 As respostas **FindFolder** a uma solicitação com a forma de resposta **myproperties** não retornarão os elementos [TotalCount](totalcount.md) e [UnreadCount](unreadcount.md) para pesquisas de pasta pública. 
  
## <a name="findfolder-error-response-example"></a>Exemplo de resposta de erro FindFolder

### <a name="description"></a>Descrição

O seguinte exemplo de corpo SOAP mostra uma resposta de erro que ocorre quando você procura uma pasta identificada por um identificador de pasta malformado.
  
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

A resposta de erro **FindFolder** inclui os seguintes elementos: 
  
- [FindFolderResponse](findfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="additional-information"></a>Informações Adicionais

- O elemento [DisplayName (cadeia de caracteres)](displayname-string.md) da pasta sempre é incluído na forma padrão. 
    
- O elemento [UnreadCount](unreadcount.md) está incluído nas pastas tarefas e anotações. 
    
- Use o valor **PropertyTag** de 0x672D com um tipo de propriedade de **inteiro** para identificar uma pasta gerenciada usando o elemento [ExtendedFieldURI](extendedfielduri.md) . 
    
## <a name="see-also"></a>Confira também



[Localizando pastas](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

