---
title: AddDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegateResponse
api_type:
- schema
ms.assetid: d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429
description: O elemento AddDelegateResponse contém o status e o resultado de uma solicitação de operação AddDelegate.
ms.openlocfilehash: 1c38563ab38facf89fd5eab119542374949244c2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466455"
---
# <a name="adddelegateresponse"></a><span data-ttu-id="cec36-103">AddDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="cec36-103">AddDelegateResponse</span></span>

<span data-ttu-id="cec36-104">O elemento **AddDelegateResponse** contém o status e o resultado de uma solicitação de [operação AddDelegate](adddelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="cec36-104">The **AddDelegateResponse** element contains the status and result of an [AddDelegate operation](adddelegate-operation.md) request.</span></span> 
  
```xml
<AddDelegateResponse>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</AddDelegateResponse>
```

 <span data-ttu-id="cec36-105">**AddDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="cec36-105">**AddDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cec36-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cec36-106">Attributes and elements</span></span>

<span data-ttu-id="cec36-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cec36-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cec36-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cec36-108">Attributes</span></span>

<span data-ttu-id="cec36-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cec36-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cec36-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cec36-110">Child elements</span></span>

|<span data-ttu-id="cec36-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cec36-111">**Element**</span></span>|<span data-ttu-id="cec36-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cec36-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cec36-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="cec36-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="cec36-114">Contém as mensagens de resposta para uma solicitação de gerenciamento de representante do Exchange Web Services.</span><span class="sxs-lookup"><span data-stu-id="cec36-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="cec36-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="cec36-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="cec36-116">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="cec36-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="cec36-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cec36-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="cec36-118">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="cec36-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="cec36-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="cec36-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="cec36-120">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="cec36-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="cec36-121">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="cec36-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="cec36-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="cec36-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="cec36-123">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="cec36-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cec36-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cec36-124">Parent elements</span></span>

<span data-ttu-id="cec36-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cec36-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cec36-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="cec36-126">Remarks</span></span>

<span data-ttu-id="cec36-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="cec36-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cec36-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cec36-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cec36-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="cec36-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cec36-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cec36-130">Schema Name</span></span>  <br/> |<span data-ttu-id="cec36-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="cec36-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cec36-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cec36-132">Validation File</span></span>  <br/> |<span data-ttu-id="cec36-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cec36-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cec36-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cec36-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="cec36-135">False</span><span class="sxs-lookup"><span data-stu-id="cec36-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cec36-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="cec36-136">See also</span></span>

- [<span data-ttu-id="cec36-137">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="cec36-137">AddDelegate operation</span></span>](adddelegate-operation.md)
- [<span data-ttu-id="cec36-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cec36-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="cec36-139">Adicionar representantes</span><span class="sxs-lookup"><span data-stu-id="cec36-139">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

