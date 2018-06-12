---
title: PrimarySmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PrimarySmtpAddress
api_type:
- schema
ms.assetid: eee79904-9412-4e61-b9b8-aff0ce25fade
description: O elemento PrimarySmtpAddress representa o endereço de Simple Mail Transfer Protocol (SMTP) principal de uma conta a ser usada para autorização de servidor-para-servidor ou acesso de representante.
ms.openlocfilehash: d33bf22af4ddf6b2f6d8d8d434168264acfaea7c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824881"
---
# <a name="primarysmtpaddress"></a><span data-ttu-id="4800f-103">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="4800f-103">PrimarySmtpAddress</span></span>

<span data-ttu-id="4800f-104">O elemento **PrimarySmtpAddress** representa o endereço de Simple Mail Transfer Protocol (SMTP) principal de uma conta a ser usada para autorização de servidor-para-servidor ou acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="4800f-104">The **PrimarySmtpAddress** element represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for server-to-server authorization or delegate access.</span></span> 
  
```xml
<PrimarySmtpAddress/>
```

 <span data-ttu-id="4800f-105">**PrimarySmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="4800f-105">**PrimarySmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4800f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4800f-106">Attributes and elements</span></span>

<span data-ttu-id="4800f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4800f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4800f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4800f-108">Attributes</span></span>

<span data-ttu-id="4800f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4800f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4800f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4800f-110">Child elements</span></span>

<span data-ttu-id="4800f-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4800f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4800f-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4800f-112">Parent elements</span></span>

|<span data-ttu-id="4800f-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4800f-113">**Element**</span></span>|<span data-ttu-id="4800f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4800f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4800f-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="4800f-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="4800f-116">Representa uma conta para representar quando você estiver usando o cabeçalho SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="4800f-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="4800f-117">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="4800f-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="4800f-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="4800f-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="4800f-119">Usado no cabeçalho SOAP para serialização de token de autenticação de servidor-para-servidor.</span><span class="sxs-lookup"><span data-stu-id="4800f-119">Used in the SOAP header for token serialization in server- to-server authentication.</span></span>  <br/> |
|[<span data-ttu-id="4800f-120">UserId</span><span class="sxs-lookup"><span data-stu-id="4800f-120">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="4800f-121">Identifica um usuário delegado ou um usuário que tem permissões de acesso de pasta.</span><span class="sxs-lookup"><span data-stu-id="4800f-121">Identifies a delegate user or a user who has folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4800f-122">Text value</span><span class="sxs-lookup"><span data-stu-id="4800f-122">Text value</span></span>

<span data-ttu-id="4800f-123">É necessário um valor de texto que representa um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="4800f-123">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4800f-124">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="4800f-124">Remarks</span></span>

<span data-ttu-id="4800f-125">Serviços Web do Exchange requer que as caixas de correio ser identificado pelo endereço SMTP principal da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4800f-125">Exchange Web Services requires that mailboxes be identified by the primary SMTP address of the mailbox.</span></span> <span data-ttu-id="4800f-126">Proxy ou endereços alternativos não são aceitas.</span><span class="sxs-lookup"><span data-stu-id="4800f-126">Proxy or alternative addresses are not accepted.</span></span>
  
<span data-ttu-id="4800f-127">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="4800f-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4800f-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4800f-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4800f-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="4800f-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4800f-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4800f-130">Schema Name</span></span>  <br/> |<span data-ttu-id="4800f-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4800f-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="4800f-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4800f-132">Validation File</span></span>  <br/> |<span data-ttu-id="4800f-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4800f-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4800f-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4800f-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="4800f-135">False</span><span class="sxs-lookup"><span data-stu-id="4800f-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4800f-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="4800f-136">See also</span></span>



- [<span data-ttu-id="4800f-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4800f-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="4800f-138">Autorização de servidor-para-servidor no EWS</span><span class="sxs-lookup"><span data-stu-id="4800f-138">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)
  
[<span data-ttu-id="4800f-139">Trabalhando com acesso de representante</span><span class="sxs-lookup"><span data-stu-id="4800f-139">Working with Delegate Access</span></span>](http://msdn.microsoft.com/library/dfd6b4a3-8fd3-47ba-83c0-52465cb5f3f3%28Office.15%29.aspx)

