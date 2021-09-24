---
title: Importar itens usando o EWS em Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: dd3d3221-c98e-4fa0-81f0-77f733d2f432
description: Saiba como importar compromissos, emails, contatos, tarefas e outros itens usando a API Gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 1e111a03f43c7c6ea30ab0dedf5cc0bb5c6a41f8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513161"
---
# <a name="import-items-by-using-ews-in-exchange"></a>Importar itens usando o EWS em Exchange

Saiba como importar compromissos, emails, contatos, tarefas e outros itens usando a API Gerenciada do EWS ou o EWS no Exchange.
  
Muitos sistemas contêm compromissos, emails, contatos e tarefas, e você pode importar esses itens para Exchange de várias maneiras diferentes. Importar itens para Exchange é simples quando as relações de caixa de correio não são mantidas nesses itens. Você pode usar o método Da API Gerenciada [Item.Save](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS ou a operação [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS para criar os itens em uma caixa de correio Exchange. No entanto, a abordagem simples não dá suporte a todos os cenários; por exemplo: 
  
- Não é possível manter a relação entre organizadores e participantes ao importar compromissos com participantes (reuniões). Isso significa que o organizador da reunião precisará reenviar convites de reunião aos participantes para restabelecer a relação entre o organizador e os participantes. Se o compromisso foi importado para o calendário de um participante, o compromisso não estará relacionado ao compromisso do organizador da reunião. Os participantes precisarão aceitar o convite de reunião do organizador para restabelecer a relação organizador-participante.
    
- As informações sobre os atribuídos não são preservadas quando as tarefas atribuídas são importadas.
    
Todas as opções de importação podem ser usadas para importar itens em lote para Exchange.
  
## <a name="use-ews-managed-api-or-ews-item-types-to-import-an-item"></a>Usar tipos de item EWS Managed API ou EWS para importar um item
<a name="bk_importproperties"> </a>

Você pode usar a API Gerenciada do EWS ou o EWS para importar emails, contatos, compromissos ou tarefas de outros sistemas. Basta definir as [propriedades ](properties-and-extended-properties-in-ews-in-exchange.md) do formato de origem em qualquer um dos objetos a seguir, dependendo do que você está importando. 
  
**Tabela 1. Objetos EWS Managed API e elementos EWS**

|**Objeto api gerenciada do EWS**|**Elemento EWS**|
|:-----|:-----|
|[EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[Mensagem](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[Contato](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[Contato](https://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[Compromisso](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[Tarefa](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[Tarefa](https://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
Use o método Api Gerenciada [Item.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS ou [a operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS para executar a importação de itens. Recomendamos essa abordagem quando você está importando itens de outros sistemas porque você tem controle sobre quais propriedades são importadas. Para obter mais informações sobre como definir propriedades em itens e salvar o item, consulte Create an item by using the [EWS Managed API](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) or [Create an item by using EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).
  
## <a name="import-items-with-full-fidelity"></a>Importar itens com fidelidade total
<a name="bk_importproperties"> </a>

Você pode usar a [operação UploadItems](https://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) EWS para carregar um item como um fluxo de dados. Essa representação de fluxo de dados de um item deve vir dos resultados de uma chamada de operação [ExportItems.](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) Como a API Gerenciada do EWS não implementa a operação **UploadItems,** se você usar a API Gerenciada do EWS, precisará escrever uma rotina para enviar as solicitações da Web. 
  
Essa é a maneira mais fácil de importar itens que foram exportados de outro Exchange servidor.
  
No exemplo a seguir, os identificadores e o conteúdo do elemento **Data** são reduzidos para a capacidade de leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1"/>
  </soap:Header>
  <soap:Body>
    <m:UploadItems>
      <m:Items>
        <t:Item CreateAction="CreateNew">
          <t:ParentFolderId  Id="AAMkADEzOTE7kV0AAA=" ChangeKey="AQAAAA=="/>
          <t:Data>AQAAAAgAAAAAAQAAAAADABZADQASDkANABMO</t:Data>
        </t:Item>
      </m:Items>
    </m:UploadItems>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **UploadItems** com um [elemento UploadItemsResponse](https://msdn.microsoft.com/library/93044d39-4489-456a-8cce-b6d69873348f%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **de NoError**, que indica que o item foi carregado com êxito. A resposta também inclui a ID do item carregado. 
  
## <a name="use-the-mime-stream-to-import-from-common-file-formats"></a>Usar o fluxo MIME para importar de formatos de arquivo comuns
<a name="bk_importproperties"> </a>

O EWS pode importar arquivos EML (.eml) e iCal (.ics). Você vai querer testar seu conteúdo MIME para ver como o analisador MIME Exchange mime lida com o conteúdo do fluxo MIME. Embora o uso do fluxo MIME seja conveniente, normalmente é melhor usar tipos de [item EWS Managed API ou EWS](#bk_importproperties)para importar um item. Veja um exemplo de como importar [um vCard](https://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).
  
### <a name="use-the-ews-managed-api-to-import-an-email-from-an-eml-file-by-using-the-mime-stream"></a>Use a API Gerenciada do EWS para importar um email de um arquivo EML usando o fluxo MIME

O exemplo a seguir mostra como definir a [propriedade MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) com o conteúdo de um arquivo EML e importar o email para uma caixa de correio. Este exemplo também mostra como definir a propriedade estendida [PidTagMessageFlags (0x0E07)](https://msdn.microsoft.com/library/office/cc839733%28v=office.15%29.aspx) em um email importado para que ele não apareça na caixa de correio como um item de rascunho. Este exemplo pressupõe que **o serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário pode autenticar em um Exchange servidor. 
  
```cs
private static void UploadMIMEEmail(ExchangeService service)
{
    EmailMessage email = new EmailMessage(service);
    
    string emlFileName = @"C:\import\email.eml";
    using (FileStream fs = new FileStream(emlFileName, FileMode.Open, FileAccess.Read))
    {
        byte[] bytes = new byte[fs.Length];
        int numBytesToRead = (int)fs.Length;
        int numBytesRead = 0;
        while (numBytesToRead > 0)
        {
            int n = fs.Read(bytes, numBytesRead, numBytesToRead);
            if (n == 0)
                break;
            numBytesRead += n;
            numBytesToRead -= n;
        }
        // Set the contents of the .eml file to the MimeContent property.
        email.MimeContent = new MimeContent("UTF-8", bytes);
    }
    
    // Indicate that this email is not a draft. Otherwise, the email will appear as a 
    // draft to clients.
    ExtendedPropertyDefinition PR_MESSAGE_FLAGS_msgflag_read = new ExtendedPropertyDefinition(3591, MapiPropertyType.Integer);
    email.SetExtendedProperty(PR_MESSAGE_FLAGS_msgflag_read, 1);
    // This results in a CreateItem call to EWS. The email will be saved in the Inbox folder.
    email.Save(WellKnownFolderName.Inbox);
}
```

### <a name="use-the-ews-managed-api-to-import-an-appointment-from-an-ical-file-by-using-the-mime-stream"></a>Use a API Gerenciada do EWS para importar um compromisso de um arquivo iCal usando o fluxo MIME

Você pode importar compromissos simples na forma de arquivos iCalendar usando o fluxo MIME. Não é possível importar reuniões, que são compromissos com participantes, porque a relação entre organizadores de reuniões e participantes deve ser definida como parte do fluxo de trabalho de calendário Exchange [de](calendars-and-ews-in-exchange.md) calendário. Os participantes não podem ser capturados no fluxo MIME. 
  
O exemplo de código a seguir mostra como importar um arquivo .ics simples para a caixa de correio de um usuário.
  
```cs
private static void UploadMIMEAppointment(ExchangeService service)
{
    Appointment appointment = new Appointment(service);
    string iCalFileName = @"C:\import\appointment.ics";
    using (FileStream fs = new FileStream(iCalFileName, FileMode.Open, FileAccess.Read))
    {
        byte[] bytes = new byte[fs.Length];
        int numBytesToRead = (int)fs.Length;
        int numBytesRead = 0;
        while (numBytesToRead > 0)
        {
            int n = fs.Read(bytes, numBytesRead, numBytesToRead);
            if (n == 0)
                break;
            numBytesRead += n;
            numBytesToRead -= n;
        }
        // Set the contents of the .ics file to the MimeContent property.
        appointment.MimeContent = new MimeContent("UTF-8", bytes);
    }
    // This results in a CreateItem call to EWS. 
    appointment.Save(WellKnownFolderName.Calendar);
}
```

### <a name="use-ews-to-import-an-item-by-using-the-mime-stream"></a>Use o EWS para importar um item usando o fluxo MIME

Você pode usar a [operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS para importar itens EML e iCal usando seu fluxo MIME. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
    <t:MailboxCulture>en-US</t:MailboxCulture>
  </soap:Header>
  <soap:Body >
    <m:CreateItem>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </m:SavedItemFolderId> 
        <m:Items>
        <t:Message>
          <t:MimeContent CharacterSet="UTF-8">
            <!-- Insert MIME content here-->
          </t:MimeContent>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="next-steps"></a>Próximas etapas
<a name="bk_importproperties"> </a>

Depois de importar itens para uma caixa de correio, talvez você queira criar uma pasta personalizada para armazenar seus itens importados [ou](how-to-work-with-folders-by-using-ews-in-exchange.md)sincronizar seus itens de cliente e caixa [de correio.](mailbox-synchronization-and-ews-in-exchange.md)
  
## <a name="see-also"></a>Confira também


- [Exportando e importando itens usando o EWS em Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [Exportar itens usando o EWS em Exchange](how-to-export-items-by-using-ews-in-exchange.md)
    
- [Pastas e itens no EWS em Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Sincronização de caixa de correio e EWS no Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

