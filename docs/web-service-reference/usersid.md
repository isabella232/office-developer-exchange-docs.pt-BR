---
title: UserSid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserSid
api_type:
- schema
ms.assetid: f8a0dcd9-8564-4e35-b307-c5d2761b48d8
description: O elemento UserSid representa um formulário de segurança descritor definition language (SDDL) do identificador de segurança de usuário em um cabeçalho SOAP de contexto de segurança serializados. Serialização de token não é suportada.
ms.openlocfilehash: 3c72f68638f99a4ee5081517027f0834ebf65b49
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838004"
---
# <a name="usersid"></a><span data-ttu-id="94e5a-104">UserSid</span><span class="sxs-lookup"><span data-stu-id="94e5a-104">UserSid</span></span>

<span data-ttu-id="94e5a-105">O elemento **UserSid** representa um formulário de segurança descritor definition language (SDDL) do identificador de segurança de usuário em um cabeçalho SOAP de contexto de segurança serializados.</span><span class="sxs-lookup"><span data-stu-id="94e5a-105">The **UserSid** element represents the security descriptor definition language (SDDL) form of the user security identifier in a serialized security context SOAP header.</span></span> <span data-ttu-id="94e5a-106">Serialização de token não é suportada.</span><span class="sxs-lookup"><span data-stu-id="94e5a-106">Token serialization is not supported.</span></span> 
  
```xml
<UserSid/>
```

 <span data-ttu-id="94e5a-107">**String**</span><span class="sxs-lookup"><span data-stu-id="94e5a-107">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94e5a-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="94e5a-108">Attributes and elements</span></span>

<span data-ttu-id="94e5a-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="94e5a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94e5a-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="94e5a-110">Attributes</span></span>

<span data-ttu-id="94e5a-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="94e5a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94e5a-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="94e5a-112">Child elements</span></span>

<span data-ttu-id="94e5a-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="94e5a-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="94e5a-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="94e5a-114">Parent elements</span></span>

|<span data-ttu-id="94e5a-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="94e5a-115">**Element**</span></span>|<span data-ttu-id="94e5a-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="94e5a-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94e5a-117">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="94e5a-117">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="94e5a-118">Usado no cabeçalho SOAP para serialização de token de autenticação de servidor-para-servidor.</span><span class="sxs-lookup"><span data-stu-id="94e5a-118">Used in the SOAP header for token serialization in server-to-server authentication.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="94e5a-119">Text value</span><span class="sxs-lookup"><span data-stu-id="94e5a-119">Text value</span></span>

<span data-ttu-id="94e5a-120">O valor de texto representa o identificador de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="94e5a-120">The text value represents a user's security identifier.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="94e5a-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="94e5a-121">Remarks</span></span>

<span data-ttu-id="94e5a-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="94e5a-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94e5a-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="94e5a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94e5a-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="94e5a-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="94e5a-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="94e5a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="94e5a-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="94e5a-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="94e5a-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="94e5a-127">Validation File</span></span>  <br/> |<span data-ttu-id="94e5a-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="94e5a-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="94e5a-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="94e5a-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="94e5a-130">False</span><span class="sxs-lookup"><span data-stu-id="94e5a-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="94e5a-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="94e5a-131">See also</span></span>



- [<span data-ttu-id="94e5a-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="94e5a-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

