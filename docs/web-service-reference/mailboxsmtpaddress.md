---
title: MailboxSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxSmtpAddress
api_type:
- schema
ms.assetid: de7c9035-ebbc-4473-ac14-3b22ce62768c
description: O elemento MailboxSmtpAddress representa o endereço SMTP do usuário cujas regras de caixa de entrada devem ser recuperadas ou atualizada; ou cuja data de expiração de senha deve ser recuperado.
ms.openlocfilehash: 60b2c018f2a05e9630e92e28de1054a421b41e52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824303"
---
# <a name="mailboxsmtpaddress"></a><span data-ttu-id="15e3a-103">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="15e3a-103">MailboxSmtpAddress</span></span>

<span data-ttu-id="15e3a-104">O elemento **MailboxSmtpAddress** representa o endereço SMTP do usuário cujas regras de caixa de entrada devem ser recuperadas ou atualizada; ou cuja data de expiração de senha deve ser recuperado.</span><span class="sxs-lookup"><span data-stu-id="15e3a-104">The **MailboxSmtpAddress** element represents the SMTP address of the user whose Inbox rules are to be retrieved or updated; or whose password expiration date is to be retrieved.</span></span> 
  
```XML
<MailboxSmtpAddress/>
```

<span data-ttu-id="15e3a-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="15e3a-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="15e3a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="15e3a-106">Attributes and elements</span></span>

<span data-ttu-id="15e3a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="15e3a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15e3a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="15e3a-108">Attributes</span></span>

<span data-ttu-id="15e3a-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="15e3a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15e3a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="15e3a-110">Child elements</span></span>

<span data-ttu-id="15e3a-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="15e3a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="15e3a-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="15e3a-112">Parent elements</span></span>

|<span data-ttu-id="15e3a-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="15e3a-113">**Element**</span></span>|<span data-ttu-id="15e3a-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="15e3a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15e3a-115">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="15e3a-115">GetInboxRules</span></span>](getinboxrules.md) <br/> |<span data-ttu-id="15e3a-116">Define uma solicitação para obter as regras de caixa de entrada em uma caixa de correio no armazenamento do servidor.</span><span class="sxs-lookup"><span data-stu-id="15e3a-116">Defines a request to get the Inbox rules on a mailbox in the server store.</span></span>  <br/> |
|[<span data-ttu-id="15e3a-117">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="15e3a-117">GetPasswordExpirationDate</span></span>](getpasswordexpirationdate.md) <br/> |<span data-ttu-id="15e3a-118">Define uma solicitação para obter a data de expiração de senha de uma conta de email.</span><span class="sxs-lookup"><span data-stu-id="15e3a-118">Defines a request to get the password expiration date of an email account.</span></span>  <br/> |
|[<span data-ttu-id="15e3a-119">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="15e3a-119">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="15e3a-120">Define uma solicitação para atualizar as regras de caixa de entrada em uma caixa de correio no armazenamento do servidor.</span><span class="sxs-lookup"><span data-stu-id="15e3a-120">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="15e3a-121">Text value</span><span class="sxs-lookup"><span data-stu-id="15e3a-121">Text value</span></span>

<span data-ttu-id="15e3a-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="15e3a-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="15e3a-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="15e3a-123">Remarks</span></span>

<span data-ttu-id="15e3a-124">O **MailboxSmtpAddress** é um elemento opcional.</span><span class="sxs-lookup"><span data-stu-id="15e3a-124">The **MailboxSmtpAddress** element is an optional element.</span></span> <span data-ttu-id="15e3a-125">Se o elemento **MailboxSmtpAddress** for omitido, o endereço do usuário conectado é usado.</span><span class="sxs-lookup"><span data-stu-id="15e3a-125">If the **MailboxSmtpAddress** element is omitted, the address of the logged on user is used.</span></span> 
  
<span data-ttu-id="15e3a-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="15e3a-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15e3a-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="15e3a-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15e3a-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="15e3a-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="15e3a-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="15e3a-129">Schema Name</span></span>  <br/> |<span data-ttu-id="15e3a-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="15e3a-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="15e3a-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="15e3a-131">Validation File</span></span>  <br/> |<span data-ttu-id="15e3a-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="15e3a-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="15e3a-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="15e3a-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="15e3a-134">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="15e3a-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="15e3a-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="15e3a-135">See also</span></span>

- [<span data-ttu-id="15e3a-136">Operação GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="15e3a-136">GetInboxRules operation</span></span>](getinboxrules-operation.md)
- [<span data-ttu-id="15e3a-137">Operação GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="15e3a-137">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="15e3a-138">Operação UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="15e3a-138">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)
- [<span data-ttu-id="15e3a-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="15e3a-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

