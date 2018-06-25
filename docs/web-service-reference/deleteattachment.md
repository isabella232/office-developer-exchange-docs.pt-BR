---
title: DeleteAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteAttachment
api_type:
- schema
ms.assetid: 43d0c1cb-92ca-4399-9b3a-acb2b5c22624
description: O elemento DeleteAttachment é o elemento raiz em uma solicitação para excluir um anexo do armazenamento do Exchange.
ms.openlocfilehash: 2beedd647febf025f6e3140ec37b196c9aeb7611
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751728"
---
# <a name="deleteattachment"></a><span data-ttu-id="54767-103">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="54767-103">DeleteAttachment</span></span>

<span data-ttu-id="54767-104">O elemento **DeleteAttachment** é o elemento raiz em uma solicitação para excluir um anexo do armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="54767-104">The **DeleteAttachment** element is the root element in a request to delete an attachment from the Exchange store.</span></span> 
  
```xml
<DeleteAttachment>
   <AttachmentIds/>
</DeleteAttachment>
```

<span data-ttu-id="54767-105">**DeleteAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="54767-105">**DeleteAttachmentType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="54767-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="54767-106">Attributes and elements</span></span>

<span data-ttu-id="54767-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="54767-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54767-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="54767-108">Attributes</span></span>

<span data-ttu-id="54767-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="54767-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54767-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="54767-110">Child elements</span></span>

|<span data-ttu-id="54767-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="54767-111">**Element**</span></span>|<span data-ttu-id="54767-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="54767-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54767-113">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="54767-113">AttachmentIds</span></span>](attachmentids.md) <br/> |<span data-ttu-id="54767-114">Contém uma matriz de identificadores de anexos que são usados para excluir os anexos.</span><span class="sxs-lookup"><span data-stu-id="54767-114">Contains an array of attachment identifiers that are used to delete the attachments.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54767-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="54767-115">Parent elements</span></span>

<span data-ttu-id="54767-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="54767-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="54767-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="54767-117">Remarks</span></span>

<span data-ttu-id="54767-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="54767-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54767-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="54767-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54767-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="54767-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="54767-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="54767-121">Schema Name</span></span>  <br/> |<span data-ttu-id="54767-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="54767-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="54767-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="54767-123">Validation File</span></span>  <br/> |<span data-ttu-id="54767-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="54767-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="54767-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="54767-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="54767-126">False</span><span class="sxs-lookup"><span data-stu-id="54767-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54767-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="54767-127">See also</span></span>

- [<span data-ttu-id="54767-128">Operação DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="54767-128">DeleteAttachment operation</span></span>](deleteattachment-operation.md)

