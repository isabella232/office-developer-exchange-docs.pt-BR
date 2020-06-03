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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455783"
---
# <a name="get-user-photos-by-using-ews-in-exchange"></a><span data-ttu-id="2186f-103">Obter fotos do usuário usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2186f-103">Get user photos by using EWS in Exchange</span></span>

<span data-ttu-id="2186f-104">Saiba como obter fotos do usuário associadas a uma caixa de correio ou contato usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="2186f-104">Learn how to get user photos that are associated with a mailbox or contact by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="2186f-105">É bom colocar um rosto em um nome.</span><span class="sxs-lookup"><span data-stu-id="2186f-105">It's nice to put a face to a name.</span></span> <span data-ttu-id="2186f-106">Se seus usuários gostam de colocar nomes em faces, seu aplicativo pode solicitar uma imagem, normalmente uma foto, do Exchange que representa uma conta de email.</span><span class="sxs-lookup"><span data-stu-id="2186f-106">If your users like to put names to faces, your application can request an image, typically a photo, from Exchange that represents an email account.</span></span> <span data-ttu-id="2186f-107">Você pode obter uma foto de usuário armazenada em um servidor do Exchange para uma caixa de correio ou pode obter uma foto de contato de contatos armazenados na sua caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2186f-107">You can get a user photo stored on an Exchange server for a mailbox, or you can get a contact photo from contacts stored in your mailbox.</span></span>
  
<span data-ttu-id="2186f-108">Você pode usar várias tecnologias diferentes para obter fotos de caixas de correio ou dos serviços de domínio do Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="2186f-108">You can use several different technologies to get photos from mailboxes or Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="2186f-109">A melhor maneira de obter uma foto depende do tipo de contato do qual você deseja obter uma foto.</span><span class="sxs-lookup"><span data-stu-id="2186f-109">The best way to get a photo depends on the type of contact that you want to get a photo from.</span></span> 
  
<span data-ttu-id="2186f-110">**Tabela 1. Tecnologias a serem usadas para obter fotos do usuário com base no tipo de contato**</span><span class="sxs-lookup"><span data-stu-id="2186f-110">**Table 1. Technologies to use to get user photos based on contact type**</span></span>

|<span data-ttu-id="2186f-111">**Tipo de contato**</span><span class="sxs-lookup"><span data-stu-id="2186f-111">**Contact type**</span></span>|<span data-ttu-id="2186f-112">**Tecnologias a serem usadas**</span><span class="sxs-lookup"><span data-stu-id="2186f-112">**Technologies to use**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2186f-113">Foto do usuário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="2186f-113">Mailbox user photo</span></span>  <br/> |[<span data-ttu-id="2186f-114">Obter uma foto de usuário de caixa de correio usando REST</span><span class="sxs-lookup"><span data-stu-id="2186f-114">Get a mailbox user photo by using REST</span></span>](#bk_REST)<br/><br/> [<span data-ttu-id="2186f-115">Obter uma foto do usuário usando o EWS</span><span class="sxs-lookup"><span data-stu-id="2186f-115">Get a user photo by using EWS</span></span>](#bk_EWS) <br/> |
|<span data-ttu-id="2186f-116">Foto do usuário de contato</span><span class="sxs-lookup"><span data-stu-id="2186f-116">Contact user photo</span></span>  <br/> |[<span data-ttu-id="2186f-117">Obter uma foto de usuário de contato usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="2186f-117">Get a contact user photo by using EWS Managed API</span></span>](#bk_EWSMA)<br/><br/> [<span data-ttu-id="2186f-118">Obter uma foto do usuário usando o EWS</span><span class="sxs-lookup"><span data-stu-id="2186f-118">Get a user photo by using EWS</span></span>](#bk_EWS) <br/> |

<span data-ttu-id="2186f-119"><a name="bk_REST"> </a></span><span class="sxs-lookup"><span data-stu-id="2186f-119"><a name="bk_REST"> </a></span></span>

## <a name="get-a-mailbox-user-photo-by-using-rest"></a><span data-ttu-id="2186f-120">Obter uma foto de usuário de caixa de correio usando REST</span><span class="sxs-lookup"><span data-stu-id="2186f-120">Get a mailbox user photo by using REST</span></span>

<span data-ttu-id="2186f-121">Você pode solicitar fotos de usuários de um servidor Exchange usando uma solicitação de http **Get** padrão.</span><span class="sxs-lookup"><span data-stu-id="2186f-121">You can request user photos from an Exchange server by using a standard HTTPS **GET** request.</span></span> <span data-ttu-id="2186f-122">Na solicitação, especifique o endereço da conta de email e um código de tamanho para a imagem, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="2186f-122">In the request, specify the email account address and a size code for the image, as shown in the following example.</span></span> 
  
```HTML
https://Exchange Server/ews/Exchange.asmx/s/GetUserPhoto?email=email address&amp;size=size code
```

<span data-ttu-id="2186f-123">Use a operação [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) do serviço de descoberta automática para recuperar a configuração **ExternalEwsUrl** , que contém a URL do ponto de extremidade dos serviços Web do Exchange (EWS) e o local do manipulador http **Exchange. asmx** que retorna as fotos do usuário.</span><span class="sxs-lookup"><span data-stu-id="2186f-123">Use the Autodiscover service [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) operation to retrieve the **ExternalEwsUrl** setting, which contains the URL of the Exchange Web Services (EWS) endpoint and the location of the **Exchange.asmx** HTTP handler that returns the user photos.</span></span> 
  
<span data-ttu-id="2186f-124">Cada código de tamanho indica a altura e a largura da imagem em pixels.</span><span class="sxs-lookup"><span data-stu-id="2186f-124">Each size code indicates the height and width of the image in pixels.</span></span> <span data-ttu-id="2186f-125">Por exemplo, o código de tamanho **HR48x48** retorna uma imagem que tem 48 pixels de altura por 48 pixels de largura.</span><span class="sxs-lookup"><span data-stu-id="2186f-125">For example, the size code **HR48x48** returns an image that is 48 pixels high by 48 pixels wide.</span></span> <span data-ttu-id="2186f-126">Os valores possíveis para o parâmetro de código de tamanho são os mesmos valores possíveis para o elemento [SizeRequested](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2186f-126">The possible values for the size code parameter are the same as the possible values for the [SizeRequested](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="2186f-127">Se a solicitação especificar um tamanho que não está disponível, a maior foto disponível será retornada.</span><span class="sxs-lookup"><span data-stu-id="2186f-127">If the request specifies a size that is not available, the largest available photo will be returned.</span></span> <span data-ttu-id="2186f-128">Se nenhuma foto estiver armazenada no servidor do Exchange, a imagem em miniatura armazenada no AD DS para a conta será retornada.</span><span class="sxs-lookup"><span data-stu-id="2186f-128">If no photo is stored on the Exchange server, the thumbnail image stored in AD DS for the account will be returned.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2186f-129">O código de tamanho **HR48x48** sempre retorna a imagem em miniatura do AD DS, se estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="2186f-129">The **HR48x48** size code always returns the AD DS thumbnail image if it is available.</span></span> 
  
<span data-ttu-id="2186f-130">O exemplo a seguir mostra como você pode usar a solicitação GET para recuperar a foto do usuário para o Sadie e salvá-la no computador local.</span><span class="sxs-lookup"><span data-stu-id="2186f-130">The following example shows how you can use the GET request to retrieve the user photo for Sadie and save it to your local computer.</span></span>
  
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

<span data-ttu-id="2186f-131">A solicitação retornará uma resposta HTTP.</span><span class="sxs-lookup"><span data-stu-id="2186f-131">The request will return an HTTP response.</span></span> 
  
<span data-ttu-id="2186f-132">**Tabela 2. Códigos de resposta para uma solicitação GetUserPhoto**</span><span class="sxs-lookup"><span data-stu-id="2186f-132">**Table 2. Response codes for a GetUserPhoto request**</span></span>

|<span data-ttu-id="2186f-133">**Código de resposta**</span><span class="sxs-lookup"><span data-stu-id="2186f-133">**Response code**</span></span>|<span data-ttu-id="2186f-134">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2186f-134">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2186f-135">200</span><span class="sxs-lookup"><span data-stu-id="2186f-135">200</span></span>  <br/> |<span data-ttu-id="2186f-136">Uma imagem está disponível para a conta de email especificada e a imagem binária está contida na resposta.</span><span class="sxs-lookup"><span data-stu-id="2186f-136">An image is available for the specified email account and the binary image is contained in the response.</span></span>  <br/> |
|<span data-ttu-id="2186f-137">304</span><span class="sxs-lookup"><span data-stu-id="2186f-137">304</span></span>  <br/> |<span data-ttu-id="2186f-138">A imagem não foi alterada desde a última vez que **ETag** foi retornado para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2186f-138">The image has not changed since the last time the **ETag** was returned to the application.</span></span>  <br/> |
|<span data-ttu-id="2186f-139">404</span><span class="sxs-lookup"><span data-stu-id="2186f-139">404</span></span>  <br/> |<span data-ttu-id="2186f-140">Nenhuma imagem está disponível para a conta de email especificada.</span><span class="sxs-lookup"><span data-stu-id="2186f-140">No image is available for the specified email account.</span></span>  <br/> |

<span data-ttu-id="2186f-141"><a name="bk_REST"> </a></span><span class="sxs-lookup"><span data-stu-id="2186f-141"><a name="bk_REST"> </a></span></span>

## <a name="cache-user-photos"></a><span data-ttu-id="2186f-142">Armazenar em cache fotos do usuário</span><span class="sxs-lookup"><span data-stu-id="2186f-142">Cache user photos</span></span>

<span data-ttu-id="2186f-143">O Exchange retorna os dados com um tipo de conteúdo image/jpeg, juntamente com uma coleção de valores de cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="2186f-143">Exchange returns the data with a content type of image/jpeg, along with a collection of header values.</span></span> <span data-ttu-id="2186f-144">O cabeçalho **ETag** é semelhante a uma chave de alteração.</span><span class="sxs-lookup"><span data-stu-id="2186f-144">The **ETag** header is similar to a change key.</span></span> <span data-ttu-id="2186f-145">O valor é uma cadeia de caracteres que representa a última vez que a foto foi atualizada.</span><span class="sxs-lookup"><span data-stu-id="2186f-145">The value is a string that represents the last time the photo was updated.</span></span> <span data-ttu-id="2186f-146">A **ETag** permanece a mesma para a foto do usuário até que a foto seja alterada.</span><span class="sxs-lookup"><span data-stu-id="2186f-146">The **ETag** remains the same for the user photo until the photo is changed.</span></span> <span data-ttu-id="2186f-147">Você pode enviar esse valor de **ETag** para o servidor na solicitação **Get** de HTTPS em um cabeçalho **If-None-Match** .</span><span class="sxs-lookup"><span data-stu-id="2186f-147">You can send this **ETag** value to the server in the HTTPS **GET** request in an **If-None-Match** header.</span></span> <span data-ttu-id="2186f-148">Se a foto não tiver sido alterada desde a última solicitação, o servidor responderá com uma resposta HTTP 304 que indica como tal.</span><span class="sxs-lookup"><span data-stu-id="2186f-148">If the photo hasn't changed since the last request, the server will respond with an HTTP 304 response that indicates as such.</span></span> <span data-ttu-id="2186f-149">Isso significa que você pode usar a foto do usuário que você solicitou e salvou anteriormente, em vez de processar um novo.</span><span class="sxs-lookup"><span data-stu-id="2186f-149">This means that you can use the user photo that you previously requested and saved rather than processing a new one.</span></span> 

<span data-ttu-id="2186f-150"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="2186f-150"><a name="bk_EWSMA"> </a></span></span>

## <a name="get-a-contact-user-photo-by-using-ews-managed-api"></a><span data-ttu-id="2186f-151">Obter uma foto de usuário de contato usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="2186f-151">Get a contact user photo by using EWS Managed API</span></span>

<span data-ttu-id="2186f-152">Seu aplicativo pode usar a API gerenciada do EWS para recuperar fotos de contatos, se o contato estiver armazenado em uma pasta de contatos na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="2186f-152">Your application can use the EWS Managed API to retrieve photos for contacts, if the contact is stored in a contact folder in the user's mailbox.</span></span> <span data-ttu-id="2186f-153">Para fazer isso, primeiro, encontre o **ItemId** do contato que você deseja usar.</span><span class="sxs-lookup"><span data-stu-id="2186f-153">To do this, first, find the **ItemId** for the contact you want use.</span></span> <span data-ttu-id="2186f-154">Depois, depois de associar a esse contato, carregue-o na coleção Attachments.</span><span class="sxs-lookup"><span data-stu-id="2186f-154">Then, after you bind to that contact, load it to the attachments collection.</span></span> <span data-ttu-id="2186f-155">Se o contato tiver uma foto, a foto será um dos anexos.</span><span class="sxs-lookup"><span data-stu-id="2186f-155">If the contact has a photo, the photo will be one of the attachments.</span></span> <span data-ttu-id="2186f-156">Percorra a coleção Attachments, verificando o valor da propriedade **IsContactPhoto** .</span><span class="sxs-lookup"><span data-stu-id="2186f-156">Loop through the attachments collection, checking the value of the **IsContactPhoto** property.</span></span> <span data-ttu-id="2186f-157">Quando você encontrar a foto do contato, poderá salvá-la no computador local e o aplicativo poderá acessá-la.</span><span class="sxs-lookup"><span data-stu-id="2186f-157">When you find the contact photo, you can save it to your local computer, and your application can access it.</span></span> 
  
<span data-ttu-id="2186f-158">O exemplo a seguir mostra esse processo.</span><span class="sxs-lookup"><span data-stu-id="2186f-158">The following example shows this process.</span></span> <span data-ttu-id="2186f-159">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="2186f-159">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="2186f-160"><a name="bk_EWS"> </a></span><span class="sxs-lookup"><span data-stu-id="2186f-160"><a name="bk_EWS"> </a></span></span>

## <a name="get-a-user-photo-by-using-ews"></a><span data-ttu-id="2186f-161">Obter uma foto do usuário usando o EWS</span><span class="sxs-lookup"><span data-stu-id="2186f-161">Get a user photo by using EWS</span></span>

<span data-ttu-id="2186f-162">Se você estiver obtendo uma foto de usuário do AD DS, poderá usar a operação [GetUserPhoto](https://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) (se souber o endereço de email) ou a operação [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) (se não souber o endereço de email).</span><span class="sxs-lookup"><span data-stu-id="2186f-162">If you're getting a user photo from AD DS, you can use the [GetUserPhoto](https://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) operation (if you know the email address) or the [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation (if you don't know the email address).</span></span> <span data-ttu-id="2186f-163">Se você estiver obtendo uma foto de usuário de uma pasta contatos na caixa de correio, use a operação [GetItem](https://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) seguida pela operação [GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2186f-163">If you're getting a user photo from a contacts folder in the mailbox, use the [GetItem](https://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) operation followed by the [GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="2186f-164">Em ambos os casos, a foto é retornada como uma cadeia de caracteres codificada em base64 na resposta XML.</span><span class="sxs-lookup"><span data-stu-id="2186f-164">In either case, the photo is returned as a Base64-encoded string in the XML response.</span></span> 
  
### <a name="get-a-mailbox-user-photo-by-using-the-getuserphoto-operation"></a><span data-ttu-id="2186f-165">Obter uma foto de usuário de caixa de correio usando a operação GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="2186f-165">Get a mailbox user photo by using the GetUserPhoto operation</span></span>

<span data-ttu-id="2186f-166">O uso da operação **GetUserPhoto** é simples.</span><span class="sxs-lookup"><span data-stu-id="2186f-166">Using the **GetUserPhoto** operation is straightforward.</span></span> <span data-ttu-id="2186f-167">Na solicitação XML, especifique o endereço de email do usuário e o [tamanho da foto](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) a ser retornado (no elemento [SizeRequested](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) ).</span><span class="sxs-lookup"><span data-stu-id="2186f-167">In the XML request, specify the email address of the user, and the [size of the photo](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) to return (in the [SizeRequested](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) element).</span></span> <span data-ttu-id="2186f-168">O exemplo de solicitação XML a seguir mostra como obter uma foto para Sadie Daniels de 360 pixels de largura por 360 pixels de altura.</span><span class="sxs-lookup"><span data-stu-id="2186f-168">The following XML request example shows how to get a photo for Sadie Daniels that's 360 pixels wide by 360 pixels high.</span></span> 
  
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

<span data-ttu-id="2186f-169">Veja a seguir a resposta de XML.</span><span class="sxs-lookup"><span data-stu-id="2186f-169">The following is the XML response.</span></span> <span data-ttu-id="2186f-170">A foto codificada em base64 está contida no elemento [PictureData](https://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) (o conteúdo foi reduzido para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="2186f-170">The Base64-encoded photo is contained in the [PictureData](https://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) element (the content has been shortened for readability).</span></span> 
  
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

### <a name="get-a-mailbox-user-photo-by-using-the-resolvenames-operation"></a><span data-ttu-id="2186f-171">Obter uma foto de usuário de caixa de correio usando a operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="2186f-171">Get a mailbox user photo by using the ResolveNames operation</span></span>

<span data-ttu-id="2186f-172">Se você não souber o endereço de email do usuário para o qual você está obtendo uma foto, poderá [usar a operação ResolveNames](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md) para obter candidatos para uma possível correspondência.</span><span class="sxs-lookup"><span data-stu-id="2186f-172">If you don't know the email address of the user for whom you are getting a photo, you can [use the ResolveNames operation](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md) to get candidates for a possible match.</span></span> <span data-ttu-id="2186f-173">Se você especificar "myproperties" para o atributo **ContactDataShape** do elemento [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) , muitos dados, incluindo as fotos do usuário, serão retornados para cada candidato.</span><span class="sxs-lookup"><span data-stu-id="2186f-173">If you specify "AllProperties" for the **ContactDataShape** attribute of the [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) element, a lot of data, including user photos, will be returned for each candidate.</span></span> <span data-ttu-id="2186f-174">O exemplo a seguir mostra a solicitação XML para resolver o nome "Sadie" e retornar todas as propriedades de cada candidato.</span><span class="sxs-lookup"><span data-stu-id="2186f-174">The following example shows the XML request to resolve the name "Sadie" and return all the properties for each candidate.</span></span> 
  
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

<span data-ttu-id="2186f-175">Um grande volume de dados será retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="2186f-175">A lot of data will be returned in the response.</span></span> <span data-ttu-id="2186f-176">O exemplo a seguir mostra somente os dados relevantes para a foto do usuário.</span><span class="sxs-lookup"><span data-stu-id="2186f-176">The following example shows only the data that is relevant to the user photo.</span></span> <span data-ttu-id="2186f-177">O elemento **Photo** contém a foto de usuário codificada em Base64 (o conteúdo foi reduzido para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="2186f-177">The **Photo** element contains the Base64-encoded user photo (the content has been shortened for readability).</span></span> 
  
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

### <a name="get-a-contact-user-photo-by-using-the-getattachment-operation"></a><span data-ttu-id="2186f-178">Obter uma foto de usuário de contato usando a operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="2186f-178">Get a contact user photo by using the GetAttachment operation</span></span>

<span data-ttu-id="2186f-179">Você pode usar o EWS para obter fotos de contatos armazenados na sua caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2186f-179">You can use EWS to get photos from contacts stored in your mailbox.</span></span> <span data-ttu-id="2186f-180">Primeiro, use a operação **GetItem** para retornar todas as propriedades para que você possa procurar fotos.</span><span class="sxs-lookup"><span data-stu-id="2186f-180">First, you use the **GetItem** operation to return all properties so you can look for photos.</span></span> <span data-ttu-id="2186f-181">O exemplo a seguir mostra uma solicitação XML para obter um item de contato.</span><span class="sxs-lookup"><span data-stu-id="2186f-181">The following example shows an XML request to get a contact item.</span></span> <span data-ttu-id="2186f-182">A ID do item foi reduzida para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2186f-182">The item ID has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="2186f-183">Procure o elemento [HasPicture](https://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) para verificar se o contato tem uma foto associada.</span><span class="sxs-lookup"><span data-stu-id="2186f-183">Look for the [HasPicture](https://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) element to verify that the contact has an associated photo.</span></span> <span data-ttu-id="2186f-184">Em seguida, examine a coleção de anexos para um que tenha um valor de true para o elemento [IsContactPhoto](https://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2186f-184">Then look through the collection of attachments for one that has a value of true for the [IsContactPhoto](https://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="2186f-185">O exemplo de resposta a seguir mostra apenas os dados relevantes.</span><span class="sxs-lookup"><span data-stu-id="2186f-185">The following response example shows only the relevant data.</span></span> <span data-ttu-id="2186f-186">Os valores de ID são reduzidos para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2186f-186">The ID values are shortened for readability.</span></span> 
  
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

Em seguida, use a operação **GetAttachment** com o **attachmentid** para solicitar o anexo que tem a foto de contato. O exemplo a seguir mostra a solicitação XML para obter o anexo. <span data-ttu-id="2186f-189">A ID é reduzida para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2186f-189">The ID is shortened for readability.</span></span> 
  
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

O exemplo a seguir mostra a resposta XML com as informações sobre o anexo solicitado. <span data-ttu-id="2186f-191">O elemento [Content](https://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) contém a cadeia de caracteres codificada em base64 para a foto do usuário, abreviado neste exemplo para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2186f-191">The [Content](https://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) element contains the Base64-encoded string for the user photo, shortened in this example for readability.</span></span> 
  
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

<span data-ttu-id="2186f-192"><a name="bk_EWS"> </a></span><span class="sxs-lookup"><span data-stu-id="2186f-192"><a name="bk_EWS"> </a></span></span>

## <a name="decode-a-base64-encoded-string"></a><span data-ttu-id="2186f-193">Decodificar uma cadeia de caracteres codificada em base64</span><span class="sxs-lookup"><span data-stu-id="2186f-193">Decode a Base64-encoded string</span></span>

<span data-ttu-id="2186f-194">Independentemente da operação que você usa para obter uma foto do usuário, você precisará decodificar essa cadeia de caracteres para usá-la em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2186f-194">Regardless of the operation you use to get a user photo, you'll need to decode that string so you can use it in your application.</span></span> <span data-ttu-id="2186f-195">O exemplo a seguir mostra como decodificar a cadeia de caracteres e, em seguida, salvá-la no computador local para que o aplicativo possa acessá-la mais tarde.</span><span class="sxs-lookup"><span data-stu-id="2186f-195">The following example shows how to decode the string, and then save it to your local computer so you application can access it later.</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="2186f-196">Confira também</span><span class="sxs-lookup"><span data-stu-id="2186f-196">See also</span></span>

- [<span data-ttu-id="2186f-197">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2186f-197">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)    
- [<span data-ttu-id="2186f-198">Resolver nomes ambíguos usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="2186f-198">Resolve ambiguous names by using EWS in Exchange 2013</span></span>](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)    
- [<span data-ttu-id="2186f-199">Processar contatos em lotes usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2186f-199">Process contacts in batches by using EWS in Exchange</span></span>](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    

