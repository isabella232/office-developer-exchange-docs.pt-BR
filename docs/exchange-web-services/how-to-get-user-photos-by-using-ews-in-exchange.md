---
title: Obtenha as fotos de usuários usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f86d1099-1f57-47dc-abf2-4d5ae4e900a9
description: Saiba como obter fotos dos usuários que estão associados uma caixa de correio ou contato usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: f0f5cddd41fc563fb9ed38e75b505830a3992411
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750755"
---
# <a name="get-user-photos-by-using-ews-in-exchange"></a>Obtenha as fotos de usuários usando o EWS no Exchange

Saiba como obter fotos dos usuários que estão associados uma caixa de correio ou contato usando a API gerenciada de EWS ou EWS no Exchange.
  
É bom colocar uma face para um nome. Se seus usuários, como colocar nomes às faces, seu aplicativo pode solicitar uma imagem, normalmente uma foto do Exchange que representa uma conta de email. Você pode obter uma foto de usuário armazenada em um servidor do Exchange para uma caixa de correio ou você pode obter uma foto do contato do contatos armazenados na sua caixa de correio.
  
Você pode usar diversas tecnologias para obtenção de fotos de caixas de correio ou os serviços de domínio Active Directory (AD DS). A melhor maneira de obter uma foto depende do tipo de contato que você deseja obter uma foto de. 
  
**Tabela 1. Tecnologias usar para obter as fotos de usuários com base no tipo de contato**

|**Tipo de contato**|**Tecnologias usar**|
|:-----|:-----|
|Foto do usuário de caixa de correio  <br/> |[Obtenha uma foto do usuário de caixa de correio usando REST](#bk_REST)<br/><br/> [Obtenha uma foto do usuário usando o EWS](#bk_EWS) <br/> |
|Fotos de contatos do usuário  <br/> |[Obtenha uma foto do contato de usuário usando a API gerenciada de EWS](#bk_EWSMA)<br/><br/> [Obtenha uma foto do usuário usando o EWS](#bk_EWS) <br/> |

<a name="bk_REST"> </a>

## <a name="get-a-mailbox-user-photo-by-using-rest"></a>Obtenha uma foto do usuário de caixa de correio usando REST

Você poderá solicitar fotos dos usuários de um servidor do Exchange usando uma solicitação HTTPS **GET** padrão. Na solicitação, especifique o endereço da conta de email e um código de tamanho para a imagem, conforme mostrado no exemplo a seguir. 
  
```HTML
https://Exchange Server/ews/Exchange.asmx/s/GetUserPhoto?email=email address&amp;size=size code
```

Use a operação de [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) de serviço de descoberta automática para recuperar a configuração de **ExternalEwsUrl** , que contém a URL do ponto de extremidade de serviços Web do Exchange (EWS) e a localização do manipulador **Exchange.asmx** HTTP que retorna o fotos dos usuários. 
  
Cada código de tamanho indica a altura e largura da imagem em pixels. Por exemplo, o código de tamanho **HR48x48** retorna uma imagem que é 48 pixels de altura por 48 pixels de largura. Os valores possíveis para o parâmetro de código de tamanho são iguais os valores possíveis para o elemento [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) . Se a solicitação especifica um tamanho que não está disponível, a foto disponível maior será retornada. Se nenhuma foto está armazenada no servidor Exchange, a imagem em miniatura armazenada no AD DS para a conta será retornada. 
  
> [!NOTE]
> O código de tamanho **HR48x48** sempre retorna a imagem em miniatura do AD DS, se ele estiver disponível. 
  
O exemplo a seguir mostra como você pode usar a solicitação GET para recuperar a foto do usuário para Sadie e salve-o em seu computador local.
  
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
  
**Tabela 2. Códigos de resposta para uma solicitação de GetUserPhoto**

|**Código de resposta**|**Descrição**|
|:-----|:-----|
|200  <br/> |Uma imagem está disponível para a conta de email especificada e a imagem binária está contida na resposta.  <br/> |
|304  <br/> |A imagem não tiver sido alterado desde a última vez em que a **ETag** foi retornado para o aplicativo.  <br/> |
|404  <br/> |Nenhuma imagem está disponível para a conta de email especificada.  <br/> |

<a name="bk_REST"> </a>

## <a name="cache-user-photos"></a>Fotos de usuário de cache

Exchange retorna os dados com um tipo de conteúdo de image/jpeg, juntamente com uma coleção de valores de cabeçalho. O cabeçalho **ETag** é semelhante a uma chave de alteração. O valor é uma cadeia de caracteres que representa a última vez em que a foto foi atualizada. A **ETag** permanece as mesmas para a foto do usuário, até que a foto seja alterada. Você pode enviar esse valor **ETag** para o servidor na solicitação de HTTPS **obter** um cabeçalho **If-None-Match** . Se a foto não mudou desde a última solicitação, o servidor responderá com uma resposta de HTTP 304 que indica como tal. Isso significa que você pode usar a foto do usuário que você solicitou e salvo anteriormente, em vez do processamento de um novo. 

<a name="bk_EWSMA"> </a>

## <a name="get-a-contact-user-photo-by-using-ews-managed-api"></a>Obtenha uma foto do contato de usuário usando a API gerenciada de EWS

Seu aplicativo pode usar a API gerenciada de EWS para recuperar as fotos de contatos, se o contato estiver armazenado em uma pasta de contato na caixa de correio do usuário. Para fazer isso, primeiro, encontre o **ItemId** para o contato que você deseja usar. Em seguida, depois que você associar a esse contato, carregá-lo à coleção attachments. Se o contato tiver uma foto, a foto será um dos anexos. Loop através da coleção de anexos, verificando o valor da propriedade **IsContactPhoto** . Quando você encontrar a foto do contato, você poderá salvá-lo ao computador local, e seu aplicativo pode acessá-lo. 
  
O exemplo a seguir mostra esse processo. Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange. 
  
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

## <a name="get-a-user-photo-by-using-ews"></a>Obtenha uma foto do usuário usando o EWS

Se estiver recebendo uma foto do usuário do AD DS, você pode usar a operação de [GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) (se você sabe o endereço de email) ou a operação [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) (se você não souber o endereço de email). Se estiver recebendo uma foto do usuário de uma pasta de contatos na caixa de correio, use a operação de [GetItem](http://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) seguida da operação [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) . Em ambos os casos, a foto é retornada como uma cadeia de caracteres codificado na Base64 na resposta XML. 
  
### <a name="get-a-mailbox-user-photo-by-using-the-getuserphoto-operation"></a>Obtenha uma foto do usuário de caixa de correio usando a operação GetUserPhoto

Usando a operação **GetUserPhoto** é simples. Na solicitação XML, especifique o endereço de email do usuário e o [tamanho da foto](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) para retornar (no elemento [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) ). O exemplo de solicitação XML a seguir mostra como obter uma foto para Sadie Daniels que é de 360 pixels de largura por 360 pixels de altura. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

Veja a seguir a resposta XML. A foto codificado na Base64 está contida no elemento [PictureData](http://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) (o conteúdo foi reduzido para facilitar a leitura). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetUserPhotoResponse ResponseClass="Success" 
         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <HasChanged>true</HasChanged>
      <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg... wATRRRSuB//2Q==</PictureData>
    </GetUserPhotoResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-mailbox-user-photo-by-using-the-resolvenames-operation"></a>Obtenha uma foto do usuário de caixa de correio usando a operação ResolveNames

Se você não souber o endereço de email do usuário para quem você está recebendo uma foto, você pode [usar a operação ResolveNames](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md) para obter candidatos para uma correspondência possível. Se você especificar "AllProperties" para o atributo **ContactDataShape** do elemento [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) , muitos dados, incluindo as fotos de usuários, serão retornado para cada candidato. O exemplo a seguir mostra a solicitação XML para resolver o nome "Sadie" e retornar todas as propriedades para cada candidato. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Muitos dados serão retornados na resposta. O exemplo a seguir mostra somente os dados que são relevantes para a foto do usuário. O elemento de **fotos** contém a foto do usuário codificado na Base64 (o conteúdo foi reduzido para facilitar a leitura). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="get-a-contact-user-photo-by-using-the-getattachment-operation"></a>Obtenha uma foto do contato de usuário usando a operação GetAttachment

Você pode usar o EWS para obtenção de fotos de contatos armazenados na sua caixa de correio. Primeiro, você deve usar a operação **GetItem** para retornar todas as propriedades para que você pode procurar por fotos. O exemplo a seguir mostra uma solicitação XML para obter um item de contato. A ID do item foi reduzida para melhorar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
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

Procure o elemento [HasPicture](http://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) verificar se o contato tem uma foto associada. Procure por meio da coleção de anexos que possui um valor true para o elemento [IsContactPhoto](http://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) . O exemplo de resposta a seguir mostra somente os dados relevantes. Os valores de ID são reduzidos para melhorar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Em seguida, use a operação de **GetAttachment** com o **AttachmentId** para solicitar o anexo que tem a foto do contato. O exemplo a seguir mostra a solicitação XML para obter o anexo. A ID é abreviada para fins de legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
         <t:AttachmentId Id="1LGlhgpgoA="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>

```

O exemplo a seguir mostra a resposta XML com as informações sobre o anexo que você solicitou. O elemento de [conteúdo](http://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) contém a cadeia de caracteres codificado na Base64 para a foto do usuário, abreviada neste exemplo, para fins de legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="decode-a-base64-encoded-string"></a>Decodificar uma cadeia de caracteres codificado na Base64

Independentemente da operação que você usar para obter uma foto do usuário, você precisará decodificar essa cadeia de caracteres, para que possa usá-lo em seu aplicativo. O exemplo a seguir mostra como decodificar a cadeia de caracteres e, em seguida, salvá-lo ao computador local para que o aplicativo você pode acessá-lo mais tarde.
  
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
- [Resolver nomes de ambíguos, usando o EWS no Exchange 2013](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)    
- [Contatos de processo em lotes, usando o EWS no Exchange](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    

