---
title: GetInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetInboxRules
api_type:
- schema
ms.assetid: 7a54992d-03a6-4afc-a2e4-dcdc9ce54194
description: O elemento de GetInboxRules define uma solicitação para obter as regras de caixa de entrada em uma caixa de correio no armazenamento do servidor.
ms.openlocfilehash: 3c3ee682dd009e5c4bec940637a7dfa3c11f8402
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752528"
---
# <a name="getinboxrules"></a><span data-ttu-id="576b1-103">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="576b1-103">GetInboxRules</span></span>

<span data-ttu-id="576b1-104">O elemento de **GetInboxRules** define uma solicitação para obter as regras de caixa de entrada em uma caixa de correio no armazenamento do servidor.</span><span class="sxs-lookup"><span data-stu-id="576b1-104">The **GetInboxRules** element defines a request to get the Inbox rules on a mailbox in the server store.</span></span> 
  
```XML
<GetInboxRules>
   <MailboxSmtpAddress/>
</GetInboxRules>
```

 <span data-ttu-id="576b1-105">**GetInboxRulesRequestType**</span><span class="sxs-lookup"><span data-stu-id="576b1-105">**GetInboxRulesRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="576b1-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="576b1-106">Attributes and elements</span></span>

<span data-ttu-id="576b1-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="576b1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="576b1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="576b1-108">Attributes</span></span>

<span data-ttu-id="576b1-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="576b1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="576b1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="576b1-110">Child elements</span></span>

|<span data-ttu-id="576b1-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="576b1-111">**Element**</span></span>|<span data-ttu-id="576b1-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="576b1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="576b1-113">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="576b1-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="576b1-114">Representa o endereço SMTP do usuário cujas regras de caixa de entrada devem ser recuperadas.</span><span class="sxs-lookup"><span data-stu-id="576b1-114">Represents the SMTP address of the user whose Inbox rules are to be retrieved.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="576b1-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="576b1-115">Parent elements</span></span>

<span data-ttu-id="576b1-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="576b1-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="576b1-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="576b1-117">Remarks</span></span>

<span data-ttu-id="576b1-118">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="576b1-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="576b1-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="576b1-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="576b1-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="576b1-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="576b1-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="576b1-121">Schema Name</span></span>  <br/> |<span data-ttu-id="576b1-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="576b1-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="576b1-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="576b1-123">Validation File</span></span>  <br/> |<span data-ttu-id="576b1-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="576b1-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="576b1-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="576b1-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="576b1-126">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="576b1-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="576b1-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="576b1-127">See also</span></span>



[<span data-ttu-id="576b1-128">Operação GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="576b1-128">GetInboxRules operation</span></span>](getinboxrules-operation.md)

