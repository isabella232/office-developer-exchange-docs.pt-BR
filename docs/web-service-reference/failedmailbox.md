---
title: FailedMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d4c9816-54bb-4932-b4ba-f057c9173a1a
description: O elemento FailedMailbox especifica a mensagem de erro para uma caixa de correio que falhou na pesquisa.
ms.openlocfilehash: 404084bc342eb555db61c4216e936bee6ced9c36
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461958"
---
# <a name="failedmailbox"></a><span data-ttu-id="bf24f-103">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="bf24f-103">FailedMailbox</span></span>

<span data-ttu-id="bf24f-104">O elemento **FailedMailbox** especifica a mensagem de erro para uma caixa de correio que falhou na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="bf24f-104">The **FailedMailbox** element specifies the error message for a mailbox that failed on search.</span></span> 
  
```XML
<FailedMailbox>
    <Mailbox/>
    <ErrorCode/>
    <ErrorMessage/>
    <IsArchive/>
</FailedMailbox>
```

 <span data-ttu-id="bf24f-105">**FailedSearchMailboxType**</span><span class="sxs-lookup"><span data-stu-id="bf24f-105">**FailedSearchMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bf24f-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="bf24f-106">Attributes and elements</span></span>

<span data-ttu-id="bf24f-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bf24f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bf24f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="bf24f-108">Attributes</span></span>

<span data-ttu-id="bf24f-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bf24f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bf24f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bf24f-110">Child elements</span></span>

|<span data-ttu-id="bf24f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bf24f-111">**Element**</span></span>|<span data-ttu-id="bf24f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bf24f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf24f-113">Caixa de correio (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="bf24f-113">Mailbox (string)</span></span>](mailbox-string.md) <br/> |<span data-ttu-id="bf24f-114">Contém um identificador para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="bf24f-114">Contains an identifier for the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="bf24f-115">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="bf24f-115">ErrorCode (int)</span></span>](errorcode-int.md) <br/> |<span data-ttu-id="bf24f-116">Especifica o código de erro da caixa de correio que falhou na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="bf24f-116">Specifies the error code of the mailbox that failed the search.</span></span>  <br/> |
|[<span data-ttu-id="bf24f-117">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="bf24f-117">ErrorMessage</span></span>](errormessage.md) <br/> |<span data-ttu-id="bf24f-118">Representa o motivo do erro de validação.</span><span class="sxs-lookup"><span data-stu-id="bf24f-118">Represents the reason for the validation error.</span></span>  <br/> |
|[<span data-ttu-id="bf24f-119">IsArchive</span><span class="sxs-lookup"><span data-stu-id="bf24f-119">IsArchive</span></span>](isarchive.md) <br/> |<span data-ttu-id="bf24f-120">Especifica um valor Boolean que indica se a caixa de correio é um arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="bf24f-120">Specifies a Boolean value that indicates whether the mailbox is an archive.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bf24f-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bf24f-121">Parent elements</span></span>

|<span data-ttu-id="bf24f-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bf24f-122">**Element**</span></span>|<span data-ttu-id="bf24f-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bf24f-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf24f-124">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="bf24f-124">FailedMailboxes</span></span>](failedmailboxes.md) <br/> |<span data-ttu-id="bf24f-125">Especifica uma matriz de caixas de correio com falha.</span><span class="sxs-lookup"><span data-stu-id="bf24f-125">Specifies an array of failed mailboxes.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bf24f-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="bf24f-126">Remarks</span></span>

<span data-ttu-id="bf24f-127">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bf24f-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bf24f-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf24f-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bf24f-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="bf24f-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bf24f-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="bf24f-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bf24f-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bf24f-131">Schema Name</span></span>  <br/> |<span data-ttu-id="bf24f-132">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="bf24f-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="bf24f-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bf24f-133">Validation File</span></span>  <br/> |<span data-ttu-id="bf24f-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bf24f-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="bf24f-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="bf24f-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="bf24f-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="bf24f-136">See also</span></span>



- [<span data-ttu-id="bf24f-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bf24f-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

