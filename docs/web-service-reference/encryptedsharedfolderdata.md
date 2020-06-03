---
title: EncryptedSharedFolderData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EncryptedSharedFolderData
api_type:
- schema
ms.assetid: c1d4ca18-c5ce-41ff-bab4-f75e358c8b9f
description: O elemento EncryptedSharedFolderData contém os dados criptografados que um cliente pode usar para autorizar o compartilhamento de seus dados de calendário ou de contato com outros clientes.
ms.openlocfilehash: 52e91eaf1ded31602b11e50c1b62159f72c101cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530660"
---
# <a name="encryptedsharedfolderdata"></a><span data-ttu-id="e2657-103">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="e2657-103">EncryptedSharedFolderData</span></span>

<span data-ttu-id="e2657-104">O elemento **EncryptedSharedFolderData** contém os dados criptografados que um cliente pode usar para autorizar o compartilhamento de seus dados de calendário ou de contato com outros clientes.</span><span class="sxs-lookup"><span data-stu-id="e2657-104">The **EncryptedSharedFolderData** element contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderData>   <Token/>   <Data/></EncryptedSharedFolderData>
```

 <span data-ttu-id="e2657-105">**EncryptedSharedFolderDataType**</span><span class="sxs-lookup"><span data-stu-id="e2657-105">**EncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2657-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e2657-106">Attributes and elements</span></span>

<span data-ttu-id="e2657-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e2657-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2657-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e2657-108">Attributes</span></span>

<span data-ttu-id="e2657-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2657-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2657-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e2657-110">Child elements</span></span>

|<span data-ttu-id="e2657-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e2657-111">**Element**</span></span>|<span data-ttu-id="e2657-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e2657-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2657-113">Token</span><span class="sxs-lookup"><span data-stu-id="e2657-113">Token</span></span>](token.md) <br/> |<span data-ttu-id="e2657-114">Contém dados criptografados que representam o token de identificação para os dados compartilhados.</span><span class="sxs-lookup"><span data-stu-id="e2657-114">Contains encrypted data that represents the identification token for the shared data.</span></span>  <br/> |
|[<span data-ttu-id="e2657-115">Dados</span><span class="sxs-lookup"><span data-stu-id="e2657-115">Data</span></span>](data.md) <br/> |<span data-ttu-id="e2657-116">Contém dados criptografados que representam os dados compartilhados.</span><span class="sxs-lookup"><span data-stu-id="e2657-116">Contains encrypted data that represents the shared data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e2657-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e2657-117">Parent elements</span></span>

|<span data-ttu-id="e2657-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e2657-118">**Element**</span></span>|<span data-ttu-id="e2657-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e2657-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2657-120">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="e2657-120">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="e2657-121">Representa uma coleção de estruturas de dados que um cliente pode usar para autorizar o compartilhamento de seus dados de calendário ou de contato com outros clientes.</span><span class="sxs-lookup"><span data-stu-id="e2657-121">Represents a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e2657-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="e2657-122">Remarks</span></span>

<span data-ttu-id="e2657-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="e2657-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2657-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e2657-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2657-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="e2657-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e2657-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e2657-126">Schema Name</span></span>  <br/> |<span data-ttu-id="e2657-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e2657-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="e2657-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e2657-128">Validation File</span></span>  <br/> |<span data-ttu-id="e2657-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e2657-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e2657-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e2657-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="e2657-131">False</span><span class="sxs-lookup"><span data-stu-id="e2657-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2657-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="e2657-132">See also</span></span>

- [<span data-ttu-id="e2657-133">Operação GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="e2657-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="e2657-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e2657-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

