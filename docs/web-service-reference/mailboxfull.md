---
title: MailboxFull
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxFull
api_type:
- schema
ms.assetid: 38b28c9b-9da2-4d6a-9cda-9c393986575b
description: O elemento MailboxFull indica se a caixa de correio do destinatário está cheia.
ms.openlocfilehash: f336f1eda122bb170aafb22a028e3faf84f4d782
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465972"
---
# <a name="mailboxfull"></a><span data-ttu-id="753f1-103">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="753f1-103">MailboxFull</span></span>

<span data-ttu-id="753f1-104">O elemento **MailboxFull** indica se a caixa de correio do destinatário está cheia.</span><span class="sxs-lookup"><span data-stu-id="753f1-104">The **MailboxFull** element indicates whether the mailbox for the recipient is full.</span></span> 
  
```XML
<MailboxFull>true | false</MailboxFull>
```

<span data-ttu-id="753f1-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="753f1-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="753f1-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="753f1-106">Attributes and elements</span></span>

<span data-ttu-id="753f1-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="753f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="753f1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="753f1-108">Attributes</span></span>

<span data-ttu-id="753f1-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="753f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="753f1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="753f1-110">Child elements</span></span>

<span data-ttu-id="753f1-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="753f1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="753f1-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="753f1-112">Parent elements</span></span>

|<span data-ttu-id="753f1-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="753f1-113">**Element**</span></span>|<span data-ttu-id="753f1-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="753f1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="753f1-115">Dicas de Email</span><span class="sxs-lookup"><span data-stu-id="753f1-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="753f1-116">Representa valores de vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="753f1-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="753f1-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="753f1-117">Text value</span></span>

<span data-ttu-id="753f1-118">Esse elemento pode ser **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="753f1-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="753f1-119">Um valor **true** indica que a caixa de correio atingiu sua capacidade; um valor **false** indica que não atingiu a capacidade.</span><span class="sxs-lookup"><span data-stu-id="753f1-119">A value of **true** indicates that the mailbox has reached its capacity; a value of **false** indicates that it has not reached capacity.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="753f1-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="753f1-120">Remarks</span></span>

<span data-ttu-id="753f1-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="753f1-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="753f1-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="753f1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="753f1-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="753f1-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="753f1-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="753f1-124">Schema Name</span></span>  <br/> |<span data-ttu-id="753f1-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="753f1-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="753f1-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="753f1-126">Validation File</span></span>  <br/> |<span data-ttu-id="753f1-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="753f1-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="753f1-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="753f1-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="753f1-129">False</span><span class="sxs-lookup"><span data-stu-id="753f1-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="753f1-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="753f1-130">See also</span></span>

- [<span data-ttu-id="753f1-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="753f1-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

