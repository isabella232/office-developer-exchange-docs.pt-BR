---
title: UpdateInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: d220064f-ff4d-4537-8077-adf94f2cbdbd
description: O elemento de UpdateInboxRules define uma solicitação para atualizar as regras de caixa de entrada em uma caixa de correio no armazenamento do servidor.
ms.openlocfilehash: 73af3efcbf4320604576b724acf18530b8b86b26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837902"
---
# <a name="updateinboxrules"></a><span data-ttu-id="050ea-103">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="050ea-103">UpdateInboxRules</span></span>

<span data-ttu-id="050ea-104">O elemento de **UpdateInboxRules** define uma solicitação para atualizar as regras de caixa de entrada em uma caixa de correio no armazenamento do servidor.</span><span class="sxs-lookup"><span data-stu-id="050ea-104">The **UpdateInboxRules** element defines a request to update the Inbox rules in a mailbox in the server store.</span></span> 
  
```XML
<UpdateInboxRules>
   <MailboxSmtpAddress/>
   <RemoveOutlookRuleBlob/>
   <Operations/>
</UpdateInboxRules>
```

 <span data-ttu-id="050ea-105">**UpdateInboxRulesRequestType**</span><span class="sxs-lookup"><span data-stu-id="050ea-105">**UpdateInboxRulesRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="050ea-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="050ea-106">Attributes and elements</span></span>

<span data-ttu-id="050ea-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="050ea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="050ea-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="050ea-108">Attributes</span></span>

<span data-ttu-id="050ea-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="050ea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="050ea-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="050ea-110">Child elements</span></span>

|<span data-ttu-id="050ea-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="050ea-111">**Element**</span></span>|<span data-ttu-id="050ea-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="050ea-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="050ea-113">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="050ea-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="050ea-114">Representa o endereço SMTP do usuário cujas regras de caixa de entrada devem ser criados, modificados ou excluídos.</span><span class="sxs-lookup"><span data-stu-id="050ea-114">Represents the SMTP address of the user whose Inbox rules are to be created, modified, or deleted.</span></span>  <br/> |
|[<span data-ttu-id="050ea-115">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="050ea-115">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md) <br/> |<span data-ttu-id="050ea-116">Indica se deseja remover o blob de regra do Microsoft Outlook.</span><span class="sxs-lookup"><span data-stu-id="050ea-116">Indicates whether to remove the Microsoft Outlook rule blob.</span></span>  <br/> |
|[<span data-ttu-id="050ea-117">Operations</span><span class="sxs-lookup"><span data-stu-id="050ea-117">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="050ea-118">Contém uma matriz das operações de regra que podem ser executadas em uma caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="050ea-118">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="050ea-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="050ea-119">Parent elements</span></span>

<span data-ttu-id="050ea-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="050ea-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="050ea-121">Text value</span><span class="sxs-lookup"><span data-stu-id="050ea-121">Text value</span></span>

<span data-ttu-id="050ea-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="050ea-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="050ea-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="050ea-123">Remarks</span></span>

<span data-ttu-id="050ea-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="050ea-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="050ea-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="050ea-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="050ea-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="050ea-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="050ea-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="050ea-127">Schema Name</span></span>  <br/> |<span data-ttu-id="050ea-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="050ea-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="050ea-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="050ea-129">Validation File</span></span>  <br/> |<span data-ttu-id="050ea-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="050ea-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="050ea-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="050ea-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="050ea-132">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="050ea-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="050ea-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="050ea-133">See also</span></span>



[<span data-ttu-id="050ea-134">Operação UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="050ea-134">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="050ea-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="050ea-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

