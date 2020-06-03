---
title: VotingInformation
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 351c8dfe-cf8c-45ba-a07d-d764f8189773
description: O elemento VotingInformation especifica as informações de votação em uma mensagem de votação e uma mensagem de solicitação de aprovação whereApproveandRejectare opções de votação.
ms.openlocfilehash: d946ba8c71d19c8cbb1befbe8c4e43e93590ccae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467743"
---
# <a name="votinginformation"></a><span data-ttu-id="a295c-103">VotingInformation</span><span class="sxs-lookup"><span data-stu-id="a295c-103">VotingInformation</span></span>

<span data-ttu-id="a295c-104">O elemento **VotingInformation** especifica informações de votação em uma mensagem de votação e uma mensagem de solicitação de aprovação onde "aprovar" e "rejeitar" são as opções de votação.</span><span class="sxs-lookup"><span data-stu-id="a295c-104">The **VotingInformation** element specifies voting information on a voting message and approval request message where "Approve" and "Reject" are the voting options.</span></span> 
  
```XML
<VotingInformation
   <UserOptions/>
   <VotingResponse/>
</VotingInformation>
```

 <span data-ttu-id="a295c-105">**VotingInformationType**</span><span class="sxs-lookup"><span data-stu-id="a295c-105">**VotingInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a295c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a295c-106">Attributes and elements</span></span>

<span data-ttu-id="a295c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a295c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a295c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a295c-108">Attributes</span></span>

<span data-ttu-id="a295c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a295c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a295c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a295c-110">Child elements</span></span>

<span data-ttu-id="a295c-111">[UserOptions](useroptions.md)  |  [VotingResponse](votingresponse.md)</span><span class="sxs-lookup"><span data-stu-id="a295c-111">[UserOptions](useroptions.md) | [VotingResponse](votingresponse.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a295c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a295c-112">Parent elements</span></span>

[<span data-ttu-id="a295c-113">Mensagem</span><span class="sxs-lookup"><span data-stu-id="a295c-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="a295c-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="a295c-114">Remarks</span></span>

<span data-ttu-id="a295c-115">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a295c-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="a295c-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a295c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a295c-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a295c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a295c-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="a295c-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a295c-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a295c-119">Schema Name</span></span>  <br/> |<span data-ttu-id="a295c-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a295c-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="a295c-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a295c-121">Validation File</span></span>  <br/> |<span data-ttu-id="a295c-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a295c-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a295c-123">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a295c-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="a295c-124">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="a295c-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a295c-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="a295c-125">See also</span></span>



[<span data-ttu-id="a295c-126">Mensagem</span><span class="sxs-lookup"><span data-stu-id="a295c-126">Message</span></span>](message-ex15websvcsotherref.md)


- [<span data-ttu-id="a295c-127">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a295c-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

