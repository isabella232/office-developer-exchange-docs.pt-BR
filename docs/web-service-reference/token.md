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
description: O elemento de Token contém os dados criptografados que representa o token de identificação para os dados compartilhados.
ms.openlocfilehash: cec11d9f2c24a250483c5be6e273f981fdf0a8e6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837769"
---
# <a name="token"></a><span data-ttu-id="8ddbc-103">Token</span><span class="sxs-lookup"><span data-stu-id="8ddbc-103">Token</span></span>

<span data-ttu-id="8ddbc-104">O elemento **Token** contém os dados criptografados que representa o token de identificação para os dados compartilhados.</span><span class="sxs-lookup"><span data-stu-id="8ddbc-104">The **Token** element contains encrypted data that represents the identification token for the shared data.</span></span> 
  
```xml
<Token/>
```

 <span data-ttu-id="8ddbc-105">**EncryptedDataContainerType**</span><span class="sxs-lookup"><span data-stu-id="8ddbc-105">**EncryptedDataContainerType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8ddbc-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8ddbc-106">Attributes and elements</span></span>

<span data-ttu-id="8ddbc-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8ddbc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ddbc-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8ddbc-108">Attributes</span></span>

<span data-ttu-id="8ddbc-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8ddbc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ddbc-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8ddbc-110">Child elements</span></span>

<span data-ttu-id="8ddbc-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8ddbc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8ddbc-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8ddbc-112">Parent elements</span></span>

|<span data-ttu-id="8ddbc-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8ddbc-113">**Element**</span></span>|<span data-ttu-id="8ddbc-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8ddbc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ddbc-115">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="8ddbc-115">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md) <br/> |<span data-ttu-id="8ddbc-116">Contém os dados criptografados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou entre em contato com o serviço de dados com outros clientes.</span><span class="sxs-lookup"><span data-stu-id="8ddbc-116">Contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8ddbc-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="8ddbc-117">Remarks</span></span>

<span data-ttu-id="8ddbc-118">O esquema que descreve este elemento está localizado no diretório Virtual do IIS que hospeda o Exchange Web Services do computador que está executando o Microsoft Exchange Server que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="8ddbc-118">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8ddbc-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8ddbc-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ddbc-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="8ddbc-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8ddbc-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8ddbc-121">Schema Name</span></span>  <br/> |<span data-ttu-id="8ddbc-122">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8ddbc-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="8ddbc-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8ddbc-123">Validation File</span></span>  <br/> |<span data-ttu-id="8ddbc-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8ddbc-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8ddbc-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8ddbc-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="8ddbc-126">False</span><span class="sxs-lookup"><span data-stu-id="8ddbc-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8ddbc-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="8ddbc-127">See also</span></span>



[<span data-ttu-id="8ddbc-128">Operação GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="8ddbc-128">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="8ddbc-129">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8ddbc-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

