---
title: PrincipalName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PrincipalName
api_type:
- schema
ms.assetid: 88c142d4-0bc7-43ea-a997-d7200664d900
description: O elemento PrincipalName representa o nome de usuário principal (UPN) da conta a ser usada para a representação do Exchange.
ms.openlocfilehash: d8557ce0435a11a5602372517db1f576028a9c97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824882"
---
# <a name="principalname"></a><span data-ttu-id="5383b-103">PrincipalName</span><span class="sxs-lookup"><span data-stu-id="5383b-103">PrincipalName</span></span>

<span data-ttu-id="5383b-104">O elemento **PrincipalName** representa o nome de usuário principal (UPN) da conta a ser usada para a representação do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5383b-104">The **PrincipalName** element represents the user principal name (UPN) of the account to be used for Exchange impersonation.</span></span> 
  
```xml
<PrincipalName/>
```

 <span data-ttu-id="5383b-105">**PrincipalNameType**</span><span class="sxs-lookup"><span data-stu-id="5383b-105">**PrincipalNameType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5383b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5383b-106">Attributes and elements</span></span>

<span data-ttu-id="5383b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5383b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5383b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5383b-108">Attributes</span></span>

<span data-ttu-id="5383b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5383b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5383b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5383b-110">Child elements</span></span>

<span data-ttu-id="5383b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5383b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5383b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5383b-112">Parent elements</span></span>

|<span data-ttu-id="5383b-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5383b-113">**Element**</span></span>|<span data-ttu-id="5383b-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5383b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5383b-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="5383b-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="5383b-116">Representa uma conta para representar quando você estiver usando o cabeçalho SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="5383b-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="5383b-117">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="5383b-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5383b-118">Text value</span><span class="sxs-lookup"><span data-stu-id="5383b-118">Text value</span></span>

<span data-ttu-id="5383b-119">O valor de texto representa o UPN do usuário.</span><span class="sxs-lookup"><span data-stu-id="5383b-119">The text value represents the UPN of a user.</span></span> <span data-ttu-id="5383b-120">Esse valor existe no objeto de usuário no serviço de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5383b-120">This value exists on the user object in the Active Directory directory service.</span></span> <span data-ttu-id="5383b-121">Contém o nome de logon do usuário e um nome de domínio que identifica o domínio no qual a conta de usuário está localizada no seguinte formato: `someone@example.com`.</span><span class="sxs-lookup"><span data-stu-id="5383b-121">This contains the user logon name and a domain name that identifies the domain in which the user account is located, in the following format:  `someone@example.com`.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5383b-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="5383b-122">Remarks</span></span>

<span data-ttu-id="5383b-123">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="5383b-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5383b-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5383b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5383b-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="5383b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5383b-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5383b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="5383b-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5383b-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="5383b-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5383b-128">Validation File</span></span>  <br/> |<span data-ttu-id="5383b-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5383b-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5383b-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5383b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="5383b-131">False</span><span class="sxs-lookup"><span data-stu-id="5383b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5383b-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="5383b-132">See also</span></span>



- [<span data-ttu-id="5383b-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5383b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="5383b-134">Autorização de servidor-para-servidor no EWS</span><span class="sxs-lookup"><span data-stu-id="5383b-134">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

