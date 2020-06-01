---
title: Operação MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1f71f04d-56a9-4fee-a4e7-d1034438329e
description: Encontre informações sobre a operação do EWS do MarkAsJunk.
ms.openlocfilehash: 25d6b01dfff64c4e45f3382223311219d349c165
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468569"
---
# <a name="markasjunk-operation"></a><span data-ttu-id="074ce-103">Operação MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="074ce-103">MarkAsJunk operation</span></span>

<span data-ttu-id="074ce-104">Encontre informações sobre a operação do EWS do **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="074ce-104">Find information about the **MarkAsJunk** EWS operation.</span></span> 
  
<span data-ttu-id="074ce-105">A operação **MarkAsJunk** adiciona e remove usuários da lista de e-mails bloqueados e move mensagens de email para a pasta lixo eletrônico.</span><span class="sxs-lookup"><span data-stu-id="074ce-105">The **MarkAsJunk** operation adds and removes users from the blocked email list and moves email messages to the Junk Email folder.</span></span> 
  
<span data-ttu-id="074ce-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="074ce-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-markasjunk-operation"></a><span data-ttu-id="074ce-107">Usando a operação MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="074ce-107">Using the MarkAsJunk operation</span></span>

<span data-ttu-id="074ce-108">A operação **MarkAsJunk** contém duas opções booleanas para indicar se um remetente de email deve ser adicionado à lista de remetentes bloqueados e se a mensagem de email de destino deve ser movida para a pasta de lixo eletrônico padrão ou para a pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="074ce-108">The **MarkAsJunk** operation contains two Boolean options to indicate whether an email sender should be added to the blocked sender list and whether the target email message should be moved to the default Junk Email folder or the Inbox folder.</span></span> <span data-ttu-id="074ce-109">As ações são determinadas pelos valores dos atributos **islixo** e **MoveItem** .</span><span class="sxs-lookup"><span data-stu-id="074ce-109">The actions are determined by the values of the **IsJunk** and **MoveItem** attributes.</span></span> <span data-ttu-id="074ce-110">A seguir estão as ações possíveis com base nas combinações de valor dos atributos **isjunk** e **MoveItem** :</span><span class="sxs-lookup"><span data-stu-id="074ce-110">The following are the possible actions based on the value combinations for the **IsJunk** and **MoveItem** attributes:</span></span> 
  
- <span data-ttu-id="074ce-111">Se o atributo **islixo** estiver definido como **true**e o atributo **MoveItem** estiver definido como **true**, o remetente da mensagem de email de destino será adicionado à lista de remetentes bloqueados e a mensagem de email será movida para a pasta lixo eletrônico.</span><span class="sxs-lookup"><span data-stu-id="074ce-111">If the **IsJunk** attribute is set to **true**, and the **MoveItem** attribute is set to **true**, the sender of the target email message is added to the blocked sender list and the email message is moved to the Junk Dmail folder.</span></span>
    
- <span data-ttu-id="074ce-112">Se o atributo **islixo** estiver definido como **true**e o atributo **MoveItem** estiver definido como **false**, o remetente da mensagem de email de destino será adicionado à lista de remetentes bloqueados e a mensagem de email não será movida da pasta.</span><span class="sxs-lookup"><span data-stu-id="074ce-112">If the **IsJunk** attribute is set to **true**, and the **MoveItem** attribute is set to **false**, the sender of the target email message is added to the blocked sender list and the email message is not moved from the folder.</span></span>
    
- <span data-ttu-id="074ce-113">Se o atributo **isjunk** for definido como **false**e o atributo **MoveItem** estiver definido como **true**, o remetente da mensagem de email de destino será removido da lista de remetentes bloqueados e a mensagem de email será movida para a pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="074ce-113">If the **IsJunk** attribute is set to **false**, and the **MoveItem** attribute is set to **true**, the sender of the target email messageis removed from the blocked sender list and the email message is moved to the Inbox folder.</span></span>
    
- <span data-ttu-id="074ce-114">Se o atributo **isjunk** for definido como **false**e o atributo **MoveItem** for definido como **false**, o remetente da mensagem de email de destino será removido da lista de remetentes bloqueados e a mensagem de email não será movida da pasta.</span><span class="sxs-lookup"><span data-stu-id="074ce-114">If the **IsJunk** attribute is set to **false**, and the **MoveItem** attribute is set to **false**, the sender of the target email message is removed from the blocked sender list and the email message is not moved from the folder.</span></span>
    
> [!IMPORTANT]
> <span data-ttu-id="074ce-115">O conteúdo da lista de remetentes bloqueados não é detectável do EWS.</span><span class="sxs-lookup"><span data-stu-id="074ce-115">The contents of the blocked sender list are not discoverable from EWS.</span></span> <span data-ttu-id="074ce-116">Se um remetente for adicionado à lista de remetentes bloqueados, você precisará manter uma cópia de uma mensagem de email enviada pelo remetente bloqueado para desbloquear o remetente no futuro.</span><span class="sxs-lookup"><span data-stu-id="074ce-116">If a sender is added to the blocked sender list, you need to keep a copy of an email message sent by the blocked sender to unblock the sender in the future.</span></span> 
  
### <a name="markasjunk-operation-soap-headers"></a><span data-ttu-id="074ce-117">Cabeçalhos SOAP de operação MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="074ce-117">MarkAsJunk operation SOAP headers</span></span>

<span data-ttu-id="074ce-118">A operação **MarkAsJunk** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="074ce-118">The **MarkAsJunk** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="074ce-119">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="074ce-119">**Header name**</span></span>|<span data-ttu-id="074ce-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="074ce-120">**Element**</span></span>|<span data-ttu-id="074ce-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="074ce-121">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="074ce-122">**Representação**</span><span class="sxs-lookup"><span data-stu-id="074ce-122">**Impersonation**</span></span> <br/> |[<span data-ttu-id="074ce-123">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="074ce-123">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="074ce-124">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="074ce-124">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="074ce-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="074ce-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="074ce-126">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="074ce-126">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="074ce-127">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="074ce-127">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="074ce-128">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="074ce-128">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="074ce-129">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="074ce-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="074ce-130">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="074ce-130">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="074ce-131">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="074ce-131">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="074ce-132">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="074ce-132">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="074ce-133">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="074ce-133">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="074ce-134">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="074ce-134">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="074ce-135">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="074ce-135">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="074ce-136">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="074ce-136">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="074ce-137">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="074ce-137">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a><span data-ttu-id="074ce-138">Exemplo de solicitação de operação MarkAsJunk: adicionar um remetente à lista de remetentes bloqueados</span><span class="sxs-lookup"><span data-stu-id="074ce-138">MarkAsJunk operation request example: Add a sender to the blocked sender list</span></span>

<span data-ttu-id="074ce-139">O exemplo a seguir de uma solicitação de operação **MarkAsJunk** mostra como adicionar o remetente de um email à lista de remetentes bloqueados e mover o email para a pasta lixo eletrônico.</span><span class="sxs-lookup"><span data-stu-id="074ce-139">The following example of a **MarkAsJunk** operation request shows how to add the sender of an email to the blocked sender list and move the email to the junk mail folder.</span></span> <span data-ttu-id="074ce-140">A operação **MarkAsJunk** aceita o identificador de mensagem de email exclusivo para identificar o email que é usado para fazer referência ao remetente adicionado à lista de remetentes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="074ce-140">The **MarkAsJunk** operation accepts the unique email message identifier to identify the email that is used to reference the sender that is added to the blocked sender list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="074ce-141">Todos os identificadores de item e as chaves de alteração deste artigo foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="074ce-141">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
        <t:RequestServerVersion Version="Exchange2013" />
    </soap:Header>
    <soap:Body>
        <m:MarkAsJunk IsJunk="true" MoveItem="true">
            <m:ItemIds>
                <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYA" />
            </m:ItemIds>
        </m:MarkAsJunk>
    </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="074ce-142">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="074ce-142">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="074ce-143">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="074ce-143">MarkAsJunk</span></span>](markasjunk.md)
    
- [<span data-ttu-id="074ce-144">ItemIds</span><span class="sxs-lookup"><span data-stu-id="074ce-144">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="074ce-145">ItemId</span><span class="sxs-lookup"><span data-stu-id="074ce-145">ItemId</span></span>](itemid.md)
    
## <a name="successful-markasjunk-operation-response"></a><span data-ttu-id="074ce-146">Resposta de operação MarkAsJunk bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="074ce-146">Successful MarkAsJunk operation response</span></span>

<span data-ttu-id="074ce-147">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação de **MarkAsJunk** para adicionar um remetente à lista de remetentes bloqueados e mover a mensagem de email para a pasta lixo eletrônico.</span><span class="sxs-lookup"><span data-stu-id="074ce-147">The following example shows a successful response to a **MarkAsJunk** operation request to add a sender to the blocked sender list and move the email message to the Junk Email folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                             MinorVersion="0" 
                             MajorBuildNumber="545" 
                             MinorBuildNumber="11" 
                             Version="Exchange2013" 
                             xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                             xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
        <m:MarkAsJunkResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
           <m:ResponseMessages>
               <m:MarkAsJunkResponseMessage ResponseClass="Success">
                  <m:ResponseCode>NoError</m:ResponseCode>
                 <m:MovedItemId Id="AAMkAD=" ChangeKey="CQAAABYu" />
               </m:MarkAsJunkResponseMessage>
           </m:ResponseMessages>
        </m:MarkAsJunkResponse>
    </s:Body>
</s:Envelope>
```

<span data-ttu-id="074ce-148">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="074ce-148">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="074ce-149">MarkAsJunkResponse</span><span class="sxs-lookup"><span data-stu-id="074ce-149">MarkAsJunkResponse</span></span>](markasjunkresponse.md)
    
- [<span data-ttu-id="074ce-150">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="074ce-150">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="074ce-151">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="074ce-151">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
    
- [<span data-ttu-id="074ce-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="074ce-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="074ce-153">MovedItemId</span><span class="sxs-lookup"><span data-stu-id="074ce-153">MovedItemId</span></span>](moveditemid.md)
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a><span data-ttu-id="074ce-154">Exemplo de solicitação de operação MarkAsJunk: remover um remetente da lista de remetentes bloqueados</span><span class="sxs-lookup"><span data-stu-id="074ce-154">MarkAsJunk operation request example: Remove a sender from the blocked sender list</span></span>

<span data-ttu-id="074ce-155">O exemplo a seguir de uma solicitação de operação **MarkAsJunk** mostra como remover o remetente de uma mensagem de email da lista de remetentes bloqueados e mover a mensagem de email para a pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="074ce-155">The following example of a **MarkAsJunk** operation request shows how to remove the sender of an email message from the blocked sender list and move the email message to the Inbox folder.</span></span> <span data-ttu-id="074ce-156">Você precisa manter uma mensagem de email enviada pelo remetente bloqueado para remover o remetente da lista de remetentes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="074ce-156">You need to keep an email message sent by the blocked sender to remove the sender from the blocked sender list.</span></span> <span data-ttu-id="074ce-157">O endereço de email do remetente é associado a mensagens de email enviadas pelo remetente.</span><span class="sxs-lookup"><span data-stu-id="074ce-157">The sender's email address is associated with email messages that have been sent by the sender.</span></span> <span data-ttu-id="074ce-158">A remoção de um remetente da lista de remetentes bloqueados não será bem-sucedida se a mensagem de email de referência não existir mais na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="074ce-158">Removing a sender from the blocked sender list will not succeed if the reference email message no longer exists in the user's mailbox.</span></span> <span data-ttu-id="074ce-159">O identificador de item usado para associar uma mensagem de email ao remetente deve estar associado a um item que existe na caixa de correio do Exchange.</span><span class="sxs-lookup"><span data-stu-id="074ce-159">The item identifier used to associate an email message with its sender must be associated with an item that exists in the Exchange mailbox.</span></span> <span data-ttu-id="074ce-160">Recomendamos que você crie uma pasta oculta para armazenar itens enviados por remetentes bloqueados anteriormente para que os remetentes possam ser desbloqueados do aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="074ce-160">We recommend that you create a hidden folder to store items sent by previously blocked senders so that the senders can be unblocked from the client application.</span></span> <span data-ttu-id="074ce-161">No caso de um item ter sido removido da caixa de correio do Exchange, um administrador deve usar o console de gerenciamento do Exchange para acessar a lista de remetentes bloqueados para remover um remetente da lista.</span><span class="sxs-lookup"><span data-stu-id="074ce-161">In the event that an item has been removed from the Exchange mailbox, an administrator has to use the Exchange Management Console to access the blocked sender list to remove a sender from the list.</span></span> <span data-ttu-id="074ce-162">Para obter informações sobre como desbloquear um usuário usando o console de gerenciamento do Exchange, consulte [como configurar as configurações de remetentes confiáveis e remetentes bloqueados no Office 365](https://support.microsoft.com/kb/2545137).</span><span class="sxs-lookup"><span data-stu-id="074ce-162">For information about how to unblock a user by using the Exchange Management Console, see [How to configure the safe senders and blocked senders settings in Office 365](https://support.microsoft.com/kb/2545137).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
    </soap:Header>
    <soap:Body>
      <m:MarkAsJunk IsJunk="false" MoveItem="true">
        <m:ItemIds>
          <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYu" />
        </m:ItemIds>
      </m:MarkAsJunk>
    </soap:Body>
 </soap:Envelope>

```

<span data-ttu-id="074ce-163">Uma resposta bem-sucedida para remover um remetente da lista de remetentes bloqueados é o mesmo que a resposta para adicionar um remetente à lista de remetentes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="074ce-163">A successful response for removing a sender from the blocked sender list is the same as the response for adding a sender to the blocked sender list.</span></span>
  
<span data-ttu-id="074ce-164">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="074ce-164">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="074ce-165">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="074ce-165">MarkAsJunk</span></span>](markasjunk.md)
    
- [<span data-ttu-id="074ce-166">ItemIds</span><span class="sxs-lookup"><span data-stu-id="074ce-166">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="074ce-167">ItemId</span><span class="sxs-lookup"><span data-stu-id="074ce-167">ItemId</span></span>](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a><span data-ttu-id="074ce-168">Resposta de erro de operação MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="074ce-168">MarkAsJunk operation error response</span></span>

<span data-ttu-id="074ce-169">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="074ce-169">The following example shows an error response to a **MarkAsJunk** operation request.</span></span> <span data-ttu-id="074ce-170">Esta é uma resposta a uma solicitação para adicionar ou remover um remetente da lista de remetentes bloqueados quando a mensagem de email especificada pelo identificador de item não existe mais na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="074ce-170">This is a response to a request to add or remove a sender from the blocked sender list when the email message specified by the item identifier no longer exists in the mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="545" 
                         MinorBuildNumber="11" 
                         Version="Exchange2013" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:MarkAsJunkResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:MarkAsJunkResponseMessage>
      </m:ResponseMessages>
    </m:MarkAsJunkResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="074ce-171">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="074ce-171">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="074ce-172">MarkAsJunkResponse</span><span class="sxs-lookup"><span data-stu-id="074ce-172">MarkAsJunkResponse</span></span>](markasjunkresponse.md)
    
- [<span data-ttu-id="074ce-173">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="074ce-173">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="074ce-174">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="074ce-174">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
    
- [<span data-ttu-id="074ce-175">MessageText</span><span class="sxs-lookup"><span data-stu-id="074ce-175">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="074ce-176">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="074ce-176">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="074ce-177">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="074ce-177">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="074ce-178">Também consulte</span><span class="sxs-lookup"><span data-stu-id="074ce-178">See also</span></span>

- [<span data-ttu-id="074ce-179">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="074ce-179">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- <span data-ttu-id="074ce-180">[Operação GetItem](getitem-operation.md) Operação GetItem</span><span class="sxs-lookup"><span data-stu-id="074ce-180">[GetItem operation](getitem-operation.md) GetItem operation</span></span> 
    
- [<span data-ttu-id="074ce-181">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="074ce-181">FindItem operation</span></span>](finditem-operation.md)
    

