---
title: Destinatários (ArrayOfSmtpAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recipients
api_type:
- schema
ms.assetid: cf68417d-85cf-49e0-857a-f987d3675344
description: O elemento Recipients especifica uma matriz de destinatários de uma mensagem.
ms.openlocfilehash: 4c2478a81836c2e52baad9c928d112108679b837
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465503"
---
# <a name="recipients-arrayofsmtpaddresstype"></a><span data-ttu-id="64a4e-103">Destinatários (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="64a4e-103">Recipients (ArrayOfSmtpAddressType)</span></span>

<span data-ttu-id="64a4e-104">O elemento **Recipients** especifica uma matriz de destinatários de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="64a4e-104">The **Recipients** element specifies an array of recipients of a message.</span></span> 
  
```xml
<Recipients>   <SmtpAddress/></Recipients>
```

 <span data-ttu-id="64a4e-105">**ArrayOfSmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="64a4e-105">**ArrayOfSmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64a4e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="64a4e-106">Attributes and elements</span></span>

<span data-ttu-id="64a4e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="64a4e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64a4e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="64a4e-108">Attributes</span></span>

<span data-ttu-id="64a4e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64a4e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64a4e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="64a4e-110">Child elements</span></span>

|<span data-ttu-id="64a4e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="64a4e-111">**Element**</span></span>|<span data-ttu-id="64a4e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="64a4e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64a4e-113">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="64a4e-113">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="64a4e-114">Representa o endereço de destinatário do protocolo SMTP de uma solicitação de compartilhamento de contato ou calendário.</span><span class="sxs-lookup"><span data-stu-id="64a4e-114">Represents the Simple Mail Transfer Protocol (SMTP) recipient address of a calendar or contact sharing request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="64a4e-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="64a4e-115">Parent elements</span></span>

|<span data-ttu-id="64a4e-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="64a4e-116">**Element**</span></span>|<span data-ttu-id="64a4e-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="64a4e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64a4e-118">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="64a4e-118">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="64a4e-119">Define uma solicitação para obter um token de autenticação opaco que identifica o convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="64a4e-119">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="64a4e-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="64a4e-120">Remarks</span></span>

<span data-ttu-id="64a4e-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="64a4e-121">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64a4e-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="64a4e-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64a4e-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="64a4e-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="64a4e-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="64a4e-124">Schema Name</span></span>  <br/> |<span data-ttu-id="64a4e-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="64a4e-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="64a4e-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="64a4e-126">Validation File</span></span>  <br/> |<span data-ttu-id="64a4e-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="64a4e-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="64a4e-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="64a4e-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="64a4e-129">False</span><span class="sxs-lookup"><span data-stu-id="64a4e-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64a4e-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="64a4e-130">See also</span></span>



[<span data-ttu-id="64a4e-131">Operação GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="64a4e-131">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="64a4e-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="64a4e-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

