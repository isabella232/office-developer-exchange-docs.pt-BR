---
title: AddNewTelUriContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cff8ef19-3e19-4107-9b35-c8a2b87a41bc
description: O elemento AddNewTelUriContactToGroup especifica os dados de entrada para a operação WSDL AddNewTelUriContactToGroup.
ms.openlocfilehash: 151c5b1dab7a3ffc9630fb4e4192b90bd1d4ae38
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464928"
---
# <a name="addnewteluricontacttogroup"></a><span data-ttu-id="b13db-103">AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="b13db-103">AddNewTelUriContactToGroup</span></span>

<span data-ttu-id="b13db-104">O elemento **AddNewTelUriContactToGroup** especifica os dados de entrada para a operação WSDL **AddNewTelUriContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="b13db-104">The **AddNewTelUriContactToGroup** element specifies the input data for the **AddNewTelUriContactToGroup** WSDL operation.</span></span> 
  
```XML
<AddNewTelUriContactToGroup>
   <TelUriAddress/>
   <ImContactSipUriAddress/>
   <ImTelephoneNumber/>
   <GroupId/>
</AddNewTelUriContactToGroup>
```

 <span data-ttu-id="b13db-105">**AddNewTelUriContactToGroupType**</span><span class="sxs-lookup"><span data-stu-id="b13db-105">**AddNewTelUriContactToGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b13db-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b13db-106">Attributes and elements</span></span>

<span data-ttu-id="b13db-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b13db-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b13db-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b13db-108">Attributes</span></span>

<span data-ttu-id="b13db-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b13db-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b13db-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b13db-110">Child elements</span></span>

<span data-ttu-id="b13db-111">[TelUriAddress](teluriaddress.md)  |  [ImContactSipUriAddress](imcontactsipuriaddress.md)  |  [ImTelephoneNumber](imtelephonenumber.md)  |  [GroupId](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="b13db-111">[TelUriAddress](teluriaddress.md) | [ImContactSipUriAddress](imcontactsipuriaddress.md) | [ImTelephoneNumber](imtelephonenumber.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b13db-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b13db-112">Parent elements</span></span>

<span data-ttu-id="b13db-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b13db-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b13db-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="b13db-114">Remarks</span></span>

<span data-ttu-id="b13db-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b13db-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b13db-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b13db-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b13db-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b13db-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b13db-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="b13db-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b13db-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b13db-119">Schema name</span></span>  <br/> |<span data-ttu-id="b13db-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b13db-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b13db-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b13db-121">Validation file</span></span>  <br/> |<span data-ttu-id="b13db-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b13db-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b13db-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b13db-123">Can be empty</span></span>  <br/> |<span data-ttu-id="b13db-124">False</span><span class="sxs-lookup"><span data-stu-id="b13db-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b13db-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="b13db-125">See also</span></span>

- [<span data-ttu-id="b13db-126">Operação AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="b13db-126">AddNewTelUriContactToGroup operation</span></span>](addnewteluricontacttogroup-operation.md)
- [<span data-ttu-id="b13db-127">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b13db-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

