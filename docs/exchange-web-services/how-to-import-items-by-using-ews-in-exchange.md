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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750778"
---
# <a name="import-items-by-using-ews-in-exchange"></a><span data-ttu-id="de779-103">Importar itens usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="de779-103">Import items by using EWS in Exchange</span></span>

<span data-ttu-id="de779-104">Saiba como importar os compromissos, emails, contatos, tarefas e outros itens usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="de779-104">Learn how to import appointments, emails, contacts, tasks, and other items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="de779-105">Muitos sistemas contêm emails, compromissos, contatos e tarefas, e você pode importar os itens para o Exchange em um número de formas diferentes.</span><span class="sxs-lookup"><span data-stu-id="de779-105">Many systems contain appointments, emails, contacts, and tasks, and you can import those items into Exchange in a number of different ways.</span></span> <span data-ttu-id="de779-106">Importando itens para o Exchange é simple quando relacionamentos de caixa de correio não são mantidos nesses itens.</span><span class="sxs-lookup"><span data-stu-id="de779-106">Importing items into Exchange is simple when mailbox relationships aren't maintained on those items.</span></span> <span data-ttu-id="de779-107">Você pode usar o método de API gerenciada de EWS [Item.Save](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) ou a operação de EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) para criar os itens em uma caixa de correio do Exchange.</span><span class="sxs-lookup"><span data-stu-id="de779-107">You can use the [Item.Save](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to create the items in an Exchange mailbox.</span></span> <span data-ttu-id="de779-108">A abordagem simple não oferece suporte a todos os cenários, no entanto; Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="de779-108">The simple approach does not support all scenarios, however; for example:</span></span> 
  
- <span data-ttu-id="de779-109">Você não pode manter a relação entre os organizadores e participantes ao importar compromissos com participantes (reuniões).</span><span class="sxs-lookup"><span data-stu-id="de779-109">You cannot maintain the relationship between organizers and attendees when importing appointments with attendees (meetings).</span></span> <span data-ttu-id="de779-110">Isso significa que o organizador da reunião precisará reenviar convites de reunião a participantes para restabelecer o relacionamento entre o organizador e participantes.</span><span class="sxs-lookup"><span data-stu-id="de779-110">This means that the meeting organizer will need to resend meeting invites to attendees in order to reestablish the relationship between the organizer and attendees.</span></span> <span data-ttu-id="de779-111">Se o compromisso foi importado no calendário do participante, o compromisso não será relacionado ao compromisso do organizador da reunião.</span><span class="sxs-lookup"><span data-stu-id="de779-111">If the appointment was imported into an attendee's calendar, the appointment will not be related to the meeting organizer's appointment.</span></span> <span data-ttu-id="de779-112">Os participantes precisarão aceitar o convite de reunião resent do organizador para restabelecer o relacionamento de participante do organizador.</span><span class="sxs-lookup"><span data-stu-id="de779-112">The attendees will need to accept the resent meeting invite from the organizer in order to reestablish the organizer-attendee relationship.</span></span>
    
- <span data-ttu-id="de779-113">Informações sobre os destinatários não são preservadas quando tarefas atribuídas são importadas.</span><span class="sxs-lookup"><span data-stu-id="de779-113">Information about the assignees is not preserved when assigned tasks are imported.</span></span>
    
<span data-ttu-id="de779-114">Todas as opções de importação podem ser usadas para importar itens de lote para o Exchange.</span><span class="sxs-lookup"><span data-stu-id="de779-114">All the import options can be used to batch import items into Exchange.</span></span>
  
## <a name="use-ews-managed-api-or-ews-item-types-to-import-an-item"></a><span data-ttu-id="de779-115">API gerenciada de EWS uso ou EWS de tipos para importar um item de item</span><span class="sxs-lookup"><span data-stu-id="de779-115">Use EWS Managed API or EWS item types to import an item</span></span>
<span data-ttu-id="de779-116"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="de779-116"></span></span>

<span data-ttu-id="de779-117">Você pode usar a API gerenciada de EWS ou o EWS para importar emails, contatos, compromissos ou tarefas de outros sistemas.</span><span class="sxs-lookup"><span data-stu-id="de779-117">You can use the EWS Managed API or EWS to import emails, contacts, appointments, or tasks from other systems.</span></span> <span data-ttu-id="de779-118">Basta defina as [Propriedades](properties-and-extended-properties-in-ews-in-exchange.md) de seu formato de fonte em qualquer um dos objetos a seguir, dependendo se você está importando.</span><span class="sxs-lookup"><span data-stu-id="de779-118">Just set the [properties ](properties-and-extended-properties-in-ews-in-exchange.md) from your source format on any of the following objects, depending on what you're importing.</span></span> 
  
<span data-ttu-id="de779-119">**Tabela 1. Objetos de API gerenciada de EWS e elementos EWS**</span><span class="sxs-lookup"><span data-stu-id="de779-119">**Table 1. EWS Managed API objects and EWS elements**</span></span>

|<span data-ttu-id="de779-120">**Objeto da API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="de779-120">**EWS Managed API object**</span></span>|<span data-ttu-id="de779-121">**Elemento EWS**</span><span class="sxs-lookup"><span data-stu-id="de779-121">**EWS element**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de779-122">EmailMessage</span><span class="sxs-lookup"><span data-stu-id="de779-122">EmailMessage</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="de779-123">Mensagem</span><span class="sxs-lookup"><span data-stu-id="de779-123">Message</span></span>](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="de779-124">Contato</span><span class="sxs-lookup"><span data-stu-id="de779-124">Contact</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="de779-125">Contato</span><span class="sxs-lookup"><span data-stu-id="de779-125">Contact</span></span>](http://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="de779-126">Compromisso</span><span class="sxs-lookup"><span data-stu-id="de779-126">Appointment</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="de779-127">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="de779-127">CalendarItem</span></span>](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="de779-128">Task</span><span class="sxs-lookup"><span data-stu-id="de779-128">Task</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="de779-129">Task</span><span class="sxs-lookup"><span data-stu-id="de779-129">Task</span></span>](http://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="de779-130">Use o método de API gerenciada de EWS [Item.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) ou a operação de EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) para executar a importação de itens.</span><span class="sxs-lookup"><span data-stu-id="de779-130">Use the [Item.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to perform the import of items.</span></span> <span data-ttu-id="de779-131">Recomendamos essa abordagem ao importar itens de outros sistemas porque você terá controle sobre quais propriedades serão importadas.</span><span class="sxs-lookup"><span data-stu-id="de779-131">We recommend this approach when you're importing items from other systems because you have control over which properties get imported.</span></span> <span data-ttu-id="de779-132">Para obter mais informações sobre como definir propriedades em itens e salva o item, consulte [criar um item usando a API gerenciada de EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) ou [criar um item usando o EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).</span><span class="sxs-lookup"><span data-stu-id="de779-132">For more information about how to set properties on items and then save the item, see [Create an item by using the EWS Managed API](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) or [Create an item by using EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).</span></span>
  
## <a name="import-items-with-full-fidelity"></a><span data-ttu-id="de779-133">Importar itens com fidelidade total</span><span class="sxs-lookup"><span data-stu-id="de779-133">Import items with full fidelity</span></span>
<span data-ttu-id="de779-134"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="de779-134"></span></span>

<span data-ttu-id="de779-135">Você pode usar a operação de EWS [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) para carregar um item como um fluxo de dados.</span><span class="sxs-lookup"><span data-stu-id="de779-135">You can use the [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) EWS operation to upload an item as a data stream.</span></span> <span data-ttu-id="de779-136">Esta representação de fluxo de dados de um item deve ser obtido dos resultados de uma chamada de operação [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="de779-136">This data stream representation of an item has to come from the results of an [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) operation call.</span></span> <span data-ttu-id="de779-137">Porque a API gerenciada de EWS não implementa a operação **UploadItems** , se você usar a API gerenciada de EWS, você precisará gravar uma rotina para enviar as solicitações da web.</span><span class="sxs-lookup"><span data-stu-id="de779-137">Because the EWS Managed API does not implement the **UploadItems** operation, if you use the EWS Managed API, you'll need to write a routine to send the web requests.</span></span> 
  
<span data-ttu-id="de779-138">Esta é a maneira mais fácil para importar itens que tenham sido exportados de outro servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="de779-138">This is the easiest way to import items that have been exported from another Exchange server.</span></span>
  
<span data-ttu-id="de779-139">No exemplo a seguir, os identificadores e o conteúdo do elemento de **dados** são reduzidos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="de779-139">In the following example, the identifiers and the **Data** element content are shortened for readability.</span></span> 
  
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

O servidor responde à solicitação **UploadItems** com um elemento [UploadItemsResponse](http://msdn.microsoft.com/library/93044d39-4489-456a-8cce-b6d69873348f%28Office.15%29.aspx) que que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que o item foi carregado com êxito. <span data-ttu-id="de779-141">A resposta também inclui a ID de item do item carregado.</span><span class="sxs-lookup"><span data-stu-id="de779-141">The response also includes the item ID of the uploaded item.</span></span> 
  
## <a name="use-the-mime-stream-to-import-from-common-file-formats"></a><span data-ttu-id="de779-142">Usar o fluxo MIME para importar de formatos de arquivo comuns</span><span class="sxs-lookup"><span data-stu-id="de779-142">Use the MIME stream to import from common file formats</span></span>
<span data-ttu-id="de779-143"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="de779-143"></span></span>

<span data-ttu-id="de779-144">EWS pode importar EML (. eml) e arquivos de iCal (. ICS).</span><span class="sxs-lookup"><span data-stu-id="de779-144">EWS can import EML (.eml) and iCal (.ics) files.</span></span> <span data-ttu-id="de779-145">Você vai querer testar seu conteúdo MIME para ver como o analisador de MIME do Exchange manipula o conteúdo de seu fluxo de MIME.</span><span class="sxs-lookup"><span data-stu-id="de779-145">You'll want to test your MIME content to see how the Exchange MIME parser handles the content of your MIME stream.</span></span> <span data-ttu-id="de779-146">Embora seja conveniente usar o fluxo MIME, é geralmente melhor [uso EWS Managed API ou EWS de tipos para importar um item de item](#bk_importproperties).</span><span class="sxs-lookup"><span data-stu-id="de779-146">Although using the MIME stream is convenient, it is typically better to [Use EWS Managed API or EWS item types to import an item](#bk_importproperties).</span></span> <span data-ttu-id="de779-147">Aqui está um exemplo de como importar [um vCard](http://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).</span><span class="sxs-lookup"><span data-stu-id="de779-147">Here's an example of how to [import a vCard](http://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).</span></span>
  
### <a name="use-the-ews-managed-api-to-import-an-email-from-an-eml-file-by-using-the-mime-stream"></a><span data-ttu-id="de779-148">Use a API gerenciada de EWS para importar um email de um arquivo EML usando-se o fluxo MIME</span><span class="sxs-lookup"><span data-stu-id="de779-148">Use the EWS Managed API to import an email from an EML file by using the MIME stream</span></span>

<span data-ttu-id="de779-149">O exemplo a seguir mostra como definir a propriedade [MimeContent](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) com o conteúdo de um arquivo EML e importe o email em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="de779-149">The following example shows how to set the [MimeContent](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) property with the contents of an EML file and then import the email into a mailbox.</span></span> <span data-ttu-id="de779-150">Este exemplo também mostra como definir o [PidTagMessageFlags (0x0E07)](http://msdn.microsoft.com/en-us/library/office/cc839733%28v=office.15%29.aspx) estendido de propriedade em um email importado para que ele não aparece na caixa de correio como um item de rascunho.</span><span class="sxs-lookup"><span data-stu-id="de779-150">This example also shows how to set the [PidTagMessageFlags (0x0E07)](http://msdn.microsoft.com/en-us/library/office/cc839733%28v=office.15%29.aspx) extended property on an imported email so that it doesn't appear in the mailbox as a draft item.</span></span> <span data-ttu-id="de779-151">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário pode autenticar em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="de779-151">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
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

### <a name="use-the-ews-managed-api-to-import-an-appointment-from-an-ical-file-by-using-the-mime-stream"></a><span data-ttu-id="de779-152">Use a API gerenciada de EWS para importar um compromisso de um arquivo iCal usando o fluxo MIME</span><span class="sxs-lookup"><span data-stu-id="de779-152">Use the EWS Managed API to import an appointment from an iCal file by using the MIME stream</span></span>

<span data-ttu-id="de779-153">Você pode importar os compromissos simples no formato iCalendar arquivos usando o fluxo MIME.</span><span class="sxs-lookup"><span data-stu-id="de779-153">You can import simple appointments in the form of iCalendar files by using the MIME stream.</span></span> <span data-ttu-id="de779-154">Não é possível importar reuniões, que são os compromissos com participantes, porque a relação entre os organizadores de reuniões e participantes tem que ser definida como parte do fluxo de trabalho de [calendário do Exchange](calendars-and-ews-in-exchange.md) .</span><span class="sxs-lookup"><span data-stu-id="de779-154">You can't import meetings, which are appointments with attendees, because the relationship between meeting organizers and attendees has to be set as part of the [Exchange calendaring](calendars-and-ews-in-exchange.md) workflow.</span></span> <span data-ttu-id="de779-155">Os participantes não podem ser capturados no fluxo de MIME.</span><span class="sxs-lookup"><span data-stu-id="de779-155">Attendees cannot be captured in the MIME stream.</span></span> 
  
<span data-ttu-id="de779-156">O exemplo de código a seguir mostra como importar um arquivo. ICS simples para caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="de779-156">The following code example shows you how to import a simple .ics file into a user's mailbox.</span></span>
  
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

### <a name="use-ews-to-import-an-item-by-using-the-mime-stream"></a><span data-ttu-id="de779-157">Use o EWS para importar um item usando o fluxo MIME</span><span class="sxs-lookup"><span data-stu-id="de779-157">Use EWS to import an item by using the MIME stream</span></span>

<span data-ttu-id="de779-158">Você pode usar a operação de EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) para importar itens de iCal e EML usando seu fluxo de MIME.</span><span class="sxs-lookup"><span data-stu-id="de779-158">You can use the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to import EML and iCal items by using their MIME stream.</span></span> 
  
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

## <a name="next-steps"></a><span data-ttu-id="de779-159">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="de779-159">Next steps</span></span>
<span data-ttu-id="de779-160"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="de779-160"></span></span>

<span data-ttu-id="de779-161">Depois de importar itens em uma caixa de correio, talvez você queira [criar uma pasta personalizada para armazenar seus itens importados](how-to-work-with-folders-by-using-ews-in-exchange.md)ou [sincronizar os itens do seu cliente e caixa de correio](mailbox-synchronization-and-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="de779-161">After you import items into a mailbox, you might want to [create a custom folder to store your imported items](how-to-work-with-folders-by-using-ews-in-exchange.md), or [synchronize your client and mailbox items](mailbox-synchronization-and-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="de779-162">Confira também</span><span class="sxs-lookup"><span data-stu-id="de779-162">See also</span></span>


- [<span data-ttu-id="de779-163">Exportando e importando itens usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="de779-163">Exporting and importing items by using EWS in Exchange</span></span>](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="de779-164">Exportar itens usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="de779-164">Export items by using EWS in Exchange</span></span>](how-to-export-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="de779-165">Pastas e itens no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="de779-165">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="de779-166">Sincronização de caixa de correio e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="de779-166">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

