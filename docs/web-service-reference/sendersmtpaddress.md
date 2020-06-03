---
title: SenderSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SenderSmtpAddress
api_type:
- schema
ms.assetid: e39c7df7-4bfa-455f-b4bb-1f1d05398eec
description: O elemento SenderSmtpAddress representa o endereço de email SMTP correspondente à caixa de correio que contém a pasta que será compartilhada.
ms.openlocfilehash: 73047dcecfbccb55d74e373891c3154bc7baeeba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464893"
---
# <a name="sendersmtpaddress"></a><span data-ttu-id="6352d-103">SenderSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="6352d-103">SenderSmtpAddress</span></span>

<span data-ttu-id="6352d-104">O elemento **SenderSmtpAddress** representa o endereço de email SMTP correspondente à caixa de correio que contém a pasta que será compartilhada.</span><span class="sxs-lookup"><span data-stu-id="6352d-104">The **SenderSmtpAddress** element represents the SMTP e-mail address corresponding to the mailbox that contains the folder that will be shared.</span></span> 
  
```xml
<SenderSmtpAddress/>
```

 <span data-ttu-id="6352d-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="6352d-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6352d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6352d-106">Attributes and elements</span></span>

<span data-ttu-id="6352d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6352d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6352d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6352d-108">Attributes</span></span>

<span data-ttu-id="6352d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6352d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6352d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6352d-110">Child elements</span></span>

<span data-ttu-id="6352d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6352d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6352d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6352d-112">Parent elements</span></span>

|<span data-ttu-id="6352d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6352d-113">**Element**</span></span>|<span data-ttu-id="6352d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6352d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6352d-115">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="6352d-115">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="6352d-116">Define uma solicitação para obter um token de autenticação opaco que identifica o convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="6352d-116">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6352d-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="6352d-117">Text value</span></span>

<span data-ttu-id="6352d-118">Um valor de texto que representa um endereço SMTP é necessário.</span><span class="sxs-lookup"><span data-stu-id="6352d-118">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6352d-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="6352d-119">Remarks</span></span>

<span data-ttu-id="6352d-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="6352d-120">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6352d-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6352d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6352d-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="6352d-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6352d-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6352d-123">Schema Name</span></span>  <br/> |<span data-ttu-id="6352d-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6352d-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6352d-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6352d-125">Validation File</span></span>  <br/> |<span data-ttu-id="6352d-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6352d-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6352d-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6352d-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="6352d-128">False</span><span class="sxs-lookup"><span data-stu-id="6352d-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6352d-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="6352d-129">See also</span></span>



[<span data-ttu-id="6352d-130">Operação GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="6352d-130">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="6352d-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6352d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

