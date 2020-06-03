---
title: Provisionar cabeçalhos x usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 45a99a14-a85f-47f8-af48-18eb6c6cc230
description: Saiba como provisionar cabeçalhos x para uma caixa de correio usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 409ddb944bbac7a60242de39cdf7ae13b17cc76a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527765"
---
# <a name="provision-x-headers-by-using-ews-in-exchange"></a><span data-ttu-id="e283d-103">Provisionar cabeçalhos x usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e283d-103">Provision x-headers by using EWS in Exchange</span></span>

<span data-ttu-id="e283d-104">Saiba como provisionar cabeçalhos x para uma caixa de correio usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="e283d-104">Learn how to provision x-headers for a mailbox by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="e283d-105">Os cabeçalhos X são cabeçalhos não padrão adicionados à coleção de cabeçalho de um email para comunicar informações.</span><span class="sxs-lookup"><span data-stu-id="e283d-105">X-headers are non-standard headers that are added to the header collection of an email to communicate information.</span></span> <span data-ttu-id="e283d-106">Por exemplo, o Exchange carimba mensagens com o cabeçalho **X-MS-Exchange-Organization-SCL** para indicar o nível de confiança de spam (SCL) atribuído ao email.</span><span class="sxs-lookup"><span data-stu-id="e283d-106">For example, Exchange stamps messages with the **X-MS-Exchange-Organization-SCL** header to indicate the spam confidence level (SCL) attributed to the email.</span></span> <span data-ttu-id="e283d-107">Clientes de email como o Outlook podem usar essas informações para determinar o tipo de ação a ser tomada no email (por exemplo, o Outlook pode impedir a exibição de imagens, a menos que o usuário execute uma ação).</span><span class="sxs-lookup"><span data-stu-id="e283d-107">Email clients like Outlook can use that information to determine what type of action to take on the email (for example, Outlook can prevent images from displaying unless the user takes an action).</span></span> 
  
<span data-ttu-id="e283d-108">O Exchange adiciona cabeçalhos x de entrada ao esquema de caixa de correio como uma propriedade nomeada na primeira vez que recebe um email com esse cabeçalho x.</span><span class="sxs-lookup"><span data-stu-id="e283d-108">Exchange adds incoming x-headers to the mailbox schema as a named property the first time it receives an email with that x-header.</span></span> <span data-ttu-id="e283d-109">O valor do cabeçalho x não é salvo nesse primeiro email; no entanto, ele é salvo em todos os emails subsequentes que incluem o cabeçalho x.</span><span class="sxs-lookup"><span data-stu-id="e283d-109">The x-header value is not saved on that first email; however, it is saved on all subsequent emails that include the x-header.</span></span> <span data-ttu-id="e283d-110">Por esse motivo, seu aplicativo deve provisionar cabeçalhos x antes de você esperar usá-los.</span><span class="sxs-lookup"><span data-stu-id="e283d-110">For this reason, your application should provision x-headers before you expect to use them.</span></span> <span data-ttu-id="e283d-111">O mapeamento entre uma propriedade nomeada e um cabeçalho x ocorre na entrega de transporte do email para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e283d-111">The mapping between a named property and an x-header occurs in the transport delivery of the email to the mailbox.</span></span> <span data-ttu-id="e283d-112">Isso significa que você precisa receber o email via entrega de transporte; Você não pode apenas salvar um email que inclua o cabeçalho x em uma caixa de correio para criar o mapeamento para uma propriedade nomeada.</span><span class="sxs-lookup"><span data-stu-id="e283d-112">This means that you need to receive the email via transport delivery; you cannot just save an email that includes the x-header to a mailbox to create the mapping to a named property.</span></span>
  
> [!NOTE]
> <span data-ttu-id="e283d-113">Se você descobrir que os cabeçalhos x não estão sendo salvos, determine se um [agente de transporte](https://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) ou um firewall de [cabeçalho](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx) está filtrando seus cabeçalhos x antes de chegar à caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e283d-113">If you find that x-headers aren't being saved, determine whether a [transport agent](https://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) or [header firewall](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx) is filtering out your x-headers before they get to the mailbox.</span></span> <span data-ttu-id="e283d-114">r</span><span class="sxs-lookup"><span data-stu-id="e283d-114">r</span></span>
  
## <a name="provision-an-x-header-by-using-the-ews-managed-api"></a><span data-ttu-id="e283d-115">Provisionar um cabeçalho x usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="e283d-115">Provision an x-header by using the EWS Managed API</span></span>
<span data-ttu-id="e283d-116"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="e283d-116"><a name="bk_example1"> </a></span></span>

<span data-ttu-id="e283d-117">O exemplo de código a seguir mostra como usar o método API gerenciada do EWS [EmailMessage. Send](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) para provisionar um cabeçalho x para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e283d-117">The following code example shows how to use the EWS Managed API [EmailMessage.Send](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) method to provision an x-header for a mailbox.</span></span> <span data-ttu-id="e283d-118">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que a caixa de correio de destino não excedeu a [cota para propriedades nomeadas](https://technet.microsoft.com/library/bb851492%28v=EXCHG.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="e283d-118">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the target mailbox hasn't exceeded the [quota for named properties](https://technet.microsoft.com/library/bb851492%28v=EXCHG.80%29.aspx).</span></span>
  
```cs
private static void ProvisionCustomXHeaderByEmail(ExchangeService service)
{
    // Create a definition for an extended property that will represent a custom x-header. X-headers must be created in the
    // InternetHeaders property set. The x-header name must match the name of the x-header sent in the subsequent emails so
    // the x-header and value are saved on the email.
    ExtendedPropertyDefinition xExperimentalHeader = new ExtendedPropertyDefinition(DefaultExtendedPropertySet.InternetHeaders,
                                                                                            "X-Experimental",
                                                                                            MapiPropertyType.String);
    // Create an item that is used to provision the custom x-header.
    EmailMessage email = new EmailMessage(service);
    email.ToRecipients.Add("user@contoso.com");
    email.SetExtendedProperty(xExperimentalHeader, "Provision X-Experimental Internet message header");
    try
    {
        // The mapping of the named property happens in transport delivery.
        email.Send();
        if (service.ServerInfo.MajorVersion == 12)
        {
            Console.WriteLine("Provisioned the X-Experimental across the mailbox database that hosts the user's mailbox.");
        }
        else // For versions of Exchange starting with Exchange 2010
        {
            Console.WriteLine("Provisioned the X-Experimental for the user's mailbox. You will need to run this " +
                                "for each mailbox that needs to process this x-header.");
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error: {0}", ex.Message);
    }
}
```

## <a name="provision-an-x-header-by-using-ews"></a><span data-ttu-id="e283d-119">Provisionar um cabeçalho x usando o EWS</span><span class="sxs-lookup"><span data-stu-id="e283d-119">Provision an x-header by using EWS</span></span>
<span data-ttu-id="e283d-120"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="e283d-120"><a name="bk_example1"> </a></span></span>

<span data-ttu-id="e283d-121">O exemplo de código a seguir mostra como usar a operação EWS [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) para criar e enviar um email para provisionar uma caixa de correio com um cabeçalho x.</span><span class="sxs-lookup"><span data-stu-id="e283d-121">The following code example shows how to use the EWS [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) operation to create and send an email to provision a mailbox with an x-header.</span></span> <span data-ttu-id="e283d-122">Esta é a solicitação XML que é enviada pela API gerenciada do EWS quando você [provisiona um cabeçalho x usando a API gerenciada do EWS](#bk_example1).</span><span class="sxs-lookup"><span data-stu-id="e283d-122">This is the XML request that is sent by the EWS Managed API when you [Provision an x-header by using the EWS Managed API](#bk_example1).</span></span>
  
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
    <m:CreateItem MessageDisposition="SendOnly">
      <m:Items>
        <t:Message>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI DistinguishedPropertySetId="InternetHeaders"
                                PropertyName="X-Experimental"
                                PropertyType="String" />
            <t:Value>Provision X-Experimental Internet message header</t:Value>
          </t:ExtendedProperty>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>user@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

## <a name="version-differences"></a><span data-ttu-id="e283d-123">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="e283d-123">Version differences</span></span>
<span data-ttu-id="e283d-124"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="e283d-124"><a name="bk_example1"> </a></span></span>

<span data-ttu-id="e283d-125">Na primeira vez que você provisionar um cabeçalho x no Exchange Online, o Exchange Online como parte do Office 365 ou uma versão local do Exchange que comece com o Exchange Server 2010, o valor de um novo cabeçalho x personalizado não será gravado na mensagem armazenada.</span><span class="sxs-lookup"><span data-stu-id="e283d-125">The first time that you provision an x-header in Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange Server 2010, the value of a new custom x-header will not be written to the stored message.</span></span> <span data-ttu-id="e283d-126">Isso ocorre porque o cabeçalho x deve primeiro ser mapeado para uma propriedade nomeada na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="e283d-126">This is because the x-header must first be mapped to a named property in the user's mailbox.</span></span> <span data-ttu-id="e283d-127">O mapeamento ocorre na primeira solicitação para adicionar as propriedades nomeadas.</span><span class="sxs-lookup"><span data-stu-id="e283d-127">The mapping occurs upon the first request to add the named properties.</span></span> <span data-ttu-id="e283d-128">Quando uma solicitação subsequente para criar a propriedade nomeada ocorre, a propriedade e o valor são armazenados na mensagem.</span><span class="sxs-lookup"><span data-stu-id="e283d-128">When a subsequent request to create the named property occurs, the property and value are stored on the message.</span></span> <span data-ttu-id="e283d-129">No Exchange 2007, a primeira vez que um cabeçalho x é gravado em um banco de dados de caixa de correio, um mapeamento é criado para o cabeçalho x para uma propriedade nomeada no banco de dados de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e283d-129">In Exchange 2007, the first time an x-header is written to a mailbox database, a mapping is created for the x-header to a named property across the mailbox database.</span></span> <span data-ttu-id="e283d-130">Quando uma solicitação subsequente para criar a propriedade nomeada ocorre, o cabeçalho x é processado e armazenado para qualquer caixa de correio no banco de dados do Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="e283d-130">When a subsequent request to create the named property occurs, the x-header is processed and stored for any mailbox in the Exchange 2007 database.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="e283d-131">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="e283d-131">Next steps</span></span>
<span data-ttu-id="e283d-132"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="e283d-132"><a name="bk_example1"> </a></span></span>

<span data-ttu-id="e283d-133">Este artigo mostra como provisionar um cabeçalho x para uma única caixa de correio enviando um email para um usuário.</span><span class="sxs-lookup"><span data-stu-id="e283d-133">This article shows you how to provision an x-header for a single mailbox by sending an email to a user.</span></span> <span data-ttu-id="e283d-134">Você também pode provisionar um cabeçalho x para muitos usuários [enviando um email em lotes para uma lista de destinatários](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) na organização do chamador.</span><span class="sxs-lookup"><span data-stu-id="e283d-134">You can also provision an x-header for many users by [sending a batch email to a list of recipients](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) in the caller's organization.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="e283d-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="e283d-135">See also</span></span>


- [<span data-ttu-id="e283d-136">Propriedades e propriedades estendidas no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e283d-136">Properties and extended properties in EWS in Exchange</span></span>](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [<span data-ttu-id="e283d-137">Exchange 2013: provisionar cabeçalhos X personalizados de forma programática</span><span class="sxs-lookup"><span data-stu-id="e283d-137">Exchange 2013: Provision custom X-headers programmatically</span></span>](https://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [<span data-ttu-id="e283d-138">Propriedades nomeadas, cabeçalhos X e você</span><span class="sxs-lookup"><span data-stu-id="e283d-138">Named Properties, X-Headers, and You</span></span>](https://blogs.technet.com/b/exchange/archive/2009/04/06/3407221.aspx)
    
- [<span data-ttu-id="e283d-139">Propriedades nomeadas, redondo 2: o que está em frente</span><span class="sxs-lookup"><span data-stu-id="e283d-139">Named Properties, Round 2: What lies Ahead</span></span>](https://blogs.technet.com/b/exchange/archive/2009/06/12/3407672.aspx)
    
- [<span data-ttu-id="e283d-140">Firewall de cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e283d-140">Header Firewall</span></span>](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="e283d-141">EWS, MIME e os cabeçalhos de mensagem da Internet ausentes</span><span class="sxs-lookup"><span data-stu-id="e283d-141">EWS, MIME, and the missing Internet message headers</span></span>](https://msdn.microsoft.com/library/office/hh545614%28v=exchg.140%29.aspx)
    
- [<span data-ttu-id="e283d-142">Processar mensagens de email em lotes usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e283d-142">Process email messages in batches by using EWS in Exchange</span></span>](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    

