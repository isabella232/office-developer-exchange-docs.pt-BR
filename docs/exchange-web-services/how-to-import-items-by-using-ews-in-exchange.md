---
title: Importar itens usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: dd3d3221-c98e-4fa0-81f0-77f733d2f432
description: Saiba como importar os compromissos, emails, contatos, tarefas e outros itens usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: c09c96eff455b7584b084e71b937853abfde731d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750778"
---
# <a name="import-items-by-using-ews-in-exchange"></a>Importar itens usando o EWS no Exchange

Saiba como importar os compromissos, emails, contatos, tarefas e outros itens usando a API gerenciada de EWS ou EWS no Exchange.
  
Muitos sistemas contêm emails, compromissos, contatos e tarefas, e você pode importar os itens para o Exchange em um número de formas diferentes. Importando itens para o Exchange é simple quando relacionamentos de caixa de correio não são mantidos nesses itens. Você pode usar o método de API gerenciada de EWS [Item.Save](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) ou a operação de EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) para criar os itens em uma caixa de correio do Exchange. A abordagem simple não oferece suporte a todos os cenários, no entanto; Por exemplo: 
  
- Você não pode manter a relação entre os organizadores e participantes ao importar compromissos com participantes (reuniões). Isso significa que o organizador da reunião precisará reenviar convites de reunião a participantes para restabelecer o relacionamento entre o organizador e participantes. Se o compromisso foi importado no calendário do participante, o compromisso não será relacionado ao compromisso do organizador da reunião. Os participantes precisarão aceitar o convite de reunião resent do organizador para restabelecer o relacionamento de participante do organizador.
    
- Informações sobre os destinatários não são preservadas quando tarefas atribuídas são importadas.
    
Todas as opções de importação podem ser usadas para importar itens de lote para o Exchange.
  
## <a name="use-ews-managed-api-or-ews-item-types-to-import-an-item"></a>API gerenciada de EWS uso ou EWS de tipos para importar um item de item
<a name="bk_importproperties"> </a>

Você pode usar a API gerenciada de EWS ou o EWS para importar emails, contatos, compromissos ou tarefas de outros sistemas. Basta defina as [Propriedades](properties-and-extended-properties-in-ews-in-exchange.md) de seu formato de fonte em qualquer um dos objetos a seguir, dependendo se você está importando. 
  
**Tabela 1. Objetos de API gerenciada de EWS e elementos EWS**

|**Objeto da API gerenciada de EWS**|**Elemento EWS**|
|:-----|:-----|
|[EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[Mensagem](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[Contato](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[Contato](http://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[Compromisso](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[Task](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[Task](http://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
Use o método de API gerenciada de EWS [Item.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) ou a operação de EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) para executar a importação de itens. Recomendamos essa abordagem ao importar itens de outros sistemas porque você terá controle sobre quais propriedades serão importadas. Para obter mais informações sobre como definir propriedades em itens e salva o item, consulte [criar um item usando a API gerenciada de EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) ou [criar um item usando o EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).
  
## <a name="import-items-with-full-fidelity"></a>Importar itens com fidelidade total
<a name="bk_importproperties"> </a>

Você pode usar a operação de EWS [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) para carregar um item como um fluxo de dados. Esta representação de fluxo de dados de um item deve ser obtido dos resultados de uma chamada de operação [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) . Porque a API gerenciada de EWS não implementa a operação **UploadItems** , se você usar a API gerenciada de EWS, você precisará gravar uma rotina para enviar as solicitações da web. 
  
Esta é a maneira mais fácil para importar itens que tenham sido exportados de outro servidor Exchange.
  
No exemplo a seguir, os identificadores e o conteúdo do elemento de **dados** são reduzidos para melhorar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

O servidor responde à solicitação **UploadItems** com um elemento [UploadItemsResponse](http://msdn.microsoft.com/library/93044d39-4489-456a-8cce-b6d69873348f%28Office.15%29.aspx) que que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que o item foi carregado com êxito. A resposta também inclui a ID de item do item carregado. 
  
## <a name="use-the-mime-stream-to-import-from-common-file-formats"></a>Usar o fluxo MIME para importar de formatos de arquivo comuns
<a name="bk_importproperties"> </a>

EWS pode importar EML (. eml) e arquivos de iCal (. ICS). Você vai querer testar seu conteúdo MIME para ver como o analisador de MIME do Exchange manipula o conteúdo de seu fluxo de MIME. Embora seja conveniente usar o fluxo MIME, é geralmente melhor [uso EWS Managed API ou EWS de tipos para importar um item de item](#bk_importproperties). Aqui está um exemplo de como importar [um vCard](http://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).
  
### <a name="use-the-ews-managed-api-to-import-an-email-from-an-eml-file-by-using-the-mime-stream"></a>Use a API gerenciada de EWS para importar um email de um arquivo EML usando-se o fluxo MIME

O exemplo a seguir mostra como definir a propriedade [MimeContent](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) com o conteúdo de um arquivo EML e importe o email em uma caixa de correio. Este exemplo também mostra como definir o [PidTagMessageFlags (0x0E07)](http://msdn.microsoft.com/en-us/library/office/cc839733%28v=office.15%29.aspx) estendido de propriedade em um email importado para que ele não aparece na caixa de correio como um item de rascunho. Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário pode autenticar em um servidor Exchange. 
  
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

### <a name="use-the-ews-managed-api-to-import-an-appointment-from-an-ical-file-by-using-the-mime-stream"></a>Use a API gerenciada de EWS para importar um compromisso de um arquivo iCal usando o fluxo MIME

Você pode importar os compromissos simples no formato iCalendar arquivos usando o fluxo MIME. Não é possível importar reuniões, que são os compromissos com participantes, porque a relação entre os organizadores de reuniões e participantes tem que ser definida como parte do fluxo de trabalho de [calendário do Exchange](calendars-and-ews-in-exchange.md) . Os participantes não podem ser capturados no fluxo de MIME. 
  
O exemplo de código a seguir mostra como importar um arquivo. ICS simples para caixa de correio do usuário.
  
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

Você pode usar a operação de EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) para importar itens de iCal e EML usando seu fluxo de MIME. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

Depois de importar itens em uma caixa de correio, talvez você queira [criar uma pasta personalizada para armazenar seus itens importados](how-to-work-with-folders-by-using-ews-in-exchange.md)ou [sincronizar os itens do seu cliente e caixa de correio](mailbox-synchronization-and-ews-in-exchange.md).
  
## <a name="see-also"></a>Confira também


- [Exportando e importando itens usando o EWS no Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [Exportar itens usando o EWS no Exchange](how-to-export-items-by-using-ews-in-exchange.md)
    
- [Pastas e itens no EWS no Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Sincronização de caixa de correio e EWS no Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

