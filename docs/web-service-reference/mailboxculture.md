---
title: MailboxCulture
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxCulture
api_type:
- schema
ms.assetid: 105cc061-3c35-455f-b102-8023e2055632
description: O elemento MailboxCulture indica a cultura a ser usada ao abrir uma caixa de correio. Esse elemento ocorre no cabeçalho SOAP.
ms.openlocfilehash: 5760bac3b4589cdba599c5200db7d77b73855ca4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467806"
---
# <a name="mailboxculture"></a><span data-ttu-id="af1c5-104">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="af1c5-104">MailboxCulture</span></span>

<span data-ttu-id="af1c5-105">O elemento **MailboxCulture** indica a cultura a ser usada ao abrir uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="af1c5-105">The **MailboxCulture** element indicates the culture to use when opening a mailbox.</span></span> <span data-ttu-id="af1c5-106">Esse elemento ocorre no cabeçalho SOAP.</span><span class="sxs-lookup"><span data-stu-id="af1c5-106">This element occurs in the SOAP header.</span></span> 
  
```xml
<MailboxCulture/>
```

<span data-ttu-id="af1c5-107">**MailboxCultureType**</span><span class="sxs-lookup"><span data-stu-id="af1c5-107">**MailboxCultureType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="af1c5-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="af1c5-108">Attributes and elements</span></span>

<span data-ttu-id="af1c5-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="af1c5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af1c5-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="af1c5-110">Attributes</span></span>

<span data-ttu-id="af1c5-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af1c5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af1c5-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="af1c5-112">Child elements</span></span>

<span data-ttu-id="af1c5-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="af1c5-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="af1c5-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="af1c5-114">Parent elements</span></span>

<span data-ttu-id="af1c5-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af1c5-115">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="af1c5-116">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="af1c5-116">Text value</span></span>

<span data-ttu-id="af1c5-117">O valor de texto indica o idioma usado nas operações do serviço Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="af1c5-117">The text value indicates the language that is used in the Exchange Web Service operations.</span></span> <span data-ttu-id="af1c5-118">Os valores possíveis para esse elemento são descritos pela RFC 3066.</span><span class="sxs-lookup"><span data-stu-id="af1c5-118">The possible values for this element are described by RFC 3066.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="af1c5-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="af1c5-119">Remarks</span></span>

<span data-ttu-id="af1c5-120">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange Server com a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="af1c5-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af1c5-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="af1c5-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af1c5-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="af1c5-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="af1c5-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="af1c5-123">Schema Name</span></span>  <br/> |<span data-ttu-id="af1c5-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="af1c5-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="af1c5-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="af1c5-125">Validation File</span></span>  <br/> |<span data-ttu-id="af1c5-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="af1c5-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="af1c5-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="af1c5-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="af1c5-128">False</span><span class="sxs-lookup"><span data-stu-id="af1c5-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af1c5-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="af1c5-129">See also</span></span>

- [<span data-ttu-id="af1c5-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="af1c5-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

