---
title: VotingInformation
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 351c8dfe-cf8c-45ba-a07d-d764f8189773
description: O elemento VotingInformation Especifica informações votação em uma mensagem de votação e whereApproveandRejectare de mensagem de solicitação de aprovação, as opções de votação.
ms.openlocfilehash: f11c25bb1f3a3c4781cfa6c51e11ff87af40c7f0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838038"
---
# <a name="votinginformation"></a><span data-ttu-id="a1313-103">VotingInformation</span><span class="sxs-lookup"><span data-stu-id="a1313-103">VotingInformation</span></span>

<span data-ttu-id="a1313-104">O elemento **VotingInformation** Especifica as informações de votação em uma mensagem de votação e a mensagem de solicitação de aprovação onde "Approve" e "Rejeitar" é as opções de votação.</span><span class="sxs-lookup"><span data-stu-id="a1313-104">The **VotingInformation** element specifies voting information on a voting message and approval request message where "Approve" and "Reject" are the voting options.</span></span> 
  
```XML
<VotingInformation
   <UserOptions/>
   <VotingResponse/>
</VotingInformation>
```

 <span data-ttu-id="a1313-105">**VotingInformationType**</span><span class="sxs-lookup"><span data-stu-id="a1313-105">**VotingInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a1313-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a1313-106">Attributes and elements</span></span>

<span data-ttu-id="a1313-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a1313-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1313-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a1313-108">Attributes</span></span>

<span data-ttu-id="a1313-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a1313-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1313-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a1313-110">Child elements</span></span>

<span data-ttu-id="a1313-111">[UserOptions](useroptions.md) | [VotingResponse](votingresponse.md)</span><span class="sxs-lookup"><span data-stu-id="a1313-111">[UserOptions](useroptions.md) | [VotingResponse](votingresponse.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a1313-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a1313-112">Parent elements</span></span>

[<span data-ttu-id="a1313-113">Mensagem</span><span class="sxs-lookup"><span data-stu-id="a1313-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="a1313-114">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="a1313-114">Remarks</span></span>

<span data-ttu-id="a1313-115">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a1313-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="a1313-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1313-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1313-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a1313-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1313-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="a1313-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a1313-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a1313-119">Schema Name</span></span>  <br/> |<span data-ttu-id="a1313-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a1313-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="a1313-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a1313-121">Validation File</span></span>  <br/> |<span data-ttu-id="a1313-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a1313-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a1313-123">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a1313-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="a1313-124">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="a1313-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1313-125">Ver também</span><span class="sxs-lookup"><span data-stu-id="a1313-125">See also</span></span>



[<span data-ttu-id="a1313-126">Mensagem</span><span class="sxs-lookup"><span data-stu-id="a1313-126">Message</span></span>](message-ex15websvcsotherref.md)


- [<span data-ttu-id="a1313-127">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a1313-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

