---
title: Importar itens usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: dd3d3221-c98e-4fa0-81f0-77f733d2f432
description: Saiba como importar compromissos, emails, contatos, tarefas e outros itens usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: bc874c667c31beb4e59a305626247488cb1a1781
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527982"
---
# <a name="import-items-by-using-ews-in-exchange"></a><span data-ttu-id="7a9b2-103">Importar itens usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7a9b2-103">Import items by using EWS in Exchange</span></span>

<span data-ttu-id="7a9b2-104">Saiba como importar compromissos, emails, contatos, tarefas e outros itens usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-104">Learn how to import appointments, emails, contacts, tasks, and other items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="7a9b2-105">Muitos sistemas contêm compromissos, emails, contatos e tarefas, e você pode importar esses itens para o Exchange de diversas maneiras.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-105">Many systems contain appointments, emails, contacts, and tasks, and you can import those items into Exchange in a number of different ways.</span></span> <span data-ttu-id="7a9b2-106">A importação de itens para o Exchange é simples quando as relações de caixa de correio não são mantidas nesses itens.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-106">Importing items into Exchange is simple when mailbox relationships aren't maintained on those items.</span></span> <span data-ttu-id="7a9b2-107">Você pode usar o método [Item. Save](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API ou a operação [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS para criar os itens em uma caixa de correio do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-107">You can use the [Item.Save](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to create the items in an Exchange mailbox.</span></span> <span data-ttu-id="7a9b2-108">No entanto, a abordagem simples não dá suporte a todos os cenários; por exemplo:</span><span class="sxs-lookup"><span data-stu-id="7a9b2-108">The simple approach does not support all scenarios, however; for example:</span></span> 
  
- <span data-ttu-id="7a9b2-109">Você não pode manter a relação entre os organizadores e participantes ao importar compromissos com participantes (reuniões).</span><span class="sxs-lookup"><span data-stu-id="7a9b2-109">You cannot maintain the relationship between organizers and attendees when importing appointments with attendees (meetings).</span></span> <span data-ttu-id="7a9b2-110">Isso significa que o organizador da reunião precisará reenviar convites de reunião para os participantes a fim de restabelecer a relação entre o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-110">This means that the meeting organizer will need to resend meeting invites to attendees in order to reestablish the relationship between the organizer and attendees.</span></span> <span data-ttu-id="7a9b2-111">Se o compromisso foi importado para o calendário de um participante, o compromisso não será relacionado ao compromisso do organizador da reunião.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-111">If the appointment was imported into an attendee's calendar, the appointment will not be related to the meeting organizer's appointment.</span></span> <span data-ttu-id="7a9b2-112">Os participantes precisarão aceitar o convite de reunião enviado do organizador para restabelecer a relação do organizador-participante.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-112">The attendees will need to accept the resent meeting invite from the organizer in order to reestablish the organizer-attendee relationship.</span></span>
    
- <span data-ttu-id="7a9b2-113">As informações sobre os destinatários não são preservadas quando as tarefas atribuídas são importadas.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-113">Information about the assignees is not preserved when assigned tasks are imported.</span></span>
    
<span data-ttu-id="7a9b2-114">Todas as opções de importação podem ser usadas para importar itens em lotes para o Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-114">All the import options can be used to batch import items into Exchange.</span></span>
  
## <a name="use-ews-managed-api-or-ews-item-types-to-import-an-item"></a><span data-ttu-id="7a9b2-115">Usar a API gerenciada do EWS ou os tipos de item do EWS para importar um item</span><span class="sxs-lookup"><span data-stu-id="7a9b2-115">Use EWS Managed API or EWS item types to import an item</span></span>
<span data-ttu-id="7a9b2-116"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="7a9b2-116"><a name="bk_importproperties"> </a></span></span>

<span data-ttu-id="7a9b2-117">Você pode usar a API gerenciada do EWS ou o EWS para importar emails, contatos, compromissos ou tarefas de outros sistemas.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-117">You can use the EWS Managed API or EWS to import emails, contacts, appointments, or tasks from other systems.</span></span> <span data-ttu-id="7a9b2-118">Basta definir as [Propriedades](properties-and-extended-properties-in-ews-in-exchange.md) do seu formato de origem em qualquer um dos seguintes objetos, dependendo do que você está importando.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-118">Just set the [properties ](properties-and-extended-properties-in-ews-in-exchange.md) from your source format on any of the following objects, depending on what you're importing.</span></span> 
  
<span data-ttu-id="7a9b2-119">**Tabela 1. Objetos da API gerenciada do EWS e elementos do EWS**</span><span class="sxs-lookup"><span data-stu-id="7a9b2-119">**Table 1. EWS Managed API objects and EWS elements**</span></span>

|<span data-ttu-id="7a9b2-120">**Objeto API gerenciada do EWS**</span><span class="sxs-lookup"><span data-stu-id="7a9b2-120">**EWS Managed API object**</span></span>|<span data-ttu-id="7a9b2-121">**Elemento do EWS**</span><span class="sxs-lookup"><span data-stu-id="7a9b2-121">**EWS element**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a9b2-122">EmailMessage</span><span class="sxs-lookup"><span data-stu-id="7a9b2-122">EmailMessage</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="7a9b2-123">Mensagem</span><span class="sxs-lookup"><span data-stu-id="7a9b2-123">Message</span></span>](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="7a9b2-124">Contato</span><span class="sxs-lookup"><span data-stu-id="7a9b2-124">Contact</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="7a9b2-125">Contato</span><span class="sxs-lookup"><span data-stu-id="7a9b2-125">Contact</span></span>](https://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="7a9b2-126">Compromisso</span><span class="sxs-lookup"><span data-stu-id="7a9b2-126">Appointment</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="7a9b2-127">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="7a9b2-127">CalendarItem</span></span>](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="7a9b2-128">Tarefa</span><span class="sxs-lookup"><span data-stu-id="7a9b2-128">Task</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="7a9b2-129">Tarefa</span><span class="sxs-lookup"><span data-stu-id="7a9b2-129">Task</span></span>](https://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="7a9b2-130">Use o método [Item. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API ou a operação [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS para executar a importação de itens.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-130">Use the [Item.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to perform the import of items.</span></span> <span data-ttu-id="7a9b2-131">Recomendamos essa abordagem quando você estiver importando itens de outros sistemas porque você tem controle sobre quais propriedades são importadas.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-131">We recommend this approach when you're importing items from other systems because you have control over which properties get imported.</span></span> <span data-ttu-id="7a9b2-132">Para obter mais informações sobre como definir propriedades em itens e salvar o item, consulte [criar um item usando a API gerenciada do EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) ou [criar um item usando o EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).</span><span class="sxs-lookup"><span data-stu-id="7a9b2-132">For more information about how to set properties on items and then save the item, see [Create an item by using the EWS Managed API](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) or [Create an item by using EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).</span></span>
  
## <a name="import-items-with-full-fidelity"></a><span data-ttu-id="7a9b2-133">Importar itens com fidelidade total</span><span class="sxs-lookup"><span data-stu-id="7a9b2-133">Import items with full fidelity</span></span>
<span data-ttu-id="7a9b2-134"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="7a9b2-134"><a name="bk_importproperties"> </a></span></span>

<span data-ttu-id="7a9b2-135">Você pode usar a operação [UploadItems](https://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) EWS para carregar um item como um fluxo de dados.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-135">You can use the [UploadItems](https://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) EWS operation to upload an item as a data stream.</span></span> <span data-ttu-id="7a9b2-136">Esta representação de fluxo de dados de um item deve ser proveniente dos resultados de uma chamada de operação [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="7a9b2-136">This data stream representation of an item has to come from the results of an [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) operation call.</span></span> <span data-ttu-id="7a9b2-137">Como a API gerenciada do EWS não implementa a operação **UploadItems** , se você usar a API gerenciada do EWS, você precisará escrever uma rotina para enviar as solicitações da Web.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-137">Because the EWS Managed API does not implement the **UploadItems** operation, if you use the EWS Managed API, you'll need to write a routine to send the web requests.</span></span> 
  
<span data-ttu-id="7a9b2-138">Essa é a maneira mais fácil de importar itens que foram exportados de outro servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-138">This is the easiest way to import items that have been exported from another Exchange server.</span></span>
  
<span data-ttu-id="7a9b2-139">No exemplo a seguir, os identificadores e o conteúdo do elemento de **dados** são reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-139">In the following example, the identifiers and the **Data** element content are shortened for readability.</span></span> 
  
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

O servidor responde à solicitação **UploadItems** com um elemento [UploadItemsResponse](https://msdn.microsoft.com/library/93044d39-4489-456a-8cce-b6d69873348f%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que o item foi carregado com êxito. <span data-ttu-id="7a9b2-141">A resposta também inclui a ID do item carregado.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-141">The response also includes the item ID of the uploaded item.</span></span> 
  
## <a name="use-the-mime-stream-to-import-from-common-file-formats"></a><span data-ttu-id="7a9b2-142">Usar o fluxo MIME para importar de formatos de arquivo comuns</span><span class="sxs-lookup"><span data-stu-id="7a9b2-142">Use the MIME stream to import from common file formats</span></span>
<span data-ttu-id="7a9b2-143"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="7a9b2-143"><a name="bk_importproperties"> </a></span></span>

<span data-ttu-id="7a9b2-144">O EWS pode importar arquivos EML (. eml) e iCal (. ICS).</span><span class="sxs-lookup"><span data-stu-id="7a9b2-144">EWS can import EML (.eml) and iCal (.ics) files.</span></span> <span data-ttu-id="7a9b2-145">Convém testar o conteúdo MIME para ver como o analisador MIME do Exchange manipula o conteúdo do seu fluxo MIME.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-145">You'll want to test your MIME content to see how the Exchange MIME parser handles the content of your MIME stream.</span></span> <span data-ttu-id="7a9b2-146">Embora o uso do fluxo MIME seja conveniente, geralmente é melhor [usar a API gerenciada do EWS ou tipos de item do EWS para importar um item](#bk_importproperties).</span><span class="sxs-lookup"><span data-stu-id="7a9b2-146">Although using the MIME stream is convenient, it is typically better to [Use EWS Managed API or EWS item types to import an item](#bk_importproperties).</span></span> <span data-ttu-id="7a9b2-147">Veja um exemplo de como [importar um vCard](https://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).</span><span class="sxs-lookup"><span data-stu-id="7a9b2-147">Here's an example of how to [import a vCard](https://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).</span></span>
  
### <a name="use-the-ews-managed-api-to-import-an-email-from-an-eml-file-by-using-the-mime-stream"></a><span data-ttu-id="7a9b2-148">Usar a API gerenciada do EWS para importar um email de um arquivo EML usando o fluxo MIME</span><span class="sxs-lookup"><span data-stu-id="7a9b2-148">Use the EWS Managed API to import an email from an EML file by using the MIME stream</span></span>

<span data-ttu-id="7a9b2-149">O exemplo a seguir mostra como definir a propriedade [MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) com o conteúdo de um arquivo EML e, em seguida, importar o email para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-149">The following example shows how to set the [MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) property with the contents of an EML file and then import the email into a mailbox.</span></span> <span data-ttu-id="7a9b2-150">Este exemplo também mostra como definir a propriedade estendida [PidTagMessageFlags (0x0E07)](https://msdn.microsoft.com/library/office/cc839733%28v=office.15%29.aspx) em um email importado para que ele não apareça na caixa de correio como um item de rascunho.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-150">This example also shows how to set the [PidTagMessageFlags (0x0E07)](https://msdn.microsoft.com/library/office/cc839733%28v=office.15%29.aspx) extended property on an imported email so that it doesn't appear in the mailbox as a draft item.</span></span> <span data-ttu-id="7a9b2-151">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário pode autenticar em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-151">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
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

### <a name="use-the-ews-managed-api-to-import-an-appointment-from-an-ical-file-by-using-the-mime-stream"></a><span data-ttu-id="7a9b2-152">Usar a API gerenciada do EWS para importar um compromisso de um arquivo iCal usando o fluxo MIME</span><span class="sxs-lookup"><span data-stu-id="7a9b2-152">Use the EWS Managed API to import an appointment from an iCal file by using the MIME stream</span></span>

<span data-ttu-id="7a9b2-153">Você pode importar compromissos simples no formato de arquivos iCalendar usando o fluxo MIME.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-153">You can import simple appointments in the form of iCalendar files by using the MIME stream.</span></span> <span data-ttu-id="7a9b2-154">Você não pode importar reuniões, que são compromissos com participantes, porque a relação entre organizadores e participantes da reunião deve ser definida como parte do fluxo de trabalho de [calendário do Exchange](calendars-and-ews-in-exchange.md) .</span><span class="sxs-lookup"><span data-stu-id="7a9b2-154">You can't import meetings, which are appointments with attendees, because the relationship between meeting organizers and attendees has to be set as part of the [Exchange calendaring](calendars-and-ews-in-exchange.md) workflow.</span></span> <span data-ttu-id="7a9b2-155">Os participantes não podem ser capturados no fluxo MIME.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-155">Attendees cannot be captured in the MIME stream.</span></span> 
  
<span data-ttu-id="7a9b2-156">O exemplo de código a seguir mostra como importar um arquivo. ics simples para a caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-156">The following code example shows you how to import a simple .ics file into a user's mailbox.</span></span>
  
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

### <a name="use-ews-to-import-an-item-by-using-the-mime-stream"></a><span data-ttu-id="7a9b2-157">Usar o EWS para importar um item usando o fluxo MIME</span><span class="sxs-lookup"><span data-stu-id="7a9b2-157">Use EWS to import an item by using the MIME stream</span></span>

<span data-ttu-id="7a9b2-158">Você pode usar a operação [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS para importar itens eml e iCal usando seu fluxo MIME.</span><span class="sxs-lookup"><span data-stu-id="7a9b2-158">You can use the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to import EML and iCal items by using their MIME stream.</span></span> 
  
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

## <a name="next-steps"></a><span data-ttu-id="7a9b2-159">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="7a9b2-159">Next steps</span></span>
<span data-ttu-id="7a9b2-160"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="7a9b2-160"><a name="bk_importproperties"> </a></span></span>

<span data-ttu-id="7a9b2-161">Depois de importar itens para uma caixa de correio, convém [criar uma pasta personalizada para armazenar os itens importados](how-to-work-with-folders-by-using-ews-in-exchange.md)ou [sincronizar seus itens de cliente e de caixa de correio](mailbox-synchronization-and-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="7a9b2-161">After you import items into a mailbox, you might want to [create a custom folder to store your imported items](how-to-work-with-folders-by-using-ews-in-exchange.md), or [synchronize your client and mailbox items](mailbox-synchronization-and-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="7a9b2-162">Confira também</span><span class="sxs-lookup"><span data-stu-id="7a9b2-162">See also</span></span>


- [<span data-ttu-id="7a9b2-163">Exportando e importando itens usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7a9b2-163">Exporting and importing items by using EWS in Exchange</span></span>](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="7a9b2-164">Exportar itens usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7a9b2-164">Export items by using EWS in Exchange</span></span>](how-to-export-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="7a9b2-165">Pastas e itens no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7a9b2-165">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="7a9b2-166">Sincronização de caixa de correio e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7a9b2-166">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

