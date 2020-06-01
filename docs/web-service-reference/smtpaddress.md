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
description: O elemento SmtpAddress representa o endereço SMTP (Simple Mail Transfer Protocol) de uma conta a ser usada para representação ou para um endereço de destinatário SMTP de um calendário ou solicitação de compartilhamento de contato.
ms.openlocfilehash: 915ff328cc384c1f2884e9fbea8c10c1ebc79288
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466686"
---
# <a name="smtpaddress"></a><span data-ttu-id="f4e2b-103">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="f4e2b-103">SmtpAddress</span></span>

<span data-ttu-id="f4e2b-104">O elemento **smtpAddress** representa o endereço SMTP (Simple Mail Transfer Protocol) de uma conta a ser usada para representação ou para um endereço de destinatário SMTP de um calendário ou solicitação de compartilhamento de contato.</span><span class="sxs-lookup"><span data-stu-id="f4e2b-104">The **SmtpAddress** element represents the Simple Mail Transfer Protocol (SMTP) address of an account to be used for impersonation or a Simple Mail Transfer Protocol (SMTP) recipient address of a calendar or contact sharing request.</span></span> 
  
```xml
<SmtpAddress/>
```

<span data-ttu-id="f4e2b-105">**SmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="f4e2b-105">**SmtpAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f4e2b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f4e2b-106">Attributes and elements</span></span>

<span data-ttu-id="f4e2b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f4e2b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4e2b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f4e2b-108">Attributes</span></span>

<span data-ttu-id="f4e2b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f4e2b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4e2b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f4e2b-110">Child elements</span></span>

<span data-ttu-id="f4e2b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f4e2b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f4e2b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f4e2b-112">Parent elements</span></span>

|<span data-ttu-id="f4e2b-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f4e2b-113">**Element**</span></span>|<span data-ttu-id="f4e2b-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f4e2b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4e2b-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="f4e2b-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="f4e2b-116">Representa uma conta a ser representada quando você estiver usando o cabeçalho SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="f4e2b-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="f4e2b-117">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="f4e2b-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="f4e2b-118">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="f4e2b-118">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="f4e2b-119">Representa um destinatário inválido para uma mensagem de compartilhamento de calendário ou contato.</span><span class="sxs-lookup"><span data-stu-id="f4e2b-119">Represents an invalid recipient for a calendar sharing or contact sharing message.</span></span>  <br/> |
|[<span data-ttu-id="f4e2b-120">Destinatários (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="f4e2b-120">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="f4e2b-121">Representa uma coleção de destinatários aos quais será concedido acesso à pasta compartilhada.</span><span class="sxs-lookup"><span data-stu-id="f4e2b-121">Represents a collection of recipients that will be granted access to the shared folder.</span></span>  <br/> |
|[<span data-ttu-id="f4e2b-122">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="f4e2b-122">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="f4e2b-123">Define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada.</span><span class="sxs-lookup"><span data-stu-id="f4e2b-123">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f4e2b-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="f4e2b-124">Text value</span></span>

<span data-ttu-id="f4e2b-125">Um valor de texto que representa um endereço SMTP é necessário.</span><span class="sxs-lookup"><span data-stu-id="f4e2b-125">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f4e2b-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="f4e2b-126">Remarks</span></span>

<span data-ttu-id="f4e2b-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f4e2b-127">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4e2b-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f4e2b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4e2b-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="f4e2b-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f4e2b-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f4e2b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="f4e2b-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f4e2b-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="f4e2b-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f4e2b-132">Validation File</span></span>  <br/> |<span data-ttu-id="f4e2b-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f4e2b-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f4e2b-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f4e2b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="f4e2b-135">False</span><span class="sxs-lookup"><span data-stu-id="f4e2b-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4e2b-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="f4e2b-136">See also</span></span>

- [<span data-ttu-id="f4e2b-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f4e2b-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

