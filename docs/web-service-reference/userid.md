---
title: UserId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserId
api_type:
- schema
ms.assetid: 244af9e0-bf3c-46b4-8bfa-9719a1ed3107
description: O elemento UserId identifica um usuário delegado ou um usuário com permissões de acesso à pasta.
ms.openlocfilehash: 68075e335383835ddce9575d85ba5fa945ed305c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455538"
---
# <a name="userid"></a><span data-ttu-id="c35a5-103">UserId</span><span class="sxs-lookup"><span data-stu-id="c35a5-103">UserId</span></span>

<span data-ttu-id="c35a5-104">O elemento **userid** identifica um usuário delegado ou um usuário com permissões de acesso à pasta.</span><span class="sxs-lookup"><span data-stu-id="c35a5-104">The **UserId** element identifies a delegate user or a user who has folder access permissions.</span></span> 
  
```xml
<UserId>
   <SID/>
   <PrimarySmtpAddress/>
   <DisplayName/>
   <DistinguishedUser/>
   <ExternalUserIdentity/>
</UserId>
```

 <span data-ttu-id="c35a5-105">**UserIdtype**</span><span class="sxs-lookup"><span data-stu-id="c35a5-105">**UserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c35a5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c35a5-106">Attributes and elements</span></span>

<span data-ttu-id="c35a5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c35a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c35a5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c35a5-108">Attributes</span></span>

<span data-ttu-id="c35a5-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c35a5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c35a5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c35a5-110">Child elements</span></span>

|<span data-ttu-id="c35a5-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c35a5-111">**Element**</span></span>|<span data-ttu-id="c35a5-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c35a5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c35a5-113">Identifica</span><span class="sxs-lookup"><span data-stu-id="c35a5-113">SID</span></span>](sid.md) <br/> |<span data-ttu-id="c35a5-114">Representa a forma SDDL (Security Descriptor Definition Language) do identificador de segurança (SID).</span><span class="sxs-lookup"><span data-stu-id="c35a5-114">Represents the security descriptor definition language (SDDL) form of the security identifier (SID).</span></span>  <br/> |
|[<span data-ttu-id="c35a5-115">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="c35a5-115">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="c35a5-116">Representa o endereço SMTP (Simple Mail Transfer Protocol) principal de uma conta a ser usada para acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="c35a5-116">Represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="c35a5-117">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="c35a5-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="c35a5-118">Define o nome de exibição de uma pasta, contato, lista de distribuição ou usuário delegado.</span><span class="sxs-lookup"><span data-stu-id="c35a5-118">Defines the display name of a folder, contact, distribution list, or delegate user.</span></span>  <br/> |
|[<span data-ttu-id="c35a5-119">DistinguishedUser</span><span class="sxs-lookup"><span data-stu-id="c35a5-119">DistinguishedUser</span></span>](distinguisheduser.md) <br/> |<span data-ttu-id="c35a5-120">Identifica contas de usuário anônimas e padrão para acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="c35a5-120">Identifies Anonymous and Default user accounts for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="c35a5-121">ExternalUserIdentity</span><span class="sxs-lookup"><span data-stu-id="c35a5-121">ExternalUserIdentity</span></span>](externaluseridentity.md) <br/> |<span data-ttu-id="c35a5-122">Identifica um usuário delegado externo ou um usuário externo com permissões de acesso de pasta.</span><span class="sxs-lookup"><span data-stu-id="c35a5-122">Identifies an external delegate user or an external user who has folder access permissions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c35a5-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c35a5-123">Parent elements</span></span>

|<span data-ttu-id="c35a5-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c35a5-124">**Element**</span></span>|<span data-ttu-id="c35a5-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c35a5-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c35a5-126">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="c35a5-126">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="c35a5-127">Identifica um único representante para adicionar ou atualizar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c35a5-127">Identifies a single delegate to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c35a5-128">Permissão</span><span class="sxs-lookup"><span data-stu-id="c35a5-128">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="c35a5-129">Define o acesso que um usuário tem a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="c35a5-129">Defines the access that a user has to a folder.</span></span>  <br/> |
|[<span data-ttu-id="c35a5-130">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="c35a5-130">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="c35a5-131">Define o acesso que um usuário tem a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="c35a5-131">Defines the access that a user has to a Calendar folder.</span></span>  <br/> |
|[<span data-ttu-id="c35a5-132">UserIds</span><span class="sxs-lookup"><span data-stu-id="c35a5-132">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="c35a5-133">Contém uma matriz de usuários delegados para obter ou remover da caixa de correio de uma entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="c35a5-133">Contains an array of delegate users to get or remove from a principal's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c35a5-134">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c35a5-134">Text value</span></span>

<span data-ttu-id="c35a5-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c35a5-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c35a5-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="c35a5-136">Remarks</span></span>

<span data-ttu-id="c35a5-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c35a5-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c35a5-138">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c35a5-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c35a5-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="c35a5-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c35a5-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c35a5-140">Schema Name</span></span>  <br/> |<span data-ttu-id="c35a5-141">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c35a5-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="c35a5-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c35a5-142">Validation File</span></span>  <br/> |<span data-ttu-id="c35a5-143">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c35a5-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c35a5-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c35a5-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="c35a5-145">False</span><span class="sxs-lookup"><span data-stu-id="c35a5-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c35a5-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="c35a5-146">See also</span></span>



[<span data-ttu-id="c35a5-147">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="c35a5-147">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="c35a5-148">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="c35a5-148">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="c35a5-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c35a5-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="c35a5-150">Adicionar representantes</span><span class="sxs-lookup"><span data-stu-id="c35a5-150">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

