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
description: O elemento PrincipalName representa o nome principal do usuário (UPN) da conta a ser usada para a representação do Exchange.
ms.openlocfilehash: 31412c1461264e28bf8d52c957a457e8d1e847ef
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44440187"
---
# <a name="principalname"></a><span data-ttu-id="dbadd-103">PrincipalName</span><span class="sxs-lookup"><span data-stu-id="dbadd-103">PrincipalName</span></span>

<span data-ttu-id="dbadd-104">O elemento **PrincipalName** representa o nome principal do usuário (UPN) da conta a ser usada para a representação do Exchange.</span><span class="sxs-lookup"><span data-stu-id="dbadd-104">The **PrincipalName** element represents the user principal name (UPN) of the account to be used for Exchange impersonation.</span></span> 
  
```xml
<PrincipalName/>
```

 <span data-ttu-id="dbadd-105">**PrincipalNameType**</span><span class="sxs-lookup"><span data-stu-id="dbadd-105">**PrincipalNameType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dbadd-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="dbadd-106">Attributes and elements</span></span>

<span data-ttu-id="dbadd-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dbadd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dbadd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="dbadd-108">Attributes</span></span>

<span data-ttu-id="dbadd-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dbadd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dbadd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dbadd-110">Child elements</span></span>

<span data-ttu-id="dbadd-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="dbadd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dbadd-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dbadd-112">Parent elements</span></span>

|<span data-ttu-id="dbadd-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dbadd-113">**Element**</span></span>|<span data-ttu-id="dbadd-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dbadd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbadd-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="dbadd-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="dbadd-116">Representa uma conta a ser representada quando você estiver usando o cabeçalho SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="dbadd-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="dbadd-117">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="dbadd-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dbadd-118">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="dbadd-118">Text value</span></span>

<span data-ttu-id="dbadd-119">O valor de texto representa o UPN de um usuário.</span><span class="sxs-lookup"><span data-stu-id="dbadd-119">The text value represents the UPN of a user.</span></span> <span data-ttu-id="dbadd-120">Esse valor existe no objeto user no serviço de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="dbadd-120">This value exists on the user object in the Active Directory directory service.</span></span> <span data-ttu-id="dbadd-121">Ele contém o nome de logon do usuário e um nome de domínio que identifica o domínio no qual a conta de usuário está localizada, no seguinte formato: `someone@example.com` .</span><span class="sxs-lookup"><span data-stu-id="dbadd-121">This contains the user logon name and a domain name that identifies the domain in which the user account is located, in the following format:  `someone@example.com`.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dbadd-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="dbadd-122">Remarks</span></span>

<span data-ttu-id="dbadd-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="dbadd-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dbadd-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="dbadd-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dbadd-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="dbadd-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dbadd-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dbadd-126">Schema Name</span></span>  <br/> |<span data-ttu-id="dbadd-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="dbadd-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="dbadd-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dbadd-128">Validation File</span></span>  <br/> |<span data-ttu-id="dbadd-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="dbadd-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dbadd-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="dbadd-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="dbadd-131">False</span><span class="sxs-lookup"><span data-stu-id="dbadd-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dbadd-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="dbadd-132">See also</span></span>



- [<span data-ttu-id="dbadd-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="dbadd-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="dbadd-134">Autorização de servidor para servidor no EWS</span><span class="sxs-lookup"><span data-stu-id="dbadd-134">Server-to-server authorization in EWS</span></span>](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

