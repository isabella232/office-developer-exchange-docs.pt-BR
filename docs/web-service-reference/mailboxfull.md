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
description: O elemento MailboxFull indica se a caixa de correio do destinatário está cheio.
ms.openlocfilehash: 8e2c9e01b93af03e875834724a942cd9b17a73f3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824286"
---
# <a name="mailboxfull"></a><span data-ttu-id="3275d-103">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="3275d-103">MailboxFull</span></span>

<span data-ttu-id="3275d-104">O elemento **MailboxFull** indica se a caixa de correio do destinatário está cheio.</span><span class="sxs-lookup"><span data-stu-id="3275d-104">The **MailboxFull** element indicates whether the mailbox for the recipient is full.</span></span> 
  
```XML
<MailboxFull>true | false</MailboxFull>
```

<span data-ttu-id="3275d-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3275d-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3275d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3275d-106">Attributes and elements</span></span>

<span data-ttu-id="3275d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3275d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3275d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3275d-108">Attributes</span></span>

<span data-ttu-id="3275d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3275d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3275d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3275d-110">Child elements</span></span>

<span data-ttu-id="3275d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3275d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3275d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3275d-112">Parent elements</span></span>

|<span data-ttu-id="3275d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3275d-113">**Element**</span></span>|<span data-ttu-id="3275d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3275d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3275d-115">Dicas de email</span><span class="sxs-lookup"><span data-stu-id="3275d-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="3275d-116">Representa os valores para os vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="3275d-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3275d-117">Text value</span><span class="sxs-lookup"><span data-stu-id="3275d-117">Text value</span></span>

<span data-ttu-id="3275d-118">Esse elemento pode ser **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="3275d-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="3275d-119">Um valor **true** indica que a caixa de correio atingiu sua capacidade; um valor **false** indica que ele não atingiu sua capacidade máxima.</span><span class="sxs-lookup"><span data-stu-id="3275d-119">A value of **true** indicates that the mailbox has reached its capacity; a value of **false** indicates that it has not reached capacity.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3275d-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="3275d-120">Remarks</span></span>

<span data-ttu-id="3275d-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3275d-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3275d-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3275d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3275d-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="3275d-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3275d-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3275d-124">Schema Name</span></span>  <br/> |<span data-ttu-id="3275d-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3275d-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="3275d-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3275d-126">Validation File</span></span>  <br/> |<span data-ttu-id="3275d-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3275d-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3275d-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3275d-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="3275d-129">False</span><span class="sxs-lookup"><span data-stu-id="3275d-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3275d-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="3275d-130">See also</span></span>

- [<span data-ttu-id="3275d-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3275d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

