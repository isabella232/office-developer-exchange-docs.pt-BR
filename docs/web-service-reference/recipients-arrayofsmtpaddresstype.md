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
description: O elemento de destinatários Especifica uma matriz de destinatários de uma mensagem.
ms.openlocfilehash: 8490988043b1e06fd3a8f553fcefaeb2e90e9d31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824988"
---
# <a name="recipients-arrayofsmtpaddresstype"></a><span data-ttu-id="30dd0-103">Destinatários (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="30dd0-103">Recipients (ArrayOfSmtpAddressType)</span></span>

<span data-ttu-id="30dd0-104">O elemento de **destinatários** Especifica uma matriz de destinatários de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="30dd0-104">The **Recipients** element specifies an array of recipients of a message.</span></span> 
  
```xml
<Recipients>   <SmtpAddress/></Recipients>
```

 <span data-ttu-id="30dd0-105">**ArrayOfSmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="30dd0-105">**ArrayOfSmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30dd0-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="30dd0-106">Attributes and elements</span></span>

<span data-ttu-id="30dd0-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="30dd0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30dd0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="30dd0-108">Attributes</span></span>

<span data-ttu-id="30dd0-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="30dd0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30dd0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="30dd0-110">Child elements</span></span>

|<span data-ttu-id="30dd0-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="30dd0-111">**Element**</span></span>|<span data-ttu-id="30dd0-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="30dd0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30dd0-113">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="30dd0-113">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="30dd0-114">Representa o endereço do destinatário Simple Mail Transfer Protocol (SMTP) de um calendário ou uma solicitação de compartilhamento do contato.</span><span class="sxs-lookup"><span data-stu-id="30dd0-114">Represents the Simple Mail Transfer Protocol (SMTP) recipient address of a calendar or contact sharing request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="30dd0-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="30dd0-115">Parent elements</span></span>

|<span data-ttu-id="30dd0-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="30dd0-116">**Element**</span></span>|<span data-ttu-id="30dd0-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="30dd0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30dd0-118">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="30dd0-118">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="30dd0-119">Define uma solicitação para obter um token de autenticação opaco que identifica o convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="30dd0-119">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="30dd0-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="30dd0-120">Remarks</span></span>

<span data-ttu-id="30dd0-121">O esquema que descreve este elemento está localizado no diretório Virtual do IIS que hospeda o Exchange Web Services do computador que está executando o Microsoft Exchange Server que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="30dd0-121">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30dd0-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="30dd0-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30dd0-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="30dd0-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="30dd0-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="30dd0-124">Schema Name</span></span>  <br/> |<span data-ttu-id="30dd0-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="30dd0-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="30dd0-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="30dd0-126">Validation File</span></span>  <br/> |<span data-ttu-id="30dd0-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="30dd0-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="30dd0-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="30dd0-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="30dd0-129">False</span><span class="sxs-lookup"><span data-stu-id="30dd0-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="30dd0-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="30dd0-130">See also</span></span>



[<span data-ttu-id="30dd0-131">Operação GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="30dd0-131">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="30dd0-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="30dd0-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

