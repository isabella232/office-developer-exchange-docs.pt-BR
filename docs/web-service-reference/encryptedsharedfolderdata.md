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
description: O elemento EncryptedSharedFolderData contém os dados criptografados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou entre em contato com o serviço de dados com outros clientes.
ms.openlocfilehash: 63966e95becaab4b3b1e54aa81f1b20a8b09dfd3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752043"
---
# <a name="encryptedsharedfolderdata"></a><span data-ttu-id="700ec-103">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="700ec-103">EncryptedSharedFolderData</span></span>

<span data-ttu-id="700ec-104">O elemento **EncryptedSharedFolderData** contém os dados criptografados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou entre em contato com o serviço de dados com outros clientes.</span><span class="sxs-lookup"><span data-stu-id="700ec-104">The **EncryptedSharedFolderData** element contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderData>   <Token/>   <Data/></EncryptedSharedFolderData>
```

 <span data-ttu-id="700ec-105">**EncryptedSharedFolderDataType**</span><span class="sxs-lookup"><span data-stu-id="700ec-105">**EncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="700ec-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="700ec-106">Attributes and elements</span></span>

<span data-ttu-id="700ec-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="700ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="700ec-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="700ec-108">Attributes</span></span>

<span data-ttu-id="700ec-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="700ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="700ec-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="700ec-110">Child elements</span></span>

|<span data-ttu-id="700ec-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="700ec-111">**Element**</span></span>|<span data-ttu-id="700ec-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="700ec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="700ec-113">Token</span><span class="sxs-lookup"><span data-stu-id="700ec-113">Token</span></span>](token.md) <br/> |<span data-ttu-id="700ec-114">Contém os dados criptografados que representa o token de identificação para os dados compartilhados.</span><span class="sxs-lookup"><span data-stu-id="700ec-114">Contains encrypted data that represents the identification token for the shared data.</span></span>  <br/> |
|[<span data-ttu-id="700ec-115">Data</span><span class="sxs-lookup"><span data-stu-id="700ec-115">Data</span></span>](data.md) <br/> |<span data-ttu-id="700ec-116">Contém os dados criptografados que representa os dados compartilhados.</span><span class="sxs-lookup"><span data-stu-id="700ec-116">Contains encrypted data that represents the shared data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="700ec-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="700ec-117">Parent elements</span></span>

|<span data-ttu-id="700ec-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="700ec-118">**Element**</span></span>|<span data-ttu-id="700ec-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="700ec-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="700ec-120">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="700ec-120">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="700ec-121">Representa uma coleção de estruturas de dados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou entre em contato com o serviço de dados com outros clientes.</span><span class="sxs-lookup"><span data-stu-id="700ec-121">Represents a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="700ec-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="700ec-122">Remarks</span></span>

<span data-ttu-id="700ec-123">O esquema que descreve este elemento está localizado no diretório Virtual do IIS que hospeda o Exchange Web Services do computador que está executando o Microsoft Exchange Server que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="700ec-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="700ec-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="700ec-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="700ec-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="700ec-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="700ec-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="700ec-126">Schema Name</span></span>  <br/> |<span data-ttu-id="700ec-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="700ec-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="700ec-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="700ec-128">Validation File</span></span>  <br/> |<span data-ttu-id="700ec-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="700ec-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="700ec-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="700ec-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="700ec-131">False</span><span class="sxs-lookup"><span data-stu-id="700ec-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="700ec-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="700ec-132">See also</span></span>

- [<span data-ttu-id="700ec-133">Operação GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="700ec-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="700ec-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="700ec-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

