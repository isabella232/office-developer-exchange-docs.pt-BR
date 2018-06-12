---
title: CertPrincipalName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a24092c9-58be-4008-92c4-68ec5c6c0fa6
description: O elemento CertPrincipalName Especifica o nome principal do certificado Secure Sockets Layer (SSL) que é necessária para conectar-se para a organização do Microsoft Exchange Server 2007 usando SSL.
ms.openlocfilehash: d2766b16a3e8a1bcd013de332d9c07f709fcf949
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751386"
---
# <a name="certprincipalname-pox"></a><span data-ttu-id="8abe4-103">CertPrincipalName (POX)</span><span class="sxs-lookup"><span data-stu-id="8abe4-103">CertPrincipalName (POX)</span></span>

<span data-ttu-id="8abe4-104">O elemento **CertPrincipalName** Especifica o nome principal do certificado Secure Sockets Layer (SSL) que é necessária para conectar-se para a organização do Microsoft Exchange Server 2007 usando SSL.</span><span class="sxs-lookup"><span data-stu-id="8abe4-104">The **CertPrincipalName** element specifies the Secure Sockets Layer (SSL) certificate principal name that is required to connect to the Microsoft Exchange Server 2007 organization by using SSL.</span></span> 
  
[<span data-ttu-id="8abe4-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="8abe4-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="8abe4-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="8abe4-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="8abe4-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="8abe4-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="8abe4-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="8abe4-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="8abe4-109">CertPrincipalName (POX)</span><span class="sxs-lookup"><span data-stu-id="8abe4-109">CertPrincipalName (POX)</span></span>](certprincipalname-pox.md)
  
```xml
<CertPrincipalName>none or servername</CertPrinicpalName>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="8abe4-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8abe4-110">Attributes and elements</span></span>

<span data-ttu-id="8abe4-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8abe4-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8abe4-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="8abe4-112">Attributes</span></span>

<span data-ttu-id="8abe4-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8abe4-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8abe4-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8abe4-114">Child elements</span></span>

<span data-ttu-id="8abe4-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8abe4-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8abe4-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8abe4-116">Parent elements</span></span>

|<span data-ttu-id="8abe4-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8abe4-117">**Element**</span></span>|<span data-ttu-id="8abe4-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8abe4-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8abe4-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="8abe4-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="8abe4-120">Contém as especificações para conectar um cliente para o computador que está executando o Exchange 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="8abe4-120">Contains the specifications for connecting a client to the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8abe4-121">Text value</span><span class="sxs-lookup"><span data-stu-id="8abe4-121">Text value</span></span>

<span data-ttu-id="8abe4-122">O valor de texto Especifica o nome principal do certificado SSL que é necessária para conectar-se à organização do Microsoft Exchange usando SSL.</span><span class="sxs-lookup"><span data-stu-id="8abe4-122">The text value specifies the SSL certificate principal name that is required to connect to the Microsoft Exchange organization by using SSL.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8abe4-123">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="8abe4-123">Remarks</span></span>

<span data-ttu-id="8abe4-124">Se o elemento **CertPrincipalName** não for especificado, o padrão é definido como msstd:SERVER, em que servidor é o valor especificado no elemento [Server POX ()](server-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="8abe4-124">If the **CertPrincipalName** element is not specified, the default is set to msstd:SERVER, where SERVER is the value that is specified in the [Server (POX)](server-pox.md) element.</span></span> <span data-ttu-id="8abe4-125">Por exemplo, se o servidor é especificado como example.com e **CertPrincipalName** for deixado em branco com [SSL (POX)](ssl-pox.md) ativado, o valor padrão de **CertPrincipalName** seria msstd:example.com.</span><span class="sxs-lookup"><span data-stu-id="8abe4-125">For example, if SERVER is specified as example.com and **CertPrincipalName** is left blank with [SSL (POX)](ssl-pox.md) turned on, the default value of **CertPrincipalName** would be msstd:example.com.</span></span> 
  
<span data-ttu-id="8abe4-126">Se **Nenhum** for especificado, o Windows validará o nome principal do certificado de acordo com a informação encontrada no tópico [Nomes de entidade](http://go.microsoft.com/fwlink/?LinkId=93417) no MSDN.</span><span class="sxs-lookup"><span data-stu-id="8abe4-126">If **none** is specified, Windows will validate the certificate principal name according to information found in the [Principal Names](http://go.microsoft.com/fwlink/?LinkId=93417) topic on MSDN.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8abe4-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="8abe4-127">See also</span></span>



[<span data-ttu-id="8abe4-128">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="8abe4-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

