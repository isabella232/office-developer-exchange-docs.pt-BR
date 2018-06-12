---
title: EncryptedSharedFolderDataCollection
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EncryptedSharedFolderDataCollection
api_type:
- schema
ms.assetid: 25c6ae87-bbb9-4dd5-a85a-d669fcea137f
description: O elemento EncryptedSharedFolderDataCollection contém uma coleção de estruturas de dados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou entre em contato com o serviço de dados com outros clientes.
ms.openlocfilehash: e4d37f5df10f5e270be5126479485239f2205d6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752041"
---
# <a name="encryptedsharedfolderdatacollection"></a><span data-ttu-id="3bcf4-103">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="3bcf4-103">EncryptedSharedFolderDataCollection</span></span>

<span data-ttu-id="3bcf4-104">O elemento **EncryptedSharedFolderDataCollection** contém uma coleção de estruturas de dados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou entre em contato com o serviço de dados com outros clientes.</span><span class="sxs-lookup"><span data-stu-id="3bcf4-104">The **EncryptedSharedFolderDataCollection** element contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderDataCollection>   <EncryptedSharedFolderData/></EncryptedSharedFolderDataCollection>
```

 <span data-ttu-id="3bcf4-105">**ArrayOfEncryptedSharedFolderDataType**</span><span class="sxs-lookup"><span data-stu-id="3bcf4-105">**ArrayOfEncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3bcf4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3bcf4-106">Attributes and elements</span></span>

<span data-ttu-id="3bcf4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3bcf4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3bcf4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3bcf4-108">Attributes</span></span>

<span data-ttu-id="3bcf4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3bcf4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3bcf4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3bcf4-110">Child elements</span></span>

|<span data-ttu-id="3bcf4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3bcf4-111">**Element**</span></span>|<span data-ttu-id="3bcf4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3bcf4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3bcf4-113">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="3bcf4-113">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md) <br/> |<span data-ttu-id="3bcf4-114">Contém os dados criptografados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou entre em contato com o serviço de dados com outros clientes.</span><span class="sxs-lookup"><span data-stu-id="3bcf4-114">Contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3bcf4-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3bcf4-115">Parent elements</span></span>

|<span data-ttu-id="3bcf4-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3bcf4-116">**Element**</span></span>|<span data-ttu-id="3bcf4-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3bcf4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3bcf4-118">GetSharingMetadataResponse</span><span class="sxs-lookup"><span data-stu-id="3bcf4-118">GetSharingMetadataResponse</span></span>](getsharingmetadataresponse.md) <br/> |<span data-ttu-id="3bcf4-119">Define uma resposta a uma solicitação de [operação GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="3bcf4-119">Defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="3bcf4-120">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3bcf4-120">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md) <br/> |<span data-ttu-id="3bcf4-121">Contém o status e o resultado de uma única solicitação de [operação GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="3bcf4-121">Contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3bcf4-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="3bcf4-122">Remarks</span></span>

<span data-ttu-id="3bcf4-123">O esquema que descreve este elemento está localizado no diretório Virtual do IIS que hospeda o Exchange Web Services do computador que está executando o Microsoft Exchange Server que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="3bcf4-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3bcf4-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3bcf4-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3bcf4-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="3bcf4-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3bcf4-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3bcf4-126">Schema Name</span></span>  <br/> |<span data-ttu-id="3bcf4-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3bcf4-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3bcf4-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3bcf4-128">Validation File</span></span>  <br/> |<span data-ttu-id="3bcf4-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3bcf4-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3bcf4-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3bcf4-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="3bcf4-131">False</span><span class="sxs-lookup"><span data-stu-id="3bcf4-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3bcf4-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="3bcf4-132">See also</span></span>

- [<span data-ttu-id="3bcf4-133">Operação GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="3bcf4-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="3bcf4-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3bcf4-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

