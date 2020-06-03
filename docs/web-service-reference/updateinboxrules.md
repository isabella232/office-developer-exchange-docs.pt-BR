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
description: O elemento UpdateInboxRules define uma solicitação para atualizar as regras de caixa de entrada em uma caixa de correio no repositório do servidor.
ms.openlocfilehash: d604604d582d28c07eaa75d3239082d1b6735e65
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456357"
---
# <a name="updateinboxrules"></a><span data-ttu-id="3a54b-103">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="3a54b-103">UpdateInboxRules</span></span>

<span data-ttu-id="3a54b-104">O elemento **UpdateInboxRules** define uma solicitação para atualizar as regras de caixa de entrada em uma caixa de correio no repositório do servidor.</span><span class="sxs-lookup"><span data-stu-id="3a54b-104">The **UpdateInboxRules** element defines a request to update the Inbox rules in a mailbox in the server store.</span></span> 
  
```XML
<UpdateInboxRules>
   <MailboxSmtpAddress/>
   <RemoveOutlookRuleBlob/>
   <Operations/>
</UpdateInboxRules>
```

 <span data-ttu-id="3a54b-105">**UpdateInboxRulesRequestType**</span><span class="sxs-lookup"><span data-stu-id="3a54b-105">**UpdateInboxRulesRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a54b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3a54b-106">Attributes and elements</span></span>

<span data-ttu-id="3a54b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3a54b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a54b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3a54b-108">Attributes</span></span>

<span data-ttu-id="3a54b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a54b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a54b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3a54b-110">Child elements</span></span>

|<span data-ttu-id="3a54b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3a54b-111">**Element**</span></span>|<span data-ttu-id="3a54b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3a54b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a54b-113">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="3a54b-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="3a54b-114">Representa o endereço SMTP do usuário cujas regras de caixa de entrada devem ser criadas, modificadas ou excluídas.</span><span class="sxs-lookup"><span data-stu-id="3a54b-114">Represents the SMTP address of the user whose Inbox rules are to be created, modified, or deleted.</span></span>  <br/> |
|[<span data-ttu-id="3a54b-115">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="3a54b-115">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md) <br/> |<span data-ttu-id="3a54b-116">Indica se o blob de regra do Microsoft Outlook deve ser removido.</span><span class="sxs-lookup"><span data-stu-id="3a54b-116">Indicates whether to remove the Microsoft Outlook rule blob.</span></span>  <br/> |
|[<span data-ttu-id="3a54b-117">Operations</span><span class="sxs-lookup"><span data-stu-id="3a54b-117">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="3a54b-118">Contém uma matriz de operações de regra que podem ser executadas em uma caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="3a54b-118">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3a54b-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3a54b-119">Parent elements</span></span>

<span data-ttu-id="3a54b-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a54b-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3a54b-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3a54b-121">Text value</span></span>

<span data-ttu-id="3a54b-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3a54b-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3a54b-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="3a54b-123">Remarks</span></span>

<span data-ttu-id="3a54b-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3a54b-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a54b-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3a54b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a54b-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="3a54b-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3a54b-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3a54b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="3a54b-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3a54b-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3a54b-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3a54b-129">Validation File</span></span>  <br/> |<span data-ttu-id="3a54b-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3a54b-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3a54b-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3a54b-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a54b-132">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="3a54b-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a54b-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="3a54b-133">See also</span></span>



[<span data-ttu-id="3a54b-134">Operação UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="3a54b-134">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="3a54b-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3a54b-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

