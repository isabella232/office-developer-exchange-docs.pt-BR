---
title: Solicitação (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: beeb5371-f57b-4346-9753-035dd42c6bee
description: O elemento de solicitação representa uma solicitação de GetFederationInformationRequest (SOAP).
ms.openlocfilehash: 0fb9301c2f318aa2c27155675dd3c43b41aabecd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825119"
---
# <a name="request-getfederationinformation-soap"></a><span data-ttu-id="5d47c-103">Solicitação (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5d47c-103">Request (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="5d47c-104">O elemento de **solicitação** representa uma solicitação de [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="5d47c-104">The **Request** element represents a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md) request.</span></span> 
  
```XML
<Request>
   <Domain/>
</Request>
```

 <span data-ttu-id="5d47c-105">**GetFederationInformationRequest**</span><span class="sxs-lookup"><span data-stu-id="5d47c-105">**GetFederationInformationRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d47c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5d47c-106">Attributes and elements</span></span>

<span data-ttu-id="5d47c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5d47c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d47c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5d47c-108">Attributes</span></span>

<span data-ttu-id="5d47c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5d47c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d47c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5d47c-110">Child elements</span></span>

|<span data-ttu-id="5d47c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5d47c-111">**Element**</span></span>|<span data-ttu-id="5d47c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5d47c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d47c-113">Domínio (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5d47c-113">Domain (GetFederationInformation) (SOAP)</span></span>](domain-getfederationinformationsoap.md) <br/> |<span data-ttu-id="5d47c-114">Identifica o domínio que tenha uma relação de confiança de Federação.</span><span class="sxs-lookup"><span data-stu-id="5d47c-114">Identifies the domain that has a federation trust.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5d47c-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5d47c-115">Parent elements</span></span>

|<span data-ttu-id="5d47c-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5d47c-116">**Element**</span></span>|<span data-ttu-id="5d47c-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5d47c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d47c-118">GetFederationInformationRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5d47c-118">GetFederationInformationRequestMessage (SOAP)</span></span>](getfederationinformationrequestmessage-soap.md) <br/> |<span data-ttu-id="5d47c-119">Prepara uma chamada para o servidor para dados de configuração de solicitação para o serviço de token de segurança (STS).</span><span class="sxs-lookup"><span data-stu-id="5d47c-119">Prepares a call to the server to request configuration data for the security token service (STS).</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="5d47c-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5d47c-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d47c-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="5d47c-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="5d47c-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5d47c-122">Schema Name</span></span>  <br/> |<span data-ttu-id="5d47c-123">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="5d47c-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="5d47c-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5d47c-124">Validation File</span></span>  <br/> |<span data-ttu-id="5d47c-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5d47c-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5d47c-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5d47c-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="5d47c-127">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="5d47c-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d47c-128">Ver também</span><span class="sxs-lookup"><span data-stu-id="5d47c-128">See also</span></span>



[<span data-ttu-id="5d47c-129">Trabalhando com a descoberta automática</span><span class="sxs-lookup"><span data-stu-id="5d47c-129">Working with Autodiscover</span></span>](http://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)

