---
title: GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f4f958ed-9cf4-4ebf-9b01-e2df9a7cbd63
description: O elemento de GetPasswordExpirationDate define uma solicitação para obter a data de expiração de senha para uma conta de email. Este elemento é a base para a operação de operação GetPasswordExpirationDate.
ms.openlocfilehash: a9e0955566372f7b99c48c56e62ce2c5025f9f95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752587"
---
# <a name="getpasswordexpirationdate"></a><span data-ttu-id="a25a8-104">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="a25a8-104">GetPasswordExpirationDate</span></span>

<span data-ttu-id="a25a8-105">O elemento de **GetPasswordExpirationDate** define uma solicitação para obter a data de expiração de senha para uma conta de email.</span><span class="sxs-lookup"><span data-stu-id="a25a8-105">The **GetPasswordExpirationDate** element defines a request to get the password expiration date for an email account.</span></span> <span data-ttu-id="a25a8-106">Este elemento é a base para a operação [GetPasswordExpirationDate operação](getpasswordexpirationdate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a25a8-106">This element is the base element for the [GetPasswordExpirationDate operation](getpasswordexpirationdate-operation.md) operation.</span></span> 
  
```XML
<GetPasswordExpirationDate>
    <MailboxSmtpAddress/>
</GetPasswordExpirationDate>
```

 <span data-ttu-id="a25a8-107">**GetPasswordExpirationDateType**</span><span class="sxs-lookup"><span data-stu-id="a25a8-107">**GetPasswordExpirationDateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a25a8-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a25a8-108">Attributes and elements</span></span>

<span data-ttu-id="a25a8-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a25a8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a25a8-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="a25a8-110">Attributes</span></span>

<span data-ttu-id="a25a8-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a25a8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a25a8-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a25a8-112">Child elements</span></span>

|<span data-ttu-id="a25a8-113">**Nome do elemento**</span><span class="sxs-lookup"><span data-stu-id="a25a8-113">**Element name**</span></span>|<span data-ttu-id="a25a8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a25a8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a25a8-115">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="a25a8-115">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="a25a8-116">Representa o endereço de email da conta de email para o qual a data de expiração de senha é a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="a25a8-116">Represents the email address of the email account for which the password expiration date is to be returned.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a25a8-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a25a8-117">Parent elements</span></span>

<span data-ttu-id="a25a8-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a25a8-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a25a8-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="a25a8-119">Remarks</span></span>

<span data-ttu-id="a25a8-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a25a8-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="a25a8-121">Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="a25a8-121">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a25a8-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a25a8-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a25a8-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="a25a8-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a25a8-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a25a8-124">Schema Name</span></span>  <br/> |<span data-ttu-id="a25a8-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a25a8-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a25a8-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a25a8-126">Validation File</span></span>  <br/> |<span data-ttu-id="a25a8-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a25a8-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a25a8-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a25a8-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="a25a8-129">False</span><span class="sxs-lookup"><span data-stu-id="a25a8-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a25a8-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="a25a8-130">See also</span></span>



[<span data-ttu-id="a25a8-131">Operação GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="a25a8-131">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)


- [<span data-ttu-id="a25a8-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a25a8-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

