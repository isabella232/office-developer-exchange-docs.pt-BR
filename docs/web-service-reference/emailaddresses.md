---
title: EmailAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EmailAddresses
api_type:
- schema
ms.assetid: fd4d773c-f7dc-4a04-9025-e772d7a45fdf
description: O elemento EmailAddresses representa uma coleção de endereços de email de um contato.
ms.openlocfilehash: 2eddb68ecffd8f61a2fbb775d8013433d715db1a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752003"
---
# <a name="emailaddresses"></a><span data-ttu-id="88067-103">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="88067-103">EmailAddresses</span></span>

<span data-ttu-id="88067-104">O elemento **EmailAddresses** representa uma coleção de endereços de email de um contato.</span><span class="sxs-lookup"><span data-stu-id="88067-104">The **EmailAddresses** element represents a collection of e-mail addresses for a contact.</span></span> 
  
```xml
<EmailAddresses>
   <Entry/>
</EmailAddresses>
```

 <span data-ttu-id="88067-105">**EmailAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="88067-105">**EmailAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88067-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="88067-106">Attributes and elements</span></span>

<span data-ttu-id="88067-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="88067-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88067-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="88067-108">Attributes</span></span>

<span data-ttu-id="88067-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="88067-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88067-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="88067-110">Child elements</span></span>

|<span data-ttu-id="88067-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="88067-111">**Element**</span></span>|<span data-ttu-id="88067-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="88067-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88067-113">Entrada (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="88067-113">Entry (EmailAddress)</span></span>](entry-emailaddress.md) <br/> |<span data-ttu-id="88067-114">Representa um único endereço de email de um contato.</span><span class="sxs-lookup"><span data-stu-id="88067-114">Represents a single e-mail address for a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="88067-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="88067-115">Parent elements</span></span>

|<span data-ttu-id="88067-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="88067-116">**Element**</span></span>|<span data-ttu-id="88067-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="88067-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88067-118">Contato</span><span class="sxs-lookup"><span data-stu-id="88067-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="88067-119">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="88067-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="88067-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="88067-120">Remarks</span></span>

<span data-ttu-id="88067-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="88067-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88067-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="88067-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88067-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="88067-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="88067-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="88067-124">Schema name</span></span>  <br/> |<span data-ttu-id="88067-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="88067-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="88067-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="88067-126">Validation file</span></span>  <br/> |<span data-ttu-id="88067-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="88067-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="88067-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="88067-128">Can be empty</span></span>  <br/> |<span data-ttu-id="88067-129">False</span><span class="sxs-lookup"><span data-stu-id="88067-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88067-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="88067-130">See also</span></span>

- [<span data-ttu-id="88067-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="88067-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="88067-132">Criação de contatos (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="88067-132">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [<span data-ttu-id="88067-133">Atualizar contatos</span><span class="sxs-lookup"><span data-stu-id="88067-133">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx) 
- [<span data-ttu-id="88067-134">Excluindo contatos</span><span class="sxs-lookup"><span data-stu-id="88067-134">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

