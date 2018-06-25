---
title: Exportar itens usando o EWS no Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e93ee68c-e134-4469-9070-fba404d46cb4
description: Saiba como exportar compromissos, emails, contatos, tarefas e outros itens usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 65b5b2ef1eba66877d5b6f6c3d4237a26a254196
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750720"
---
# <a name="export-items-by-using-ews-in-exchange"></a>Exportar itens usando o EWS no Exchange

Saiba como exportar compromissos, emails, contatos, tarefas e outros itens usando a API gerenciada de EWS ou EWS no Exchange.
  
Você pode exportar itens do Exchange usando a API gerenciada de EWS ou EWS em um número de formas diferentes. A opção que você usar depende de:
  
- O tipo de item que será exportado.
    
- O grau de fidelidade que deseja manter entre o estado de item no Exchange e o item exportado.
    
- O formato do item exportado.
    
- Quaisquer requisitos de pós-processamento.
    
- Se você deseja importar o item de volta para o Exchange.
    
Este artigo mostra como usar cada uma das opções diferentes para exportar itens. Você pode usar qualquer opção para exportar itens do Exchange de lote.
  
## <a name="export-an-item-into-a-custom-format"></a>Exportar um item em um formato personalizado
<a name="bk_exportcustom"> </a>

Você pode usar os resultados de uma chamada de método de API gerenciada de EWS [Item.Bind](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) ou analisar os resultados de uma operação de EWS [GetItem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) em um formato que funciona com os requisitos de aplicativos. Use esta opção quando você está exportando itens para importá-los para um banco de dados, arquivos. csv, ou outro formato ou sistema. Você pode até mesmo salvar o item no formato do item EWS XML, que pode ser útil porque muitos sistemas têm a capacidade de análise de XML. Recomendamos que você use o método **Item.Bind** ou a operação de **GetItem** (sem a propriedade [Item.MimeContent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) ) porque essa opção lhe dá controle sobre quais propriedades serão exportadas. 
  
## <a name="export-items-with-full-fidelity"></a>Exportar itens com fidelidade total
<a name="bk_exportfullfidelity"> </a>

Se você deseja exportar itens com fidelidade total, você pode usar a operação de EWS [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) . A operação **ExportItems** exporta cada item como um fluxo de dados. Este fluxo de dados não é para análise, mas pode ser usado como um backup de nível de item que pode ser importado novamente para uma caixa de correio do Exchange. Você pode incluir o número de itens em cada solicitação de **ExportItems** , embora seja recomendável que você inclua não mais de 100 itens em cada chamada. Porque a API gerenciada de EWS não implementa a operação **ExportItems** , se você usar a API gerenciada de EWS, você precisará gravar uma rotina para enviar as solicitações da web. Opcionalmente, você pode usar o método [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) obter metadados sobre o item para que você possa indexar e armazenar informações sobre o fluxo de dados. 
  
Recomendamos que você use a operação **ExportItems** para exportar itens que você planeja importar para uma caixa de correio do Exchange. 
  
O exemplo a seguir mostra como usar a operação **ExportItems** . Neste exemplo, o identificador do item é abreviado para fins de legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013"/>
  </soap:Header>
  <soap:Body>
    <m:ExportItems>
      <m:ItemIds>
        <t:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89GAAA="/>
      </m:ItemIds>
    </m:ExportItems>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **ExportItems** com um elemento [ExportItemsResponse](http://msdn.microsoft.com/library/ef44354b-fbdb-4f7c-b6bd-b27f56a1d018%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que o item foi exportado com sucesso. A resposta também inclui a ID de item do item exportado e o fluxo de dados que contém o conteúdo exportado. O exemplo a seguir mostra o corpo SOAP que contenha o item exportado.
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:ExportItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
    <m:ResponseMessages>
      <m:ExportItemsResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89GAAA=" ChangeKey="FwAAAA=="/>
        <m:Data>
          AQAAAAgAAAAAAAAALgBlAHgAdABlAHMAdAAuAG0AaQBjAHIAbwBzAG8AZgB0AC4A
          cgAyAEAAYQB1AGoAaQBuAGcALQBkAG8AbQAuAGUAeAB0AGUAcwB0AC4AbQBpAGMAcgBvAHMA
          bwBmAHQALgBjAG8AbQAAAAMAADkAAAAAAwD+DwYAAAADAARAAwACQAMADkA=
        </m:Data>
      </m:ExportItemsResponseMessage>
     </m:ResponseMessages>
  </m:ExportItemsResponse>
</s:Body>
```

## <a name="use-the-mime-stream-to-export-into-common-file-formats"></a>Use o fluxo MIME para exportar em formatos de arquivo comuns
<a name="bk_exportfullfidelity"> </a>

Você pode usar o método de API gerenciada de EWS [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) ou a operação de EWS [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) para obter uma representação de MIME de um item. Porque o Exchange não armazena o conteúdo MIME de cada item, ele deve converter uma representação de banco de dados de cada item no fluxo de MIME. Como essa conversão é dispendiosa, que não é recomendável que você solicitar o fluxo MIME para itens em grande escala. Observe também que o fluxo MIME contém um conjunto limitado de propriedades; Você pode precisar considerar outras opções, se o conjunto de propriedades não contém as propriedades que você precisa. 
  
### <a name="use-the-ews-managed-api-to-export-an-email-into-an-eml-and-mht-file-by-using-the-mime-stream"></a>Use a API gerenciada de EWS para exportar um email em um arquivo. eml e. mht usando o fluxo MIME
<a name="bk_exportemailmime"> </a>

Outlook e outros aplicativos de email comuns podem abrir o formato de arquivo EML (. eml). O exemplo a seguir mostra como você pode exportar um email usando o fluxo MIME e usa o fluxo de MIME para criar um EML e um arquivo de MIME HTML (. mht). O formato de arquivo MIME HTML suportam a vários navegadores da web. Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário pode autenticar em um servidor Exchange. 
  
```cs
private static void ExportMIMEEmail(ExchangeService service)
{
    Folder inbox = Folder.Bind(service, WellKnownFolderName.Inbox);
    ItemView view = new ItemView(1);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly);
    // This results in a FindItem call to EWS.
    FindItemsResults<Item> results = inbox.FindItems(view);
    foreach (var item in results)
    { 
        PropertySet props = new PropertySet(EmailMessageSchema.MimeContent);
        // This results in a GetItem call to EWS.
        var email = EmailMessage.Bind(service, item.Id, props);
                
        string emlFileName = @"C:\export\email.eml";
        string mhtFileName = @"C:\export\email.mht";
        // Save as .eml.
        using (FileStream fs = new FileStream(emlFileName, FileMode.Create, FileAccess.Write))
        {
            fs.Write(email.MimeContent.Content, 0, email.MimeContent.Content.Length);
        }
        // Save as .mht.
        using (FileStream fs = new FileStream(mhtFileName, FileMode.Create, FileAccess.Write))
        {
            fs.Write(email.MimeContent.Content, 0, email.MimeContent.Content.Length);
        }
    }
}
```

### <a name="use-the-ews-managed-api-to-export-an-appointment-into-an-ical-file-by-using-the-mime-stream"></a>Use a API gerenciada de EWS para exportar um compromisso em um arquivo iCal usando o fluxo MIME
<a name="bk_exporticalmime"> </a>

Outlook e outros aplicativos de calendário comuns podem abrir o formato de arquivo iCalendar (. ICS). O exemplo a seguir mostra como exportar um compromisso usando-se o fluxo MIME e usa o fluxo de MIME para criar um arquivo iCal. Observe que muitas propriedades não são exportadas com o fluxo MIME, incluindo os participantes e propriedades relacionadas ao anexo. Você pode capturar outras propriedades do EWS solicitando-los e salvá-los no arquivo iCal como extensões privadas. Essas extensões privadas são prefixados com "x-". 
  
Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário pode autenticar em um servidor Exchange. Este exemplo também pressupõe que você tenha um compromisso com o assunto "2015 financeiros projeções" na pasta de calendário. 
  
```cs
private static void ExportMIMEAppointment(ExchangeService service)
{
    Folder inbox = Folder.Bind(service, WellKnownFolderName.Calendar);
    ItemView view = new ItemView(1);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly); 
    // This results in a FindItem call to EWS.
    FindItemsResults<Item> results = inbox.FindItems("subject:'2015 Financial Projections'", view);
    foreach (var item in results)
    {
        PropertySet props = new PropertySet(AppointmentSchema.MimeContent);
        // This results in a GetItem call to EWS.
        var email = Appointment.Bind(service, item.Id, props);
        string iCalFileName = @"C:\export\appointment.ics";
        // Save as .ics.
        using (FileStream fs = new FileStream(iCalFileName, FileMode.Create, FileAccess.Write))
        {
            fs.Write(email.MimeContent.Content, 0, email.MimeContent.Content.Length);
        }
    }
}
```

### <a name="use-the-ews-managed-api-to-export-a-contact-into-a-vcard-file-by-using-the-mime-stream"></a>Use a API gerenciada de EWS para exportar um contato em um arquivo vCard usando o fluxo MIME
<a name="bk_exportvcardmime"> </a>

Outlook e outros aplicativos comuns de gerenciamento de contatos podem abrir o formato de arquivo vCard (. vcf). O exemplo a seguir mostra como exportar um contato usando o fluxo MIME e usa o fluxo de MIME para criar um vCard. Você pode capturar outras propriedades do EWS solicitando-los e salvá-los na. vCard como extensões privadas. Essas extensões são prefixados com "x-". 
  
Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário pode autenticar em um servidor Exchange. 
  
```cs
private static void ExportMIMEContact(ExchangeService service)
{
    Folder inbox = Folder.Bind(service, WellKnownFolderName.Contacts);
    ItemView view = new ItemView(1);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly);
    // This results in a FindItem call to EWS.
    FindItemsResults<Item> results = inbox.FindItems(view);
    foreach (var item in results)
    {
        PropertySet props = new PropertySet(ContactSchema.MimeContent);
        // This results in a GetItem call to EWS.
        var email = Contact.Bind(service, item.Id, props);
        string vcfFileName = @"C:\export\contact.vcf";
        // Save as .vcf.
        using (FileStream fs = new FileStream(vcfFileName, FileMode.Create, FileAccess.Write))
        {
            fs.Write(email.MimeContent.Content, 0, email.MimeContent.Content.Length);
        }
    }
}
```

> [!NOTE]
> Você não pode importar arquivos vCard usando a propriedade **MimeContent** . Você pode importar contatos usando o método de API gerenciada de EWS [Contact.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) ou a operação de EWS [CreateItem](http://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) . 
  
### <a name="use-ews-to-export-any-item-by-using-the-mime-stream"></a>Use o EWS para exportar qualquer item usando o fluxo MIME
<a name="bk_exportewsmime"> </a>

Use a operação **GetItem** para obter o fluxo MIME de um item. A solicitação de **GetItem** a seguir mostra como solicitar o conteúdo MIME de um item. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkADEzYjJkLTYxMwB8GqYicWAAA=" ChangeKey="CQAAABzXv"/>
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

O exemplo a seguir mostra a resposta a uma solicitação para obter o fluxo MIME. O fluxo MIME foi reduzido para melhorar a legibilidade.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="893" 
                         MinorBuildNumber="17" 
                         Version="V2_10" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:MimeContent CharacterSet="UTF-8">UmVjZ6IGZyb2b2suY29y5hMzgwZTA1YtDQo=</t:MimeContent>
              <t:ItemId Id="AAMkADEzYjJkLTYxMwB8GqYicWAAA=" ChangeKey="CQAAABzXv"/>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## 
<a name="bk_exportfullfidelity"> </a>

Após exportar itens, talvez você queira [Importar itens para o Exchange](how-to-import-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>Confira também


- [Exportando e importando itens usando o EWS no Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [Importar itens usando o EWS no Exchange](how-to-import-items-by-using-ews-in-exchange.md)
    
- [Pastas e itens no EWS no Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Sincronização de caixa de correio e EWS no Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

