---
title: SmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SmtpAddress
api_type:
- schema
ms.assetid: 779305a6-ad1e-424e-8a69-4e3bef61d787
description: O elemento SmtpAddress representa o endereço de Simple Mail Transfer Protocol (SMTP) de uma conta a ser usada para representação ou um endereço de destinatário de Simple Mail Transfer Protocol (SMTP) de um calendário ou uma solicitação de compartilhamento do contato.
ms.openlocfilehash: 39588f0892cdcec819a1972547155730be5785f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825511"
---
# <a name="smtpaddress"></a><span data-ttu-id="b0501-103">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="b0501-103">SmtpAddress</span></span>

<span data-ttu-id="b0501-104">O elemento **SmtpAddress** representa o endereço de Simple Mail Transfer Protocol (SMTP) de uma conta a ser usada para representação ou um endereço de destinatário de Simple Mail Transfer Protocol (SMTP) de um calendário ou uma solicitação de compartilhamento do contato.</span><span class="sxs-lookup"><span data-stu-id="b0501-104">The **SmtpAddress** element represents the Simple Mail Transfer Protocol (SMTP) address of an account to be used for impersonation or a Simple Mail Transfer Protocol (SMTP) recipient address of a calendar or contact sharing request.</span></span> 
  
```xml
<SmtpAddress/>
```

<span data-ttu-id="b0501-105">**SmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="b0501-105">**SmtpAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b0501-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b0501-106">Attributes and elements</span></span>

<span data-ttu-id="b0501-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b0501-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0501-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b0501-108">Attributes</span></span>

<span data-ttu-id="b0501-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b0501-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0501-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b0501-110">Child elements</span></span>

<span data-ttu-id="b0501-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b0501-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b0501-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b0501-112">Parent elements</span></span>

|<span data-ttu-id="b0501-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b0501-113">**Element**</span></span>|<span data-ttu-id="b0501-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b0501-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0501-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="b0501-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="b0501-116">Representa uma conta para representar quando você estiver usando o cabeçalho SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="b0501-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="b0501-117">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="b0501-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="b0501-118">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="b0501-118">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="b0501-119">Representa um destinatário inválido para um compartilhamento de calendário ou mensagem de compartilhamento do contato.</span><span class="sxs-lookup"><span data-stu-id="b0501-119">Represents an invalid recipient for a calendar sharing or contact sharing message.</span></span>  <br/> |
|[<span data-ttu-id="b0501-120">Destinatários (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="b0501-120">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="b0501-121">Representa uma coleção dos destinatários que receberão acesso à pasta compartilhada.</span><span class="sxs-lookup"><span data-stu-id="b0501-121">Represents a collection of recipients that will be granted access to the shared folder.</span></span>  <br/> |
|[<span data-ttu-id="b0501-122">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="b0501-122">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="b0501-123">Define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada.</span><span class="sxs-lookup"><span data-stu-id="b0501-123">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b0501-124">Text value</span><span class="sxs-lookup"><span data-stu-id="b0501-124">Text value</span></span>

<span data-ttu-id="b0501-125">É necessário um valor de texto que representa um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="b0501-125">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b0501-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="b0501-126">Remarks</span></span>

<span data-ttu-id="b0501-127">O esquema que descreve este elemento está localizado no diretório Virtual do IIS que hospeda o Exchange Web Services do computador que está executando o Microsoft Exchange Server que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="b0501-127">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0501-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b0501-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0501-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="b0501-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b0501-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b0501-130">Schema Name</span></span>  <br/> |<span data-ttu-id="b0501-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b0501-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="b0501-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b0501-132">Validation File</span></span>  <br/> |<span data-ttu-id="b0501-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b0501-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b0501-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b0501-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0501-135">False</span><span class="sxs-lookup"><span data-stu-id="b0501-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0501-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="b0501-136">See also</span></span>

- [<span data-ttu-id="b0501-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b0501-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

