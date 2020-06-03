---
title: DeliverMeetingRequests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliverMeetingRequests
api_type:
- schema
ms.assetid: 04b999af-0b27-4e6d-a8b1-400955a1afaa
description: O elemento DeliverMeetingRequests define como as solicitações de reunião são tratadas entre o representante e a entidade de segurança. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 3998443613437bca2267678f7bc2c5584b779135
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463675"
---
# <a name="delivermeetingrequests"></a><span data-ttu-id="6fdc0-104">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="6fdc0-104">DeliverMeetingRequests</span></span>

<span data-ttu-id="6fdc0-105">O elemento **DeliverMeetingRequests** define como as solicitações de reunião são tratadas entre o representante e a entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="6fdc0-105">The **DeliverMeetingRequests** element defines how meeting requests are handled between the delegate and the principal.</span></span> <span data-ttu-id="6fdc0-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6fdc0-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```XML
<DeliverMeetingRequests>DelegatesOnly or DelegatesAndMe or DelegatesAndSendInformationToMe or NoForward</DeliverMeetingRequests>
```

 <span data-ttu-id="6fdc0-107">**DeliverMeetingRequestsType**</span><span class="sxs-lookup"><span data-stu-id="6fdc0-107">**DeliverMeetingRequestsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6fdc0-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6fdc0-108">Attributes and elements</span></span>

<span data-ttu-id="6fdc0-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6fdc0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6fdc0-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="6fdc0-110">Attributes</span></span>

<span data-ttu-id="6fdc0-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6fdc0-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6fdc0-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6fdc0-112">Child elements</span></span>

<span data-ttu-id="6fdc0-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6fdc0-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6fdc0-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6fdc0-114">Parent elements</span></span>

|<span data-ttu-id="6fdc0-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6fdc0-115">**Element**</span></span>|<span data-ttu-id="6fdc0-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6fdc0-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6fdc0-117">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="6fdc0-117">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="6fdc0-118">Define uma solicitação para adicionar representantes a uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6fdc0-118">Defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="6fdc0-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="6fdc0-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6fdc0-120">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="6fdc0-120">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="6fdc0-121">Define uma solicitação para atualizar representantes em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6fdc0-121">Defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="6fdc0-122">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="6fdc0-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6fdc0-123">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="6fdc0-123">GetDelegateResponse</span></span>](getdelegateresponse.md) <br/> |<span data-ttu-id="6fdc0-124">Contém o status e o resultado de uma solicitação getdelegate.</span><span class="sxs-lookup"><span data-stu-id="6fdc0-124">Contains the status and result of a GetDelegate request.</span></span> <span data-ttu-id="6fdc0-125">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="6fdc0-125">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6fdc0-126">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="6fdc0-126">Text value</span></span>

<span data-ttu-id="6fdc0-127">A tabela a seguir lista os valores possíveis para o elemento **DeliverMeetingRequests** .</span><span class="sxs-lookup"><span data-stu-id="6fdc0-127">The following table lists the possible values for the **DeliverMeetingRequests** element.</span></span> 
  
<span data-ttu-id="6fdc0-128">**Valores do elemento DeliverMeetingRequests**</span><span class="sxs-lookup"><span data-stu-id="6fdc0-128">**DeliverMeetingRequests element values**</span></span>

|<span data-ttu-id="6fdc0-129">**Valor**</span><span class="sxs-lookup"><span data-stu-id="6fdc0-129">**Value**</span></span>|<span data-ttu-id="6fdc0-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6fdc0-130">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6fdc0-131">DelegatesOnly</span><span class="sxs-lookup"><span data-stu-id="6fdc0-131">DelegatesOnly</span></span>  <br/> |<span data-ttu-id="6fdc0-132">As solicitações de reunião são encaminhadas para o representante e movidas para a pasta itens excluídos na caixa de correio da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="6fdc0-132">Meeting requests are forwarded to the delegate and moved to the Deleted Items folder in the principal's mailbox.</span></span>  <br/> |
|<span data-ttu-id="6fdc0-133">DelegatesAndMe</span><span class="sxs-lookup"><span data-stu-id="6fdc0-133">DelegatesAndMe</span></span>  <br/> |<span data-ttu-id="6fdc0-134">As solicitações de reunião são encaminhadas para o representante e permanecem na pasta caixa de entrada na caixa de correio da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="6fdc0-134">Meeting requests are forwarded to the delegate and remain in the Inbox folder in the principal's mailbox.</span></span>  <br/> |
|<span data-ttu-id="6fdc0-135">DelegatesAndSendInformationToMe</span><span class="sxs-lookup"><span data-stu-id="6fdc0-135">DelegatesAndSendInformationToMe</span></span>  <br/> |<span data-ttu-id="6fdc0-136">As solicitações de reunião são encaminhadas para o representante e permanecem na pasta caixa de entrada na caixa de correio da entidade de segurança, mas os botões aceitar, provisório e recusar não aparecem no painel de leitura do Microsoft Office Outlook.</span><span class="sxs-lookup"><span data-stu-id="6fdc0-136">Meeting requests are forwarded to the delegate and remain in the Inbox folder in the principal's mailbox, but the Accept, Tentative, and Decline buttons do not appear in the Microsoft Office Outlook reading pane.</span></span>  <br/> |
|<span data-ttu-id="6fdc0-137">Noforward</span><span class="sxs-lookup"><span data-stu-id="6fdc0-137">NoForward</span></span>  <br/> |<span data-ttu-id="6fdc0-138">As solicitações de reunião não são encaminhadas para o representante.</span><span class="sxs-lookup"><span data-stu-id="6fdc0-138">Meeting requests are not forwarded to the delegate.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6fdc0-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="6fdc0-139">Remarks</span></span>

<span data-ttu-id="6fdc0-140">A configuração **DeliverMeetingRequests** afeta todos os representantes da caixa de correio de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="6fdc0-140">The **DeliverMeetingRequests** setting affects all delegates in a principal's mailbox.</span></span> 
  
<span data-ttu-id="6fdc0-141">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6fdc0-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6fdc0-142">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6fdc0-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6fdc0-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="6fdc0-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6fdc0-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6fdc0-144">Schema Name</span></span>  <br/> |<span data-ttu-id="6fdc0-145">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6fdc0-145">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6fdc0-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6fdc0-146">Validation File</span></span>  <br/> |<span data-ttu-id="6fdc0-147">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6fdc0-147">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6fdc0-148">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6fdc0-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="6fdc0-149">False</span><span class="sxs-lookup"><span data-stu-id="6fdc0-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6fdc0-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="6fdc0-150">See also</span></span>

- [<span data-ttu-id="6fdc0-151">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="6fdc0-151">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="6fdc0-152">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="6fdc0-152">UpdateDelegate operation</span></span>](updatedelegate-operation.md)  
- [<span data-ttu-id="6fdc0-153">Operação getdelegate</span><span class="sxs-lookup"><span data-stu-id="6fdc0-153">GetDelegate operation</span></span>](getdelegate-operation.md)
- [<span data-ttu-id="6fdc0-154">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6fdc0-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="6fdc0-155">Adicionar representantes</span><span class="sxs-lookup"><span data-stu-id="6fdc0-155">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

