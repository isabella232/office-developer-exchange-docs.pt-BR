---
title: GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f4f958ed-9cf4-4ebf-9b01-e2df9a7cbd63
description: O elemento GetPasswordExpirationDate define uma solicitação para obter a data de expiração da senha de uma conta de email. Este elemento é o elemento base para a operação de operação GetPasswordExpirationDate.
ms.openlocfilehash: ececbf51f71c7d87705d727229fce2314d922efb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456490"
---
# <a name="getpasswordexpirationdate"></a><span data-ttu-id="1958f-104">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="1958f-104">GetPasswordExpirationDate</span></span>

<span data-ttu-id="1958f-105">O elemento **GetPasswordExpirationDate** define uma solicitação para obter a data de expiração da senha de uma conta de email.</span><span class="sxs-lookup"><span data-stu-id="1958f-105">The **GetPasswordExpirationDate** element defines a request to get the password expiration date for an email account.</span></span> <span data-ttu-id="1958f-106">Este elemento é o elemento base para a operação de [operação GetPasswordExpirationDate](getpasswordexpirationdate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1958f-106">This element is the base element for the [GetPasswordExpirationDate operation](getpasswordexpirationdate-operation.md) operation.</span></span> 
  
```XML
<GetPasswordExpirationDate>
    <MailboxSmtpAddress/>
</GetPasswordExpirationDate>
```

 <span data-ttu-id="1958f-107">**GetPasswordExpirationDateType**</span><span class="sxs-lookup"><span data-stu-id="1958f-107">**GetPasswordExpirationDateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1958f-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1958f-108">Attributes and elements</span></span>

<span data-ttu-id="1958f-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1958f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1958f-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="1958f-110">Attributes</span></span>

<span data-ttu-id="1958f-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1958f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1958f-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1958f-112">Child elements</span></span>

|<span data-ttu-id="1958f-113">**Nome do elemento**</span><span class="sxs-lookup"><span data-stu-id="1958f-113">**Element name**</span></span>|<span data-ttu-id="1958f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1958f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1958f-115">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="1958f-115">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="1958f-116">Representa o endereço de email da conta de email para a qual a data de vencimento da senha deve ser retornada.</span><span class="sxs-lookup"><span data-stu-id="1958f-116">Represents the email address of the email account for which the password expiration date is to be returned.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1958f-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1958f-117">Parent elements</span></span>

<span data-ttu-id="1958f-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1958f-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1958f-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="1958f-119">Remarks</span></span>

<span data-ttu-id="1958f-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1958f-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="1958f-121">Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="1958f-121">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1958f-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1958f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1958f-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="1958f-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1958f-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1958f-124">Schema Name</span></span>  <br/> |<span data-ttu-id="1958f-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="1958f-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1958f-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1958f-126">Validation File</span></span>  <br/> |<span data-ttu-id="1958f-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1958f-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1958f-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1958f-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="1958f-129">False</span><span class="sxs-lookup"><span data-stu-id="1958f-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1958f-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="1958f-130">See also</span></span>



[<span data-ttu-id="1958f-131">Operação GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="1958f-131">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)


- [<span data-ttu-id="1958f-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1958f-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

