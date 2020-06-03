---
title: Exportar itens usando o EWS no Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: e93ee68c-e134-4469-9070-fba404d46cb4
description: Saiba como exportar compromissos, emails, contatos, tarefas e outros itens usando a API gerenciada do EWS ou o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: a01c9487821958b06ec162f2aee27e2d2804eaaf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455881"
---
# <a name="export-items-by-using-ews-in-exchange"></a>Exportar itens usando o EWS no Exchange

Saiba como exportar compromissos, emails, contatos, tarefas e outros itens usando a API gerenciada do EWS ou o EWS no Exchange.
  
Você pode exportar itens do Exchange usando a API gerenciada do EWS ou o EWS de várias maneiras diferentes. A opção que você usa depende:
  
- O tipo de item que é exportado.
    
- O grau de fidelidade que você deseja manter entre o estado do item no Exchange e o item exportado.
    
- O formato do item exportado.
    
- Todos os requisitos de pós-processamento.
    
- Se você deseja importar o item de volta para o Exchange.
    
Este artigo mostra como usar cada uma das diferentes opções para exportar itens. Você pode usar qualquer opção para exportar itens em lotes do Exchange.
  
## <a name="export-an-item-into-a-custom-format"></a>Exportar um item para um formato personalizado
<a name="bk_exportcustom"> </a>

Você pode usar os resultados de um [Item. vincule](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) a chamada de método de API gerenciada do EWS ou analise os resultados de uma operação do EWS do [GetItem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) em um formato que funciona com seus requisitos de aplicativo. Use essa opção quando você estiver exportando itens para importá-los para um banco de dados, um arquivo. csv ou outro formato ou sistema. Você pode até mesmo salvar o item no formato do item EWS XML, que pode ser útil porque muitos sistemas têm capacidade de análise XML. Recomendamos que você use o método **Item. bind** ou a operação **GetItem** (sem a propriedade [Item. MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) ) porque essa opção dá controle sobre quais propriedades são exportadas. 
  
## <a name="export-items-with-full-fidelity"></a>Exportar itens com fidelidade total
<a name="bk_exportfullfidelity"> </a>

Se você quiser exportar itens com fidelidade total, poderá usar a operação [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) do EWS. A operação **ExportItems** exporta cada item como um fluxo de dados. Esse fluxo de dados não é para análise, mas pode ser usado como um backup de nível de item que pode ser importado de volta para uma caixa de correio do Exchange. Você pode incluir muitos itens em cada solicitação **ExportItems** , embora seja recomendável que você não inclua mais de 100 itens em cada chamada. Como a API gerenciada do EWS não implementa a operação **ExportItems** , se você usar a API gerenciada do EWS, você precisará escrever uma rotina para enviar as solicitações da Web. Opcionalmente, você pode usar o método [Item. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) para obter metadados sobre o item para que você possa indexar e armazenar informações sobre o fluxo de dados. 
  
Recomendamos que você use a operação **ExportItems** para exportar itens que você planeja importar para uma caixa de correio do Exchange. 
  
O exemplo a seguir mostra como usar a operação **ExportItems** . Neste exemplo, o identificador de item é reduzido para facilitar a leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

O servidor responde à solicitação **ExportItems** com um elemento [ExportItemsResponse](https://msdn.microsoft.com/library/ef44354b-fbdb-4f7c-b6bd-b27f56a1d018%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que o item foi exportado com êxito. A resposta também inclui a ID do item exportado e o fluxo de dados que contém o conteúdo exportado. O exemplo a seguir mostra o corpo SOAP que contém o item exportado.
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:ExportItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="use-the-mime-stream-to-export-into-common-file-formats"></a>Usar o fluxo MIME para exportar para formatos de arquivo comuns
<a name="bk_exportfullfidelity"> </a>

Você pode usar o método [Item. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) de API gerenciada do EWS ou a operação [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS para obter uma representação MIME de um item. Como o Exchange não armazena o conteúdo MIME de cada item, ele precisa converter a representação de banco de dados de cada item no fluxo MIME. Como essa conversão é cara, não recomendamos que você solicite o fluxo MIME para itens em uma escala grande. Observe também que o fluxo MIME contém um conjunto limitado de propriedades; Você pode ter que considerar outras opções se o conjunto de propriedades não contiver as propriedades que você precisa. 
  
### <a name="use-the-ews-managed-api-to-export-an-email-into-an-eml-and-mht-file-by-using-the-mime-stream"></a>Use a API gerenciada do EWS para exportar um email para um arquivo. eml e. mht usando o fluxo MIME
<a name="bk_exportemailmime"> </a>

O Outlook e outros aplicativos de email comuns podem abrir o formato de arquivo EML (. eml). O exemplo a seguir mostra como você pode exportar um email usando o fluxo MIME e usar o fluxo MIME para criar um arquivo EML e HTML (. mht). Muitos navegadores da Web oferecem suporte ao formato de arquivo MIME HTML. Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário pode autenticar em um servidor Exchange. 
  
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

### <a name="use-the-ews-managed-api-to-export-an-appointment-into-an-ical-file-by-using-the-mime-stream"></a>Usar a API gerenciada do EWS para exportar um compromisso para um arquivo iCal usando o fluxo MIME
<a name="bk_exporticalmime"> </a>

O Outlook e outros aplicativos de calendário comuns podem abrir o formato de arquivo iCal (. ICS). O exemplo a seguir mostra como exportar um compromisso usando o fluxo MIME e usar o fluxo MIME para criar um arquivo iCal. Observe que muitas propriedades não são exportadas com o fluxo MIME, incluindo participantes e propriedades relacionadas a anexos. Você pode capturar outras propriedades do EWS solicitando-as e salvando-as no arquivo iCal como extensões privadas. Essas extensões privadas são prefixadas com "x-". 
  
Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário pode autenticar em um servidor Exchange. Este exemplo também pressupõe que você tenha um compromisso com o assunto "projeções financeiras 2015" na pasta calendário. 
  
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

### <a name="use-the-ews-managed-api-to-export-a-contact-into-a-vcard-file-by-using-the-mime-stream"></a>Usar a API gerenciada do EWS para exportar um contato para um arquivo vCard usando o fluxo MIME
<a name="bk_exportvcardmime"> </a>

O Outlook e outros aplicativos de gerenciamento de contato comuns podem abrir o formato de arquivo vCard (. vcf). O exemplo a seguir mostra como exportar um contato usando o fluxo MIME e usar o fluxo MIME para criar um vCard. Você pode capturar outras propriedades do EWS solicitando-as e salvando-as no. vCard como extensões privadas. Essas extensões são prefixadas com "x-". 
  
Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário pode autenticar em um servidor Exchange. 
  
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
> Não é possível importar arquivos vCard usando a propriedade **MimeContent** . Você pode importar contatos usando o [contato. salvar](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) o método de API gerenciada do EWS ou a operação [CreateItem](https://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) do EWS. 
  
### <a name="use-ews-to-export-any-item-by-using-the-mime-stream"></a>Usar o EWS para exportar qualquer item usando o fluxo MIME
<a name="bk_exportewsmime"> </a>

Use a operação **GetItem** para obter o fluxo MIME de um item. A solicitação **GetItem** a seguir mostra como solicitar o conteúdo MIME de um item. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

O exemplo a seguir mostra a resposta a uma solicitação para obter o fluxo MIME. O fluxo MIME foi reduzido para legibilidade.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="893" 
                         MinorBuildNumber="17" 
                         Version="V2_10" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Após exportar itens, talvez você queira [importar itens para o Exchange](how-to-import-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>Confira também


- [Exportando e importando itens usando o EWS no Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [Importar itens usando o EWS no Exchange](how-to-import-items-by-using-ews-in-exchange.md)
    
- [Pastas e itens no EWS no Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Sincronização de caixa de correio e EWS no Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

