---
title: Obter fotos do usuário usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: f86d1099-1f57-47dc-abf2-4d5ae4e900a9
description: Saiba como obter fotos do usuário associadas a uma caixa de correio ou contato usando a API gerenciada do EWS ou o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: 14f2bc6bef1ce3c3529f03e213e3ada7c45a5a71
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455783"
---
# <a name="get-user-photos-by-using-ews-in-exchange"></a>Obter fotos do usuário usando o EWS no Exchange

Saiba como obter fotos do usuário associadas a uma caixa de correio ou contato usando a API gerenciada do EWS ou o EWS no Exchange.
  
É bom colocar um rosto em um nome. Se seus usuários gostam de colocar nomes em faces, seu aplicativo pode solicitar uma imagem, normalmente uma foto, do Exchange que representa uma conta de email. Você pode obter uma foto de usuário armazenada em um servidor do Exchange para uma caixa de correio ou pode obter uma foto de contato de contatos armazenados na sua caixa de correio.
  
Você pode usar várias tecnologias diferentes para obter fotos de caixas de correio ou dos serviços de domínio do Active Directory (AD DS). A melhor maneira de obter uma foto depende do tipo de contato do qual você deseja obter uma foto. 
  
**Tabela 1. Tecnologias a serem usadas para obter fotos do usuário com base no tipo de contato**

|**Tipo de contato**|**Tecnologias a serem usadas**|
|:-----|:-----|
|Foto do usuário da caixa de correio  <br/> |[Obter uma foto de usuário de caixa de correio usando REST](#bk_REST)<br/><br/> [Obter uma foto do usuário usando o EWS](#bk_EWS) <br/> |
|Foto do usuário de contato  <br/> |[Obter uma foto de usuário de contato usando a API gerenciada do EWS](#bk_EWSMA)<br/><br/> [Obter uma foto do usuário usando o EWS](#bk_EWS) <br/> |

<a name="bk_REST"> </a>

## <a name="get-a-mailbox-user-photo-by-using-rest"></a>Obter uma foto de usuário de caixa de correio usando REST

Você pode solicitar fotos de usuários de um servidor Exchange usando uma solicitação de http **Get** padrão. Na solicitação, especifique o endereço da conta de email e um código de tamanho para a imagem, conforme mostrado no exemplo a seguir. 
  
```HTML
https://Exchange Server/ews/Exchange.asmx/s/GetUserPhoto?email=email address&amp;size=size code
```

Use a operação [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) do serviço de descoberta automática para recuperar a configuração **ExternalEwsUrl** , que contém a URL do ponto de extremidade dos serviços Web do Exchange (EWS) e o local do manipulador http **Exchange. asmx** que retorna as fotos do usuário. 
  
Cada código de tamanho indica a altura e a largura da imagem em pixels. Por exemplo, o código de tamanho **HR48x48** retorna uma imagem que tem 48 pixels de altura por 48 pixels de largura. Os valores possíveis para o parâmetro de código de tamanho são os mesmos valores possíveis para o elemento [SizeRequested](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) . Se a solicitação especificar um tamanho que não está disponível, a maior foto disponível será retornada. Se nenhuma foto estiver armazenada no servidor do Exchange, a imagem em miniatura armazenada no AD DS para a conta será retornada. 
  
> [!NOTE]
> O código de tamanho **HR48x48** sempre retorna a imagem em miniatura do AD DS, se estiver disponível. 
  
O exemplo a seguir mostra como você pode usar a solicitação GET para recuperar a foto do usuário para o Sadie e salvá-la no computador local.
  
```cs
// Create the web request with the REST URL.
HttpWebRequest request = 
   WebRequest.Create("https://www.contoso.com/ews/exchange.asmx/s/GetUserPhoto?email=sadie@contoso.com&amp;size=HR240x240") 
   as HttpWebRequest;
// Submit the request.
using (HttpWebResponse resp = request.GetResponse() as HttpWebResponse)
{
   // Take the response and save it as an image.
   Bitmap image = new Bitmap(resp.GetResponseStream());
   image.Save("Sadie.jpg");
}

```

A solicitação retornará uma resposta HTTP. 
  
**Tabela 2. Códigos de resposta para uma solicitação GetUserPhoto**

|**Código de resposta**|**Descrição**|
|:-----|:-----|
|200  <br/> |Uma imagem está disponível para a conta de email especificada e a imagem binária está contida na resposta.  <br/> |
|304  <br/> |A imagem não foi alterada desde a última vez que **ETag** foi retornado para o aplicativo.  <br/> |
|404  <br/> |Nenhuma imagem está disponível para a conta de email especificada.  <br/> |

<a name="bk_REST"> </a>

## <a name="cache-user-photos"></a>Armazenar em cache fotos do usuário

O Exchange retorna os dados com um tipo de conteúdo image/jpeg, juntamente com uma coleção de valores de cabeçalho. O cabeçalho **ETag** é semelhante a uma chave de alteração. O valor é uma cadeia de caracteres que representa a última vez que a foto foi atualizada. A **ETag** permanece a mesma para a foto do usuário até que a foto seja alterada. Você pode enviar esse valor de **ETag** para o servidor na solicitação **Get** de HTTPS em um cabeçalho **If-None-Match** . Se a foto não tiver sido alterada desde a última solicitação, o servidor responderá com uma resposta HTTP 304 que indica como tal. Isso significa que você pode usar a foto do usuário que você solicitou e salvou anteriormente, em vez de processar um novo. 

<a name="bk_EWSMA"> </a>

## <a name="get-a-contact-user-photo-by-using-ews-managed-api"></a>Obter uma foto de usuário de contato usando a API gerenciada do EWS

Seu aplicativo pode usar a API gerenciada do EWS para recuperar fotos de contatos, se o contato estiver armazenado em uma pasta de contatos na caixa de correio do usuário. Para fazer isso, primeiro, encontre o **ItemId** do contato que você deseja usar. Depois, depois de associar a esse contato, carregue-o na coleção Attachments. Se o contato tiver uma foto, a foto será um dos anexos. Percorra a coleção Attachments, verificando o valor da propriedade **IsContactPhoto** . Quando você encontrar a foto do contato, poderá salvá-la no computador local e o aplicativo poderá acessá-la. 
  
O exemplo a seguir mostra esse processo. Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange. 
  
```cs
private static void GetContactPhoto(ExchangeService service, string ItemId)
{
   // Bind to an existing contact by using the ItemId passed into this function.
   Contact contact = Contact.Bind(service, ItemId);
   // Load the contact to get access to the collection of attachments.
   contact.Load(new PropertySet(ContactSchema.Attachments));
   // Loop through the attachments looking for a contact photo.
   foreach (Attachment attachment in contact.Attachments)
   {
      if ((attachment as FileAttachment).IsContactPhoto)
      {
         // Load the attachment to access the content.
         attachment.Load();
      }
   }
   FileAttachment photo = contact.GetContactPictureAttachment();
   // Create a file stream and save the contact photo to your computer.
   using (FileStream file = new FileStream(photo.Name, FileMode.Create, System.IO.FileAccess.Write))
   {
      photo.Load(file);
   }
}

```

<a name="bk_EWS"> </a>

## <a name="get-a-user-photo-by-using-ews"></a>Obter uma foto do usuário usando o EWS

Se você estiver obtendo uma foto de usuário do AD DS, poderá usar a operação [GetUserPhoto](https://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) (se souber o endereço de email) ou a operação [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) (se não souber o endereço de email). Se você estiver obtendo uma foto de usuário de uma pasta contatos na caixa de correio, use a operação [GetItem](https://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) seguida pela operação [GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) . Em ambos os casos, a foto é retornada como uma cadeia de caracteres codificada em base64 na resposta XML. 
  
### <a name="get-a-mailbox-user-photo-by-using-the-getuserphoto-operation"></a>Obter uma foto de usuário de caixa de correio usando a operação GetUserPhoto

O uso da operação **GetUserPhoto** é simples. Na solicitação XML, especifique o endereço de email do usuário e o [tamanho da foto](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) a ser retornado (no elemento [SizeRequested](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) ). O exemplo de solicitação XML a seguir mostra como obter uma foto para Sadie Daniels de 360 pixels de largura por 360 pixels de altura. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013 "/>
   </soap:Header>
   <soap:Body>
      <m:GetUserPhoto>
         <m:Email>sadie@contoso.com</m:Email>
         <m:SizeRequested>HR360x360</m:SizeRequested>
      </m:GetUserPhoto>
   </soap:Body>
</soap:Envelope>

```

Veja a seguir a resposta de XML. A foto codificada em base64 está contida no elemento [PictureData](https://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) (o conteúdo foi reduzido para facilitar a leitura). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetUserPhotoResponse ResponseClass="Success" 
         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <HasChanged>true</HasChanged>
      <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg... wATRRRSuB//2Q==</PictureData>
    </GetUserPhotoResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-mailbox-user-photo-by-using-the-resolvenames-operation"></a>Obter uma foto de usuário de caixa de correio usando a operação ResolveNames

Se você não souber o endereço de email do usuário para o qual você está obtendo uma foto, poderá [usar a operação ResolveNames](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md) para obter candidatos para uma possível correspondência. Se você especificar "myproperties" para o atributo **ContactDataShape** do elemento [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) , muitos dados, incluindo as fotos do usuário, serão retornados para cada candidato. O exemplo a seguir mostra a solicitação XML para resolver o nome "Sadie" e retornar todas as propriedades de cada candidato. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
<soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>  
<soap:Body>
  <m:ResolveNames ReturnFullContactData="true" ContactDataShape="AllProperties">
      <m:UnresolvedEntry>sadie</m:UnresolvedEntry>
    </m:ResolveNames>
  </soap:Body>
</soap:Envelope>
```

Um grande volume de dados será retornado na resposta. O exemplo a seguir mostra somente os dados relevantes para a foto do usuário. O elemento **Photo** contém a foto de usuário codificada em Base64 (o conteúdo foi reduzido para facilitar a leitura). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>Sadie Daniels</t:Name>
                <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>Sadie Daniels</t:DisplayName>
                <t:GivenName>Sadie</t:GivenName>
                <t:Initials/>
                <t:CompanyName>CONTOSO</t:CompanyName>
......
                <t:Photo>/9j/4AAQSkZJRgABAQE...qKKKAP/2Q==</t:Photo>
......
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </m:ResolveNamesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-contact-user-photo-by-using-the-getattachment-operation"></a>Obter uma foto de usuário de contato usando a operação GetAttachment

Você pode usar o EWS para obter fotos de contatos armazenados na sua caixa de correio. Primeiro, use a operação **GetItem** para retornar todas as propriedades para que você possa procurar fotos. O exemplo a seguir mostra uma solicitação XML para obter um item de contato. A ID do item foi reduzida para legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='https://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAAGECXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AABLzXRv"/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>

```

Procure o elemento [HasPicture](https://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) para verificar se o contato tem uma foto associada. Em seguida, examine a coleção de anexos para um que tenha um valor de true para o elemento [IsContactPhoto](https://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) . O exemplo de resposta a seguir mostra apenas os dados relevantes. Os valores de ID são reduzidos para legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAAGECXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AABLzXRv"/>
              <t:ParentFolderId Id="nIxIAAA=" ChangeKey="AQAAAA=="/>
              <t:ItemClass>IPM.Contact</t:ItemClass>
              <t:Subject>Hope Gross</t:Subject>
              <t:Sensitivity>Normal</t:Sensitivity>
......
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="1LGlhgpgoA="/>
                  <t:Name>ContactPicture.jpg</t:Name>
                  <t:Size>6260</t:Size>
                  <t:LastModifiedTime>2011-03-09T16:55:55</t:LastModifiedTime>
                  <t:IsInline>false</t:IsInline>
                  <t:IsContactPhoto>true</t:IsContactPhoto>
                </t:FileAttachment>
              </t:Attachments>
......
              <t:HasPicture>true</t:HasPicture>
            </t:Contact>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

Em seguida, use a operação **GetAttachment** com o **attachmentid** para solicitar o anexo que tem a foto de contato. O exemplo a seguir mostra a solicitação XML para obter o anexo. A ID é reduzida para legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
         <t:AttachmentId Id="1LGlhgpgoA="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>

```

O exemplo a seguir mostra a resposta XML com as informações sobre o anexo solicitado. O elemento [Content](https://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) contém a cadeia de caracteres codificada em base64 para a foto do usuário, abreviado neste exemplo para legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="+KsDBEr1LGlhgpgoA="/>
              <t:Name>ContactPicture.jpg</t:Name>
              <t:Content>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg...D//2Q==</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:GetAttachmentResponse>
  </s:Body>
</s:Envelope>

```

<a name="bk_EWS"> </a>

## <a name="decode-a-base64-encoded-string"></a>Decodificar uma cadeia de caracteres codificada em base64

Independentemente da operação que você usa para obter uma foto do usuário, você precisará decodificar essa cadeia de caracteres para usá-la em seu aplicativo. O exemplo a seguir mostra como decodificar a cadeia de caracteres e, em seguida, salvá-la no computador local para que o aplicativo possa acessá-la mais tarde.
  
```cs
// Convert the encoded string into a byte array.
byte[] data = System.Convert.FromBase64String(Photo);
// Create a memory stream to read the data.
MemoryStream ms = new MemoryStream(data);
// Save the data on your local computer as a JPG image.
using (FileStream file = new FileStream(ContactName + ".jpg", FileMode.Create, System.IO.FileAccess.Write))
{
   byte[] bytes = new byte[ms.Length];
   ms.Read(bytes, 0, (int)ms.Length);
   file.Write(bytes, 0, bytes.Length);
   ms.Close();
}

```

## <a name="see-also"></a>Confira também

- [Pessoas e contatos no EWS no Exchange](people-and-contacts-in-ews-in-exchange.md)    
- [Resolver nomes ambíguos usando o EWS no Exchange 2013](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)    
- [Processar contatos em lotes usando o EWS no Exchange](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    

