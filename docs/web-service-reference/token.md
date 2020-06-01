---
title: Token
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Token
api_type:
- schema
ms.assetid: 62b700e1-88c7-41ef-b431-d7af4a8b54a7
description: O elemento token contém dados criptografados que representam o token de identificação para os dados compartilhados.
ms.openlocfilehash: c2e80082f9b4ecb96defdca8c5f0223a945661ba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458905"
---
# <a name="token"></a><span data-ttu-id="419d5-103">Token</span><span class="sxs-lookup"><span data-stu-id="419d5-103">Token</span></span>

<span data-ttu-id="419d5-104">O elemento **token** contém dados criptografados que representam o token de identificação para os dados compartilhados.</span><span class="sxs-lookup"><span data-stu-id="419d5-104">The **Token** element contains encrypted data that represents the identification token for the shared data.</span></span> 
  
```xml
<Token/>
```

 <span data-ttu-id="419d5-105">**EncryptedDataContainerType**</span><span class="sxs-lookup"><span data-stu-id="419d5-105">**EncryptedDataContainerType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="419d5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="419d5-106">Attributes and elements</span></span>

<span data-ttu-id="419d5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="419d5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="419d5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="419d5-108">Attributes</span></span>

<span data-ttu-id="419d5-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="419d5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="419d5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="419d5-110">Child elements</span></span>

<span data-ttu-id="419d5-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="419d5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="419d5-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="419d5-112">Parent elements</span></span>

|<span data-ttu-id="419d5-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="419d5-113">**Element**</span></span>|<span data-ttu-id="419d5-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="419d5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="419d5-115">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="419d5-115">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md) <br/> |<span data-ttu-id="419d5-116">Contém os dados criptografados que um cliente pode usar para autorizar o compartilhamento de seus dados de calendário ou de contato com outros clientes.</span><span class="sxs-lookup"><span data-stu-id="419d5-116">Contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="419d5-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="419d5-117">Remarks</span></span>

<span data-ttu-id="419d5-118">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="419d5-118">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="419d5-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="419d5-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="419d5-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="419d5-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="419d5-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="419d5-121">Schema Name</span></span>  <br/> |<span data-ttu-id="419d5-122">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="419d5-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="419d5-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="419d5-123">Validation File</span></span>  <br/> |<span data-ttu-id="419d5-124">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="419d5-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="419d5-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="419d5-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="419d5-126">False</span><span class="sxs-lookup"><span data-stu-id="419d5-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="419d5-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="419d5-127">See also</span></span>



[<span data-ttu-id="419d5-128">Operação GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="419d5-128">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="419d5-129">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="419d5-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

