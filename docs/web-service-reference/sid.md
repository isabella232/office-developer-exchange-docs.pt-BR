---
title: Identifica
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SID
api_type:
- schema
ms.assetid: 2f33b29b-163b-4106-a74d-6fb76ec38951
description: O elemento SID representa a forma SDDL (Security Descriptor Definition Language) do identificador de segurança (SID) da conta a ser usada para a representação ou acesso de representante.
ms.openlocfilehash: 0e3f740e9a056f7c0042049d97757b5f2d3c441d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468044"
---
# <a name="sid"></a><span data-ttu-id="42cc3-103">Identifica</span><span class="sxs-lookup"><span data-stu-id="42cc3-103">SID</span></span>

<span data-ttu-id="42cc3-104">O elemento **Sid** representa a forma SDDL (Security Descriptor Definition Language) do identificador de segurança (SID) da conta a ser usada para a representação ou acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="42cc3-104">The **SID** element represents the security descriptor definition language (SDDL) form of the security identifier (SID) for the account to use for impersonation or delegate access.</span></span> 
  
```xml
<SID/>
```

 <span data-ttu-id="42cc3-105">**SIDType**</span><span class="sxs-lookup"><span data-stu-id="42cc3-105">**SIDType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="42cc3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="42cc3-106">Attributes and elements</span></span>

<span data-ttu-id="42cc3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="42cc3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="42cc3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="42cc3-108">Attributes</span></span>

<span data-ttu-id="42cc3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42cc3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="42cc3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="42cc3-110">Child elements</span></span>

<span data-ttu-id="42cc3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="42cc3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="42cc3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="42cc3-112">Parent elements</span></span>

|<span data-ttu-id="42cc3-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="42cc3-113">**Element**</span></span>|<span data-ttu-id="42cc3-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="42cc3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="42cc3-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="42cc3-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="42cc3-116">Representa uma conta a ser representada ao usar o cabeçalho SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="42cc3-116">Represents an account to impersonate when using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="42cc3-117">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="42cc3-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="42cc3-118">UserId</span><span class="sxs-lookup"><span data-stu-id="42cc3-118">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="42cc3-119">Identifica um usuário delegado ou um usuário com permissões de acesso à pasta.</span><span class="sxs-lookup"><span data-stu-id="42cc3-119">Identifies a delegate user or a user with folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="42cc3-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="42cc3-120">Text value</span></span>

<span data-ttu-id="42cc3-121">O valor de texto é uma representação de cadeia de caracteres de um SID.</span><span class="sxs-lookup"><span data-stu-id="42cc3-121">The text value is a string representation of a SID.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="42cc3-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="42cc3-122">Remarks</span></span>

<span data-ttu-id="42cc3-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange Server com a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="42cc3-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="42cc3-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="42cc3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="42cc3-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="42cc3-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="42cc3-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="42cc3-126">Schema Name</span></span>  <br/> |<span data-ttu-id="42cc3-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="42cc3-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="42cc3-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="42cc3-128">Validation File</span></span>  <br/> |<span data-ttu-id="42cc3-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="42cc3-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="42cc3-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="42cc3-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="42cc3-131">False</span><span class="sxs-lookup"><span data-stu-id="42cc3-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="42cc3-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="42cc3-132">See also</span></span>



- [<span data-ttu-id="42cc3-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="42cc3-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

