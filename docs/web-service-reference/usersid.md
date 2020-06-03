---
title: Userid
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
description: O elemento userid representa a forma SDDL (Security Descriptor Definition Language) do identificador de segurança do usuário em um cabeçalho SOAP de contexto de segurança serializado. Não há suporte para serialização de token.
ms.openlocfilehash: b8ee51b1998546fc4ab14bd3666192ae63c8dba8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462014"
---
# <a name="usersid"></a><span data-ttu-id="74926-104">Userid</span><span class="sxs-lookup"><span data-stu-id="74926-104">UserSid</span></span>

<span data-ttu-id="74926-105">O elemento **userid** representa a forma SDDL (Security Descriptor Definition Language) do identificador de segurança do usuário em um cabeçalho SOAP de contexto de segurança serializado.</span><span class="sxs-lookup"><span data-stu-id="74926-105">The **UserSid** element represents the security descriptor definition language (SDDL) form of the user security identifier in a serialized security context SOAP header.</span></span> <span data-ttu-id="74926-106">Não há suporte para serialização de token.</span><span class="sxs-lookup"><span data-stu-id="74926-106">Token serialization is not supported.</span></span> 
  
```xml
<UserSid/>
```

 <span data-ttu-id="74926-107">**String**</span><span class="sxs-lookup"><span data-stu-id="74926-107">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74926-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="74926-108">Attributes and elements</span></span>

<span data-ttu-id="74926-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="74926-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74926-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="74926-110">Attributes</span></span>

<span data-ttu-id="74926-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74926-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74926-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="74926-112">Child elements</span></span>

<span data-ttu-id="74926-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="74926-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="74926-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="74926-114">Parent elements</span></span>

|<span data-ttu-id="74926-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="74926-115">**Element**</span></span>|<span data-ttu-id="74926-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="74926-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74926-117">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="74926-117">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="74926-118">Usado no cabeçalho SOAP para serialização de token na autenticação de servidor para servidor.</span><span class="sxs-lookup"><span data-stu-id="74926-118">Used in the SOAP header for token serialization in server-to-server authentication.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="74926-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="74926-119">Text value</span></span>

<span data-ttu-id="74926-120">O valor de texto representa o identificador de segurança de um usuário.</span><span class="sxs-lookup"><span data-stu-id="74926-120">The text value represents a user's security identifier.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="74926-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="74926-121">Remarks</span></span>

<span data-ttu-id="74926-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="74926-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74926-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="74926-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74926-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="74926-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="74926-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="74926-125">Schema Name</span></span>  <br/> |<span data-ttu-id="74926-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="74926-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="74926-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="74926-127">Validation File</span></span>  <br/> |<span data-ttu-id="74926-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="74926-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="74926-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="74926-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="74926-130">False</span><span class="sxs-lookup"><span data-stu-id="74926-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74926-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="74926-131">See also</span></span>



- [<span data-ttu-id="74926-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="74926-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

