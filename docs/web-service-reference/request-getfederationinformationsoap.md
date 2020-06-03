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
description: O elemento Request representa uma solicitação GetFederationInformationRequest (SOAP).
ms.openlocfilehash: dbd88537d03f6325cf0025d08c63ae486544d705
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459578"
---
# <a name="request-getfederationinformation-soap"></a><span data-ttu-id="cf2ab-103">Solicitação (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf2ab-103">Request (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="cf2ab-104">O elemento **Request** representa uma solicitação [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="cf2ab-104">The **Request** element represents a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md) request.</span></span> 
  
```XML
<Request>
   <Domain/>
</Request>
```

 <span data-ttu-id="cf2ab-105">**GetFederationInformationRequest**</span><span class="sxs-lookup"><span data-stu-id="cf2ab-105">**GetFederationInformationRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf2ab-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cf2ab-106">Attributes and elements</span></span>

<span data-ttu-id="cf2ab-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cf2ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf2ab-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cf2ab-108">Attributes</span></span>

<span data-ttu-id="cf2ab-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cf2ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf2ab-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cf2ab-110">Child elements</span></span>

|<span data-ttu-id="cf2ab-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cf2ab-111">**Element**</span></span>|<span data-ttu-id="cf2ab-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cf2ab-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf2ab-113">Domínio (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf2ab-113">Domain (GetFederationInformation) (SOAP)</span></span>](domain-getfederationinformationsoap.md) <br/> |<span data-ttu-id="cf2ab-114">Identifica o domínio que tem uma confiança de Federação.</span><span class="sxs-lookup"><span data-stu-id="cf2ab-114">Identifies the domain that has a federation trust.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cf2ab-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cf2ab-115">Parent elements</span></span>

|<span data-ttu-id="cf2ab-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cf2ab-116">**Element**</span></span>|<span data-ttu-id="cf2ab-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cf2ab-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf2ab-118">GetFederationInformationRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf2ab-118">GetFederationInformationRequestMessage (SOAP)</span></span>](getfederationinformationrequestmessage-soap.md) <br/> |<span data-ttu-id="cf2ab-119">Prepara uma chamada para o servidor para solicitar dados de configuração para o serviço de token de segurança (STS).</span><span class="sxs-lookup"><span data-stu-id="cf2ab-119">Prepares a call to the server to request configuration data for the security token service (STS).</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="cf2ab-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cf2ab-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf2ab-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="cf2ab-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="cf2ab-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cf2ab-122">Schema Name</span></span>  <br/> |<span data-ttu-id="cf2ab-123">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="cf2ab-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="cf2ab-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cf2ab-124">Validation File</span></span>  <br/> |<span data-ttu-id="cf2ab-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cf2ab-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cf2ab-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cf2ab-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf2ab-127">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="cf2ab-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf2ab-128">Confira também</span><span class="sxs-lookup"><span data-stu-id="cf2ab-128">See also</span></span>



[<span data-ttu-id="cf2ab-129">Trabalhando com a descoberta automática</span><span class="sxs-lookup"><span data-stu-id="cf2ab-129">Working with Autodiscover</span></span>](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)

