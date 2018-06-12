---
title: SID
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
description: O elemento SID representa um formulário de segurança descritor definition language (SDDL) do identificador de segurança (SID) para a conta usada para representação ou acesso de representante.
ms.openlocfilehash: efcea42c12ec1d26ea31fdb8de337c37a2338a96
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825492"
---
# <a name="sid"></a><span data-ttu-id="8aaa8-103">SID</span><span class="sxs-lookup"><span data-stu-id="8aaa8-103">SID</span></span>

<span data-ttu-id="8aaa8-104">O elemento **SID** representa um formulário de segurança descritor definition language (SDDL) do identificador de segurança (SID) para a conta usada para representação ou acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="8aaa8-104">The **SID** element represents the security descriptor definition language (SDDL) form of the security identifier (SID) for the account to use for impersonation or delegate access.</span></span> 
  
```xml
<SID/>
```

 <span data-ttu-id="8aaa8-105">**SIDType**</span><span class="sxs-lookup"><span data-stu-id="8aaa8-105">**SIDType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8aaa8-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8aaa8-106">Attributes and elements</span></span>

<span data-ttu-id="8aaa8-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8aaa8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8aaa8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8aaa8-108">Attributes</span></span>

<span data-ttu-id="8aaa8-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8aaa8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8aaa8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8aaa8-110">Child elements</span></span>

<span data-ttu-id="8aaa8-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8aaa8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8aaa8-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8aaa8-112">Parent elements</span></span>

|<span data-ttu-id="8aaa8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8aaa8-113">**Element**</span></span>|<span data-ttu-id="8aaa8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8aaa8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8aaa8-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="8aaa8-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="8aaa8-116">Representa uma conta para representar ao usar o cabeçalho SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="8aaa8-116">Represents an account to impersonate when using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="8aaa8-117">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="8aaa8-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="8aaa8-118">UserId</span><span class="sxs-lookup"><span data-stu-id="8aaa8-118">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="8aaa8-119">Identifica um usuário delegado ou um usuário com permissões de acesso de pasta.</span><span class="sxs-lookup"><span data-stu-id="8aaa8-119">Identifies a delegate user or a user with folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8aaa8-120">Text value</span><span class="sxs-lookup"><span data-stu-id="8aaa8-120">Text value</span></span>

<span data-ttu-id="8aaa8-121">O valor de texto é uma representação de cadeia de caracteres de um SID.</span><span class="sxs-lookup"><span data-stu-id="8aaa8-121">The text value is a string representation of a SID.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8aaa8-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="8aaa8-122">Remarks</span></span>

<span data-ttu-id="8aaa8-123">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server com a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="8aaa8-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8aaa8-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8aaa8-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8aaa8-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="8aaa8-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8aaa8-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8aaa8-126">Schema Name</span></span>  <br/> |<span data-ttu-id="8aaa8-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8aaa8-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="8aaa8-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8aaa8-128">Validation File</span></span>  <br/> |<span data-ttu-id="8aaa8-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8aaa8-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8aaa8-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8aaa8-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="8aaa8-131">False</span><span class="sxs-lookup"><span data-stu-id="8aaa8-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8aaa8-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="8aaa8-132">See also</span></span>



- [<span data-ttu-id="8aaa8-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8aaa8-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

