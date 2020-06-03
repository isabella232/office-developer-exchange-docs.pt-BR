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
# <a name="export-items-by-using-ews-in-exchange"></a><span data-ttu-id="66250-103">Exportar itens usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="66250-103">Export items by using EWS in Exchange</span></span>

<span data-ttu-id="66250-104">Saiba como exportar compromissos, emails, contatos, tarefas e outros itens usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="66250-104">Learn how to export appointments, emails, contacts, tasks, and other items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="66250-105">Você pode exportar itens do Exchange usando a API gerenciada do EWS ou o EWS de várias maneiras diferentes.</span><span class="sxs-lookup"><span data-stu-id="66250-105">You can export items from Exchange by using the EWS Managed API or EWS in a number of different ways.</span></span> <span data-ttu-id="66250-106">A opção que você usa depende:</span><span class="sxs-lookup"><span data-stu-id="66250-106">The option you use depends on:</span></span>
  
- <span data-ttu-id="66250-107">O tipo de item que é exportado.</span><span class="sxs-lookup"><span data-stu-id="66250-107">The item type that is exported.</span></span>
    
- <span data-ttu-id="66250-108">O grau de fidelidade que você deseja manter entre o estado do item no Exchange e o item exportado.</span><span class="sxs-lookup"><span data-stu-id="66250-108">The degree of fidelity that you want maintained between the item state in Exchange and the exported item.</span></span>
    
- <span data-ttu-id="66250-109">O formato do item exportado.</span><span class="sxs-lookup"><span data-stu-id="66250-109">The format of the exported item.</span></span>
    
- <span data-ttu-id="66250-110">Todos os requisitos de pós-processamento.</span><span class="sxs-lookup"><span data-stu-id="66250-110">Any post-processing requirements.</span></span>
    
- <span data-ttu-id="66250-111">Se você deseja importar o item de volta para o Exchange.</span><span class="sxs-lookup"><span data-stu-id="66250-111">Whether you want to import the item back into Exchange.</span></span>
    
<span data-ttu-id="66250-112">Este artigo mostra como usar cada uma das diferentes opções para exportar itens.</span><span class="sxs-lookup"><span data-stu-id="66250-112">This article shows you how to use each of the different options to export items.</span></span> <span data-ttu-id="66250-113">Você pode usar qualquer opção para exportar itens em lotes do Exchange.</span><span class="sxs-lookup"><span data-stu-id="66250-113">You can use any option to batch export items out of Exchange.</span></span>
  
## <a name="export-an-item-into-a-custom-format"></a><span data-ttu-id="66250-114">Exportar um item para um formato personalizado</span><span class="sxs-lookup"><span data-stu-id="66250-114">Export an item into a custom format</span></span>
<span data-ttu-id="66250-115"><a name="bk_exportcustom"> </a></span><span class="sxs-lookup"><span data-stu-id="66250-115"><a name="bk_exportcustom"> </a></span></span>

<span data-ttu-id="66250-116">Você pode usar os resultados de um [Item. vincule](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) a chamada de método de API gerenciada do EWS ou analise os resultados de uma operação do EWS do [GetItem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) em um formato que funciona com seus requisitos de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="66250-116">You can use the results of an [Item.Bind](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) EWS Managed API method call or parse the results of a [GetItem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) EWS operation into a format that works with your application requirements.</span></span> <span data-ttu-id="66250-117">Use essa opção quando você estiver exportando itens para importá-los para um banco de dados, um arquivo. csv ou outro formato ou sistema.</span><span class="sxs-lookup"><span data-stu-id="66250-117">Use this option when you are exporting items in order to import them into a database, .csv file, or another format or system.</span></span> <span data-ttu-id="66250-118">Você pode até mesmo salvar o item no formato do item EWS XML, que pode ser útil porque muitos sistemas têm capacidade de análise XML.</span><span class="sxs-lookup"><span data-stu-id="66250-118">You can even save the item in the form of the item EWS XML, which can be useful because many systems have XML parsing capability.</span></span> <span data-ttu-id="66250-119">Recomendamos que você use o método **Item. bind** ou a operação **GetItem** (sem a propriedade [Item. MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) ) porque essa opção dá controle sobre quais propriedades são exportadas.</span><span class="sxs-lookup"><span data-stu-id="66250-119">We recommend that you use the **Item.Bind** method or the **GetItem** operation (without the [Item.MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) property) because this option gives you control over which properties are exported.</span></span> 
  
## <a name="export-items-with-full-fidelity"></a><span data-ttu-id="66250-120">Exportar itens com fidelidade total</span><span class="sxs-lookup"><span data-stu-id="66250-120">Export items with full fidelity</span></span>
<span data-ttu-id="66250-121"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="66250-121"><a name="bk_exportfullfidelity"> </a></span></span>

<span data-ttu-id="66250-122">Se você quiser exportar itens com fidelidade total, poderá usar a operação [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) do EWS.</span><span class="sxs-lookup"><span data-stu-id="66250-122">If you want to export items with full fidelity, you can use the [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="66250-123">A operação **ExportItems** exporta cada item como um fluxo de dados.</span><span class="sxs-lookup"><span data-stu-id="66250-123">The **ExportItems** operation exports each item as a data stream.</span></span> <span data-ttu-id="66250-124">Esse fluxo de dados não é para análise, mas pode ser usado como um backup de nível de item que pode ser importado de volta para uma caixa de correio do Exchange.</span><span class="sxs-lookup"><span data-stu-id="66250-124">This data stream is not for parsing, but can be used as an item-level backup that can be imported back into an Exchange mailbox.</span></span> <span data-ttu-id="66250-125">Você pode incluir muitos itens em cada solicitação **ExportItems** , embora seja recomendável que você não inclua mais de 100 itens em cada chamada.</span><span class="sxs-lookup"><span data-stu-id="66250-125">You can include many items in each **ExportItems** request, although we recommend that you include no more than 100 items in each call.</span></span> <span data-ttu-id="66250-126">Como a API gerenciada do EWS não implementa a operação **ExportItems** , se você usar a API gerenciada do EWS, você precisará escrever uma rotina para enviar as solicitações da Web.</span><span class="sxs-lookup"><span data-stu-id="66250-126">Because the EWS Managed API does not implement the **ExportItems** operation, if you use the EWS Managed API, you'll need to write a routine to send the web requests.</span></span> <span data-ttu-id="66250-127">Opcionalmente, você pode usar o método [Item. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) para obter metadados sobre o item para que você possa indexar e armazenar informações sobre o fluxo de dados.</span><span class="sxs-lookup"><span data-stu-id="66250-127">You can optionally use the [Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method to get metadata about the item so that you can index and store information about the data stream.</span></span> 
  
<span data-ttu-id="66250-128">Recomendamos que você use a operação **ExportItems** para exportar itens que você planeja importar para uma caixa de correio do Exchange.</span><span class="sxs-lookup"><span data-stu-id="66250-128">We recommend that you use the **ExportItems** operation to export items that you plan to import into an Exchange mailbox.</span></span> 
  
<span data-ttu-id="66250-129">O exemplo a seguir mostra como usar a operação **ExportItems** .</span><span class="sxs-lookup"><span data-stu-id="66250-129">The following example shows how to use the **ExportItems** operation.</span></span> <span data-ttu-id="66250-130">Neste exemplo, o identificador de item é reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="66250-130">In this example, the item identifier is shortened for readability.</span></span> 
  
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

O servidor responde à solicitação **ExportItems** com um elemento [ExportItemsResponse](https://msdn.microsoft.com/library/ef44354b-fbdb-4f7c-b6bd-b27f56a1d018%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que o item foi exportado com êxito. A resposta também inclui a ID do item exportado e o fluxo de dados que contém o conteúdo exportado. <span data-ttu-id="66250-133">O exemplo a seguir mostra o corpo SOAP que contém o item exportado.</span><span class="sxs-lookup"><span data-stu-id="66250-133">The following example shows the SOAP body that contains the exported item.</span></span>
  
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

## <a name="use-the-mime-stream-to-export-into-common-file-formats"></a><span data-ttu-id="66250-134">Usar o fluxo MIME para exportar para formatos de arquivo comuns</span><span class="sxs-lookup"><span data-stu-id="66250-134">Use the MIME stream to export into common file formats</span></span>
<span data-ttu-id="66250-135"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="66250-135"><a name="bk_exportfullfidelity"> </a></span></span>

<span data-ttu-id="66250-136">Você pode usar o método [Item. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) de API gerenciada do EWS ou a operação [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS para obter uma representação MIME de um item.</span><span class="sxs-lookup"><span data-stu-id="66250-136">You can use the [Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) EWS Managed API method or the [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS operation to get a MIME representation of an item.</span></span> <span data-ttu-id="66250-137">Como o Exchange não armazena o conteúdo MIME de cada item, ele precisa converter a representação de banco de dados de cada item no fluxo MIME.</span><span class="sxs-lookup"><span data-stu-id="66250-137">Because Exchange doesn't store the MIME content of each item, it has to convert the database representation of each item into the MIME stream.</span></span> <span data-ttu-id="66250-138">Como essa conversão é cara, não recomendamos que você solicite o fluxo MIME para itens em uma escala grande.</span><span class="sxs-lookup"><span data-stu-id="66250-138">Because this conversion is costly, we do not recommend that you request the MIME stream for items on a large scale.</span></span> <span data-ttu-id="66250-139">Observe também que o fluxo MIME contém um conjunto limitado de propriedades; Você pode ter que considerar outras opções se o conjunto de propriedades não contiver as propriedades que você precisa.</span><span class="sxs-lookup"><span data-stu-id="66250-139">Also note that the MIME stream contains a limited set of properties; you might have to consider other options if the property set doesn't contain the properties you need.</span></span> 
  
### <a name="use-the-ews-managed-api-to-export-an-email-into-an-eml-and-mht-file-by-using-the-mime-stream"></a><span data-ttu-id="66250-140">Use a API gerenciada do EWS para exportar um email para um arquivo. eml e. mht usando o fluxo MIME</span><span class="sxs-lookup"><span data-stu-id="66250-140">Use the EWS Managed API to export an email into an .eml and .mht file by using the MIME stream</span></span>
<span data-ttu-id="66250-141"><a name="bk_exportemailmime"> </a></span><span class="sxs-lookup"><span data-stu-id="66250-141"><a name="bk_exportemailmime"> </a></span></span>

<span data-ttu-id="66250-142">O Outlook e outros aplicativos de email comuns podem abrir o formato de arquivo EML (. eml).</span><span class="sxs-lookup"><span data-stu-id="66250-142">Outlook and other common email applications can open the EML (.eml) file format.</span></span> <span data-ttu-id="66250-143">O exemplo a seguir mostra como você pode exportar um email usando o fluxo MIME e usar o fluxo MIME para criar um arquivo EML e HTML (. mht).</span><span class="sxs-lookup"><span data-stu-id="66250-143">The following example shows you how you can export an email by using the MIME stream, and use the MIME stream to create an EML and a MIME HTML (.mht) file.</span></span> <span data-ttu-id="66250-144">Muitos navegadores da Web oferecem suporte ao formato de arquivo MIME HTML.</span><span class="sxs-lookup"><span data-stu-id="66250-144">Many web browsers support the MIME HTML file format.</span></span> <span data-ttu-id="66250-145">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário pode autenticar em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="66250-145">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
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

### <a name="use-the-ews-managed-api-to-export-an-appointment-into-an-ical-file-by-using-the-mime-stream"></a><span data-ttu-id="66250-146">Usar a API gerenciada do EWS para exportar um compromisso para um arquivo iCal usando o fluxo MIME</span><span class="sxs-lookup"><span data-stu-id="66250-146">Use the EWS Managed API to export an appointment into an iCal file by using the MIME stream</span></span>
<span data-ttu-id="66250-147"><a name="bk_exporticalmime"> </a></span><span class="sxs-lookup"><span data-stu-id="66250-147"><a name="bk_exporticalmime"> </a></span></span>

<span data-ttu-id="66250-148">O Outlook e outros aplicativos de calendário comuns podem abrir o formato de arquivo iCal (. ICS).</span><span class="sxs-lookup"><span data-stu-id="66250-148">Outlook and other common calendar applications can open the iCal (.ics) file format.</span></span> <span data-ttu-id="66250-149">O exemplo a seguir mostra como exportar um compromisso usando o fluxo MIME e usar o fluxo MIME para criar um arquivo iCal.</span><span class="sxs-lookup"><span data-stu-id="66250-149">The following example shows you how to export an appointment by using the MIME stream, and use the MIME stream to create an iCal file.</span></span> <span data-ttu-id="66250-150">Observe que muitas propriedades não são exportadas com o fluxo MIME, incluindo participantes e propriedades relacionadas a anexos.</span><span class="sxs-lookup"><span data-stu-id="66250-150">Note that many properties are not exported with the MIME stream, including attendees and attachment-related properties.</span></span> <span data-ttu-id="66250-151">Você pode capturar outras propriedades do EWS solicitando-as e salvando-as no arquivo iCal como extensões privadas.</span><span class="sxs-lookup"><span data-stu-id="66250-151">You can capture other properties from EWS by requesting them and saving them in the iCal file as private extensions.</span></span> <span data-ttu-id="66250-152">Essas extensões privadas são prefixadas com "x-".</span><span class="sxs-lookup"><span data-stu-id="66250-152">These private extensions are prefixed with "x-".</span></span> 
  
<span data-ttu-id="66250-153">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário pode autenticar em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="66250-153">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> <span data-ttu-id="66250-154">Este exemplo também pressupõe que você tenha um compromisso com o assunto "projeções financeiras 2015" na pasta calendário.</span><span class="sxs-lookup"><span data-stu-id="66250-154">This example also assumes that you have an appointment with the subject "2015 Financial Projections" in the calendar folder.</span></span> 
  
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

### <a name="use-the-ews-managed-api-to-export-a-contact-into-a-vcard-file-by-using-the-mime-stream"></a><span data-ttu-id="66250-155">Usar a API gerenciada do EWS para exportar um contato para um arquivo vCard usando o fluxo MIME</span><span class="sxs-lookup"><span data-stu-id="66250-155">Use the EWS Managed API to export a contact into a vCard file by using the MIME stream</span></span>
<span data-ttu-id="66250-156"><a name="bk_exportvcardmime"> </a></span><span class="sxs-lookup"><span data-stu-id="66250-156"><a name="bk_exportvcardmime"> </a></span></span>

<span data-ttu-id="66250-157">O Outlook e outros aplicativos de gerenciamento de contato comuns podem abrir o formato de arquivo vCard (. vcf).</span><span class="sxs-lookup"><span data-stu-id="66250-157">Outlook and other common contact management applications can open the vCard (.vcf) file format.</span></span> <span data-ttu-id="66250-158">O exemplo a seguir mostra como exportar um contato usando o fluxo MIME e usar o fluxo MIME para criar um vCard.</span><span class="sxs-lookup"><span data-stu-id="66250-158">The following example shows you how to export a contact by using the MIME stream, and use the MIME stream to create a vCard.</span></span> <span data-ttu-id="66250-159">Você pode capturar outras propriedades do EWS solicitando-as e salvando-as no.</span><span class="sxs-lookup"><span data-stu-id="66250-159">You can capture other properties from EWS by requesting them and saving them in the .</span></span> <span data-ttu-id="66250-160">vCard como extensões privadas.</span><span class="sxs-lookup"><span data-stu-id="66250-160">vCard as private extensions.</span></span> <span data-ttu-id="66250-161">Essas extensões são prefixadas com "x-".</span><span class="sxs-lookup"><span data-stu-id="66250-161">These extensions are prefixed with "x-".</span></span> 
  
<span data-ttu-id="66250-162">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário pode autenticar em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="66250-162">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
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
> <span data-ttu-id="66250-163">Não é possível importar arquivos vCard usando a propriedade **MimeContent** .</span><span class="sxs-lookup"><span data-stu-id="66250-163">You cannot import vCard files by using the **MimeContent** property.</span></span> <span data-ttu-id="66250-164">Você pode importar contatos usando o [contato. salvar](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) o método de API gerenciada do EWS ou a operação [CreateItem](https://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) do EWS.</span><span class="sxs-lookup"><span data-stu-id="66250-164">You can import contacts by using the [Contact.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](https://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) EWS operation.</span></span> 
  
### <a name="use-ews-to-export-any-item-by-using-the-mime-stream"></a><span data-ttu-id="66250-165">Usar o EWS para exportar qualquer item usando o fluxo MIME</span><span class="sxs-lookup"><span data-stu-id="66250-165">Use EWS to export any item by using the MIME stream</span></span>
<span data-ttu-id="66250-166"><a name="bk_exportewsmime"> </a></span><span class="sxs-lookup"><span data-stu-id="66250-166"><a name="bk_exportewsmime"> </a></span></span>

<span data-ttu-id="66250-167">Use a operação **GetItem** para obter o fluxo MIME de um item.</span><span class="sxs-lookup"><span data-stu-id="66250-167">Use the **GetItem** operation to get the MIME stream of an item.</span></span> <span data-ttu-id="66250-168">A solicitação **GetItem** a seguir mostra como solicitar o conteúdo MIME de um item.</span><span class="sxs-lookup"><span data-stu-id="66250-168">The following **GetItem** request shows how to request the MIME content of an item.</span></span> 
  
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

<span data-ttu-id="66250-169">O exemplo a seguir mostra a resposta a uma solicitação para obter o fluxo MIME.</span><span class="sxs-lookup"><span data-stu-id="66250-169">The following example shows the response to a request to get the MIME stream.</span></span> <span data-ttu-id="66250-170">O fluxo MIME foi reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="66250-170">The MIME stream has been shortened for readability.</span></span>
  
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
<span data-ttu-id="66250-171"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="66250-171"><a name="bk_exportfullfidelity"> </a></span></span>

<span data-ttu-id="66250-172">Após exportar itens, talvez você queira [importar itens para o Exchange](how-to-import-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="66250-172">After exporting items, you might want to [import items into Exchange](how-to-import-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="66250-173">Confira também</span><span class="sxs-lookup"><span data-stu-id="66250-173">See also</span></span>


- [<span data-ttu-id="66250-174">Exportando e importando itens usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="66250-174">Exporting and importing items by using EWS in Exchange</span></span>](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="66250-175">Importar itens usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="66250-175">Import items by using EWS in Exchange</span></span>](how-to-import-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="66250-176">Pastas e itens no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="66250-176">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="66250-177">Sincronização de caixa de correio e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="66250-177">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

