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
description: O elemento de DeliverMeetingRequests define como as solicitações de reunião são manipuladas entre o delegado e a entidade. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 803bd2da72bdb21b507a59cc11635a40d4431acf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751773"
---
# <a name="delivermeetingrequests"></a><span data-ttu-id="93c7b-104">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="93c7b-104">DeliverMeetingRequests</span></span>

<span data-ttu-id="93c7b-105">O elemento de **DeliverMeetingRequests** define como as solicitações de reunião são manipuladas entre o delegado e a entidade.</span><span class="sxs-lookup"><span data-stu-id="93c7b-105">The **DeliverMeetingRequests** element defines how meeting requests are handled between the delegate and the principal.</span></span> <span data-ttu-id="93c7b-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="93c7b-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```XML
<DeliverMeetingRequests>DelegatesOnly or DelegatesAndMe or DelegatesAndSendInformationToMe or NoForward</DeliverMeetingRequests>
```

 <span data-ttu-id="93c7b-107">**DeliverMeetingRequestsType**</span><span class="sxs-lookup"><span data-stu-id="93c7b-107">**DeliverMeetingRequestsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93c7b-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="93c7b-108">Attributes and elements</span></span>

<span data-ttu-id="93c7b-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="93c7b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93c7b-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="93c7b-110">Attributes</span></span>

<span data-ttu-id="93c7b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="93c7b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93c7b-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="93c7b-112">Child elements</span></span>

<span data-ttu-id="93c7b-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="93c7b-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="93c7b-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="93c7b-114">Parent elements</span></span>

|<span data-ttu-id="93c7b-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="93c7b-115">**Element**</span></span>|<span data-ttu-id="93c7b-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="93c7b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93c7b-117">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="93c7b-117">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="93c7b-118">Define uma solicitação para adicionar representantes para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="93c7b-118">Defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="93c7b-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="93c7b-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="93c7b-120">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="93c7b-120">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="93c7b-121">Define uma solicitação de atualização de representantes em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="93c7b-121">Defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="93c7b-122">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="93c7b-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="93c7b-123">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="93c7b-123">GetDelegateResponse</span></span>](getdelegateresponse.md) <br/> |<span data-ttu-id="93c7b-124">Contém o status e o resultado de uma solicitação de GetDelegate.</span><span class="sxs-lookup"><span data-stu-id="93c7b-124">Contains the status and result of a GetDelegate request.</span></span> <span data-ttu-id="93c7b-125">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="93c7b-125">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="93c7b-126">Text value</span><span class="sxs-lookup"><span data-stu-id="93c7b-126">Text value</span></span>

<span data-ttu-id="93c7b-127">A tabela a seguir lista os valores possíveis para o elemento **DeliverMeetingRequests** .</span><span class="sxs-lookup"><span data-stu-id="93c7b-127">The following table lists the possible values for the **DeliverMeetingRequests** element.</span></span> 
  
<span data-ttu-id="93c7b-128">**Valores de elemento DeliverMeetingRequests**</span><span class="sxs-lookup"><span data-stu-id="93c7b-128">**DeliverMeetingRequests element values**</span></span>

|<span data-ttu-id="93c7b-129">**Valor**</span><span class="sxs-lookup"><span data-stu-id="93c7b-129">**Value**</span></span>|<span data-ttu-id="93c7b-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="93c7b-130">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="93c7b-131">DelegatesOnly</span><span class="sxs-lookup"><span data-stu-id="93c7b-131">DelegatesOnly</span></span>  <br/> |<span data-ttu-id="93c7b-132">Solicitações de reunião são encaminhadas para o representante e movidas para a pasta Itens excluídos na caixa de correio do principal.</span><span class="sxs-lookup"><span data-stu-id="93c7b-132">Meeting requests are forwarded to the delegate and moved to the Deleted Items folder in the principal's mailbox.</span></span>  <br/> |
|<span data-ttu-id="93c7b-133">DelegatesAndMe</span><span class="sxs-lookup"><span data-stu-id="93c7b-133">DelegatesAndMe</span></span>  <br/> |<span data-ttu-id="93c7b-134">Solicitações de reunião são encaminhadas para o representante e permanecem na pasta caixa de entrada na caixa de correio do principal.</span><span class="sxs-lookup"><span data-stu-id="93c7b-134">Meeting requests are forwarded to the delegate and remain in the Inbox folder in the principal's mailbox.</span></span>  <br/> |
|<span data-ttu-id="93c7b-135">DelegatesAndSendInformationToMe</span><span class="sxs-lookup"><span data-stu-id="93c7b-135">DelegatesAndSendInformationToMe</span></span>  <br/> |<span data-ttu-id="93c7b-136">Solicitações de reunião são encaminhadas para o representante e permanecem na pasta caixa de entrada na caixa de correio da entidade de segurança, mas os botões de aceitar, recusar e provisório não aparecem no painel de leitura do Microsoft Office Outlook.</span><span class="sxs-lookup"><span data-stu-id="93c7b-136">Meeting requests are forwarded to the delegate and remain in the Inbox folder in the principal's mailbox, but the Accept, Tentative, and Decline buttons do not appear in the Microsoft Office Outlook reading pane.</span></span>  <br/> |
|<span data-ttu-id="93c7b-137">NoForward</span><span class="sxs-lookup"><span data-stu-id="93c7b-137">NoForward</span></span>  <br/> |<span data-ttu-id="93c7b-138">Solicitações de reunião não são encaminhadas para o representante.</span><span class="sxs-lookup"><span data-stu-id="93c7b-138">Meeting requests are not forwarded to the delegate.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="93c7b-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="93c7b-139">Remarks</span></span>

<span data-ttu-id="93c7b-140">A configuração de **DeliverMeetingRequests** afeta todos os delegados na caixa de correio da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="93c7b-140">The **DeliverMeetingRequests** setting affects all delegates in a principal's mailbox.</span></span> 
  
<span data-ttu-id="93c7b-141">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="93c7b-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93c7b-142">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="93c7b-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93c7b-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="93c7b-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="93c7b-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="93c7b-144">Schema Name</span></span>  <br/> |<span data-ttu-id="93c7b-145">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="93c7b-145">Messages schema</span></span>  <br/> |
|<span data-ttu-id="93c7b-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="93c7b-146">Validation File</span></span>  <br/> |<span data-ttu-id="93c7b-147">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="93c7b-147">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="93c7b-148">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="93c7b-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="93c7b-149">False</span><span class="sxs-lookup"><span data-stu-id="93c7b-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93c7b-150">Ver também</span><span class="sxs-lookup"><span data-stu-id="93c7b-150">See also</span></span>

- [<span data-ttu-id="93c7b-151">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="93c7b-151">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="93c7b-152">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="93c7b-152">UpdateDelegate operation</span></span>](updatedelegate-operation.md)  
- [<span data-ttu-id="93c7b-153">Operação GetDelegate</span><span class="sxs-lookup"><span data-stu-id="93c7b-153">GetDelegate operation</span></span>](getdelegate-operation.md)
- [<span data-ttu-id="93c7b-154">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="93c7b-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="93c7b-155">Adicionando representantes</span><span class="sxs-lookup"><span data-stu-id="93c7b-155">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

