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
description: O elemento MailboxSmtpAddress representa o endereço SMTP do usuário cujas regras de caixa de entrada devem ser recuperadas ou atualizadas; ou cuja data de expiração de senha deve ser recuperada.
ms.openlocfilehash: 613e8098210257280bec47f2b22a2d29d04fa07c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530541"
---
# <a name="mailboxsmtpaddress"></a><span data-ttu-id="efcad-103">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="efcad-103">MailboxSmtpAddress</span></span>

<span data-ttu-id="efcad-104">O elemento **MailboxSmtpAddress** representa o endereço SMTP do usuário cujas regras de caixa de entrada devem ser recuperadas ou atualizadas; ou cuja data de expiração de senha deve ser recuperada.</span><span class="sxs-lookup"><span data-stu-id="efcad-104">The **MailboxSmtpAddress** element represents the SMTP address of the user whose Inbox rules are to be retrieved or updated; or whose password expiration date is to be retrieved.</span></span> 
  
```XML
<MailboxSmtpAddress/>
```

<span data-ttu-id="efcad-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="efcad-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="efcad-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="efcad-106">Attributes and elements</span></span>

<span data-ttu-id="efcad-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="efcad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="efcad-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="efcad-108">Attributes</span></span>

<span data-ttu-id="efcad-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="efcad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="efcad-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="efcad-110">Child elements</span></span>

<span data-ttu-id="efcad-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="efcad-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="efcad-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="efcad-112">Parent elements</span></span>

|<span data-ttu-id="efcad-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="efcad-113">**Element**</span></span>|<span data-ttu-id="efcad-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="efcad-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="efcad-115">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="efcad-115">GetInboxRules</span></span>](getinboxrules.md) <br/> |<span data-ttu-id="efcad-116">Define uma solicitação para obter as regras de caixa de entrada em uma caixa de correio no repositório do servidor.</span><span class="sxs-lookup"><span data-stu-id="efcad-116">Defines a request to get the Inbox rules on a mailbox in the server store.</span></span>  <br/> |
|[<span data-ttu-id="efcad-117">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="efcad-117">GetPasswordExpirationDate</span></span>](getpasswordexpirationdate.md) <br/> |<span data-ttu-id="efcad-118">Define uma solicitação para obter a data de expiração da senha de uma conta de email.</span><span class="sxs-lookup"><span data-stu-id="efcad-118">Defines a request to get the password expiration date of an email account.</span></span>  <br/> |
|[<span data-ttu-id="efcad-119">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="efcad-119">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="efcad-120">Define uma solicitação para atualizar as regras de caixa de entrada em uma caixa de correio no repositório do servidor.</span><span class="sxs-lookup"><span data-stu-id="efcad-120">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="efcad-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="efcad-121">Text value</span></span>

<span data-ttu-id="efcad-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="efcad-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="efcad-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="efcad-123">Remarks</span></span>

<span data-ttu-id="efcad-124">O elemento **MailboxSmtpAddress** é um elemento opcional.</span><span class="sxs-lookup"><span data-stu-id="efcad-124">The **MailboxSmtpAddress** element is an optional element.</span></span> <span data-ttu-id="efcad-125">Se o elemento **MailboxSmtpAddress** for omitido, o endereço do usuário conectado será usado.</span><span class="sxs-lookup"><span data-stu-id="efcad-125">If the **MailboxSmtpAddress** element is omitted, the address of the logged on user is used.</span></span> 
  
<span data-ttu-id="efcad-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="efcad-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="efcad-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="efcad-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="efcad-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="efcad-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="efcad-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="efcad-129">Schema Name</span></span>  <br/> |<span data-ttu-id="efcad-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="efcad-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="efcad-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="efcad-131">Validation File</span></span>  <br/> |<span data-ttu-id="efcad-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="efcad-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="efcad-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="efcad-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="efcad-134">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="efcad-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="efcad-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="efcad-135">See also</span></span>

- [<span data-ttu-id="efcad-136">Operação GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="efcad-136">GetInboxRules operation</span></span>](getinboxrules-operation.md)
- [<span data-ttu-id="efcad-137">Operação GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="efcad-137">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="efcad-138">Operação UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="efcad-138">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)
- [<span data-ttu-id="efcad-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="efcad-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

