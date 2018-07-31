---
title: ConnectingSID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectingSID
api_type:
- schema
ms.assetid: 56d6aa52-8fa6-4773-9046-44a6f4f5d97c
description: O elemento ConnectingSID representa uma conta para representar quando você estiver usando o cabeçalho SOAP ExchangeImpersonation.
ms.openlocfilehash: a30f11721506989a84f52dd04c328974f4483956
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354334"
---
# <a name="connectingsid"></a><span data-ttu-id="1bbe0-103">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="1bbe0-103">ConnectingSID</span></span>

<span data-ttu-id="1bbe0-104">O elemento **ConnectingSID** representa uma conta para representar quando você estiver usando o cabeçalho SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-104">The **ConnectingSID** element represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span> 
  
- [<span data-ttu-id="1bbe0-105">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="1bbe0-105">ExchangeImpersonation</span></span>](exchangeimpersonation.md) 
- [<span data-ttu-id="1bbe0-106">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="1bbe0-106">ConnectingSID</span></span>](connectingsid.md)
  
```xml
<ConnectingSID>
   <PrincipalName/>
</ConnectingSID>
```

```xml
<ConnectingSID>
   <SmtpAddress/>
</ConnectingSID>
```

```xml
<ConnectingSID>
    <SID/> 
</ConnectingSID>
```

```xml
<ConnectingSID>
   <PrimarySmtpAddress/>
</ConnectingSID>
```

<span data-ttu-id="1bbe0-107">**ConnectingSIDType**</span><span class="sxs-lookup"><span data-stu-id="1bbe0-107">**ConnectingSIDType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1bbe0-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1bbe0-108">Attributes and elements</span></span>

<span data-ttu-id="1bbe0-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1bbe0-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="1bbe0-110">Attributes</span></span>

<span data-ttu-id="1bbe0-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1bbe0-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1bbe0-112">Child elements</span></span>

|<span data-ttu-id="1bbe0-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1bbe0-113">**Element**</span></span>|<span data-ttu-id="1bbe0-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1bbe0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1bbe0-115">PrincipalName</span><span class="sxs-lookup"><span data-stu-id="1bbe0-115">PrincipalName</span></span>](principalname.md) <br/> |<span data-ttu-id="1bbe0-116">Representa o nome de usuário principal (UPN) da conta a ser usada para a representação.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-116">Represents the user principal name (UPN) of the account to use for impersonation.</span></span> <span data-ttu-id="1bbe0-117">Este deve ser o UPN para o domínio em que a conta de usuário existe.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-117">This should be the UPN for the domain where the user account exists.</span></span>  <br/> |
|[<span data-ttu-id="1bbe0-118">SID</span><span class="sxs-lookup"><span data-stu-id="1bbe0-118">SID</span></span>](sid.md) <br/> |<span data-ttu-id="1bbe0-119">Representa o formulário de segurança descritor definition language (SDDL) do identificador de segurança (SID) para a conta a ser usada para representação.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-119">Represents the security descriptor definition language (SDDL) form of the security identifier (SID) for the account to use for impersonation.</span></span>  <br/> |
|[<span data-ttu-id="1bbe0-120">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="1bbe0-120">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="1bbe0-121">Representa o endereço de Simple Mail Transfer Protocol (SMTP) principal da conta a ser usada para a representação do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-121">Represents the primary Simple Mail Transfer Protocol (SMTP) address of the account to use for Exchange impersonation.</span></span> <span data-ttu-id="1bbe0-122">Se o endereço SMTP principal for fornecido, ele será custo uma pesquisa de serviço de diretório do Active Directory extra para obter o SID do usuário.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-122">If the primary SMTP address is supplied, it will cost an extra Active Directory directory service lookup in order to obtain the SID of the user.</span></span> <span data-ttu-id="1bbe0-123">Recomendamos que você use o UPN ou SID se eles estiverem disponíveis.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-123">We recommend that you use the SID or UPN if they are available.</span></span>  <br/> |
|[<span data-ttu-id="1bbe0-124">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="1bbe0-124">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="1bbe0-125">Representa o endereço de Simple Mail Transfer Protocol (SMTP) da conta a ser usada para a representação do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-125">Represents the Simple Mail Transfer Protocol (SMTP) address of the account to use for Exchange Impersonation.</span></span> <span data-ttu-id="1bbe0-126">Se o endereço SMTP for fornecido, ele será custo uma pesquisa do Active Directory extra para obter o SID do usuário.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-126">If the SMTP address is supplied, it will cost an extra Active Directory lookup in order to obtain the SID of the user.</span></span> <span data-ttu-id="1bbe0-127">Recomendamos que você use o UPN ou SID se eles estiverem disponíveis.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-127">We recommend that you use the SID or UPN if they are available.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1bbe0-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1bbe0-128">Parent elements</span></span>

|<span data-ttu-id="1bbe0-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1bbe0-129">**Element**</span></span>|<span data-ttu-id="1bbe0-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1bbe0-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1bbe0-131">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="1bbe0-131">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="1bbe0-132">Usado no cabeçalho de uma solicitação SOAP.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-132">Used in the SOAP header of a request.</span></span> <span data-ttu-id="1bbe0-133">Quando esse elemento estiver presente, o chamador está tentando representar a conta que está contida no elemento **ExchangeImpersonation** .</span><span class="sxs-lookup"><span data-stu-id="1bbe0-133">When this element is present, the caller is trying to impersonate the account that is contained within the **ExchangeImpersonation** element.</span></span>  <br/> <span data-ttu-id="1bbe0-134">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="1bbe0-134">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1bbe0-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="1bbe0-135">Remarks</span></span>

<span data-ttu-id="1bbe0-136">A chamada conta deve ter o **ms-exch-impersonation** direto no servidor de acesso para cliente e o **ms-exch-MayImpersonate** direito em ou o banco de dados de caixa de correio que contém a caixa de correio para representar ou o usuário do Active Directory ou um contato objeto.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-136">The calling account must have the **ms-exch-impersonation** right on the Client Access server and the **ms-exch-MayImpersonate** right on either the mailbox database that contains the mailbox to impersonate or the Active Directory user or contact object.</span></span> 
  
<span data-ttu-id="1bbe0-137">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1bbe0-138">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1bbe0-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1bbe0-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="1bbe0-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1bbe0-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1bbe0-140">Schema name</span></span>  <br/> |<span data-ttu-id="1bbe0-141">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1bbe0-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="1bbe0-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1bbe0-142">Validation file</span></span>  <br/> |<span data-ttu-id="1bbe0-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1bbe0-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1bbe0-144">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="1bbe0-144">Can be empty</span></span>  <br/> |<span data-ttu-id="1bbe0-145">False</span><span class="sxs-lookup"><span data-stu-id="1bbe0-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1bbe0-146">Ver também</span><span class="sxs-lookup"><span data-stu-id="1bbe0-146">See also</span></span>

- [<span data-ttu-id="1bbe0-147">Autorização de servidor-para-servidor no EWS</span><span class="sxs-lookup"><span data-stu-id="1bbe0-147">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

