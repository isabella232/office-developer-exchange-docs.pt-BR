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
description: O elemento UserId identifica um usuário delegado ou um usuário que tem permissões de acesso de pasta.
ms.openlocfilehash: 8e9867f5a8cdd62dd2dae55fbf527595ac14f46d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837981"
---
# <a name="userid"></a><span data-ttu-id="fbdec-103">UserId</span><span class="sxs-lookup"><span data-stu-id="fbdec-103">UserId</span></span>

<span data-ttu-id="fbdec-104">O elemento **UserId** identifica um usuário delegado ou um usuário que tem permissões de acesso de pasta.</span><span class="sxs-lookup"><span data-stu-id="fbdec-104">The **UserId** element identifies a delegate user or a user who has folder access permissions.</span></span> 
  
```xml
<UserId>
   <SID/>
   <PrimarySmtpAddress/>
   <DisplayName/>
   <DistinguishedUser/>
   <ExternalUserIdentity/>
</UserId>
```

 <span data-ttu-id="fbdec-105">**UserIdType**</span><span class="sxs-lookup"><span data-stu-id="fbdec-105">**UserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fbdec-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="fbdec-106">Attributes and elements</span></span>

<span data-ttu-id="fbdec-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fbdec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fbdec-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fbdec-108">Attributes</span></span>

<span data-ttu-id="fbdec-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fbdec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fbdec-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fbdec-110">Child elements</span></span>

|<span data-ttu-id="fbdec-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fbdec-111">**Element**</span></span>|<span data-ttu-id="fbdec-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fbdec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fbdec-113">SID</span><span class="sxs-lookup"><span data-stu-id="fbdec-113">SID</span></span>](sid.md) <br/> |<span data-ttu-id="fbdec-114">Representa o formulário de segurança descritor definition language (SDDL) do identificador de segurança (SID).</span><span class="sxs-lookup"><span data-stu-id="fbdec-114">Represents the security descriptor definition language (SDDL) form of the security identifier (SID).</span></span>  <br/> |
|[<span data-ttu-id="fbdec-115">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="fbdec-115">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="fbdec-116">Representa o endereço de Simple Mail Transfer Protocol (SMTP) principal de uma conta a ser usada para acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="fbdec-116">Represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="fbdec-117">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="fbdec-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="fbdec-118">Define o nome de exibição de uma pasta, contatos, lista de distribuição ou usuário delegado.</span><span class="sxs-lookup"><span data-stu-id="fbdec-118">Defines the display name of a folder, contact, distribution list, or delegate user.</span></span>  <br/> |
|[<span data-ttu-id="fbdec-119">DistinguishedUser</span><span class="sxs-lookup"><span data-stu-id="fbdec-119">DistinguishedUser</span></span>](distinguisheduser.md) <br/> |<span data-ttu-id="fbdec-120">Identifica as contas de usuário anônimo e padrão para acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="fbdec-120">Identifies Anonymous and Default user accounts for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="fbdec-121">ExternalUserIdentity</span><span class="sxs-lookup"><span data-stu-id="fbdec-121">ExternalUserIdentity</span></span>](externaluseridentity.md) <br/> |<span data-ttu-id="fbdec-122">Identifica um usuário delegado externo ou um usuário externo que tem permissões de acesso de pasta.</span><span class="sxs-lookup"><span data-stu-id="fbdec-122">Identifies an external delegate user or an external user who has folder access permissions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fbdec-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fbdec-123">Parent elements</span></span>

|<span data-ttu-id="fbdec-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fbdec-124">**Element**</span></span>|<span data-ttu-id="fbdec-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fbdec-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fbdec-126">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="fbdec-126">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="fbdec-127">Identifica um único representante para adicionar ou atualizar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fbdec-127">Identifies a single delegate to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="fbdec-128">Permissão</span><span class="sxs-lookup"><span data-stu-id="fbdec-128">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="fbdec-129">Define o que um usuário tem acesso a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="fbdec-129">Defines the access that a user has to a folder.</span></span>  <br/> |
|[<span data-ttu-id="fbdec-130">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="fbdec-130">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="fbdec-131">Define o que um usuário tem acesso a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="fbdec-131">Defines the access that a user has to a Calendar folder.</span></span>  <br/> |
|[<span data-ttu-id="fbdec-132">UserIds</span><span class="sxs-lookup"><span data-stu-id="fbdec-132">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="fbdec-133">Contém uma matriz de usuários do representante para obter ou remova a caixa de correio da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="fbdec-133">Contains an array of delegate users to get or remove from a principal's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fbdec-134">Text value</span><span class="sxs-lookup"><span data-stu-id="fbdec-134">Text value</span></span>

<span data-ttu-id="fbdec-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fbdec-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fbdec-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="fbdec-136">Remarks</span></span>

<span data-ttu-id="fbdec-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fbdec-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fbdec-138">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="fbdec-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fbdec-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="fbdec-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fbdec-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fbdec-140">Schema Name</span></span>  <br/> |<span data-ttu-id="fbdec-141">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="fbdec-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="fbdec-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fbdec-142">Validation File</span></span>  <br/> |<span data-ttu-id="fbdec-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fbdec-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fbdec-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fbdec-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="fbdec-145">False</span><span class="sxs-lookup"><span data-stu-id="fbdec-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fbdec-146">Ver também</span><span class="sxs-lookup"><span data-stu-id="fbdec-146">See also</span></span>



[<span data-ttu-id="fbdec-147">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="fbdec-147">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="fbdec-148">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="fbdec-148">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="fbdec-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fbdec-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="fbdec-150">Adicionando representantes</span><span class="sxs-lookup"><span data-stu-id="fbdec-150">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

