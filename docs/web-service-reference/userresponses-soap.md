---
title: Userresponses (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a48766df-4cc8-47c2-a8c1-826daec94e5a
description: O elemento userresponses contém as definições de configuração para cada usuário solicitado.
ms.openlocfilehash: db2bab16334b90395d29dc03353dce05b0e45357
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526743"
---
# <a name="userresponses-soap"></a><span data-ttu-id="fc404-103">Userresponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fc404-103">UserResponses (SOAP)</span></span>

<span data-ttu-id="fc404-104">O elemento **Userresponses** contém as definições de configuração para cada usuário solicitado.</span><span class="sxs-lookup"><span data-stu-id="fc404-104">The **UserResponses** element contains the configuration settings for each requested user.</span></span> 
  
```XML
<UserResponses>
   <UserResponse/>
</UserResponses>
```

 <span data-ttu-id="fc404-105">**ArrayOfUserResponse**</span><span class="sxs-lookup"><span data-stu-id="fc404-105">**ArrayOfUserResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc404-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fc404-106">Attributes and elements</span></span>

<span data-ttu-id="fc404-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fc404-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc404-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fc404-108">Attributes</span></span>

<span data-ttu-id="fc404-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc404-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc404-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fc404-110">Child elements</span></span>

|<span data-ttu-id="fc404-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fc404-111">**Element**</span></span>|<span data-ttu-id="fc404-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc404-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc404-113">Userresponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fc404-113">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="fc404-114">Representa uma resposta a uma solicitação de [operação de GetUserSettings (SOAP)](getusersettings-operation-soap.md) para um usuário individual.</span><span class="sxs-lookup"><span data-stu-id="fc404-114">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fc404-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fc404-115">Parent elements</span></span>

|<span data-ttu-id="fc404-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fc404-116">**Element**</span></span>|<span data-ttu-id="fc404-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc404-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc404-118">Resposta (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fc404-118">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="fc404-119">Contém a resposta a uma solicitação de [operação GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="fc404-119">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="fc404-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fc404-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc404-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="fc404-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="fc404-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fc404-122">Schema Name</span></span>  <br/> |<span data-ttu-id="fc404-123">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="fc404-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="fc404-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fc404-124">Validation File</span></span>  <br/> |<span data-ttu-id="fc404-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fc404-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fc404-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fc404-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc404-127">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="fc404-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc404-128">Confira também</span><span class="sxs-lookup"><span data-stu-id="fc404-128">See also</span></span>



[<span data-ttu-id="fc404-129">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fc404-129">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

