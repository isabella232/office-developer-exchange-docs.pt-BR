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
description: O elemento CertPrincipalName especifica o nome principal do certificado SSL (Secure Sockets Layer) necessário para se conectar à organização do Microsoft Exchange Server 2007 usando SSL.
ms.openlocfilehash: fb2a1c8577bce41945b669be56f2a94a2c4dca26
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463339"
---
# <a name="certprincipalname-pox"></a><span data-ttu-id="8c21f-103">CertPrincipalName (POX)</span><span class="sxs-lookup"><span data-stu-id="8c21f-103">CertPrincipalName (POX)</span></span>

<span data-ttu-id="8c21f-104">O elemento **CertPrincipalName** especifica o nome principal do certificado SSL (Secure Sockets Layer) necessário para se conectar à organização do Microsoft Exchange Server 2007 usando SSL.</span><span class="sxs-lookup"><span data-stu-id="8c21f-104">The **CertPrincipalName** element specifies the Secure Sockets Layer (SSL) certificate principal name that is required to connect to the Microsoft Exchange Server 2007 organization by using SSL.</span></span> 
  
[<span data-ttu-id="8c21f-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="8c21f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="8c21f-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="8c21f-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="8c21f-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="8c21f-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="8c21f-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="8c21f-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="8c21f-109">CertPrincipalName (POX)</span><span class="sxs-lookup"><span data-stu-id="8c21f-109">CertPrincipalName (POX)</span></span>](certprincipalname-pox.md)
  
```xml
<CertPrincipalName>none or servername</CertPrinicpalName>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="8c21f-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8c21f-110">Attributes and elements</span></span>

<span data-ttu-id="8c21f-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8c21f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8c21f-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="8c21f-112">Attributes</span></span>

<span data-ttu-id="8c21f-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8c21f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8c21f-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8c21f-114">Child elements</span></span>

<span data-ttu-id="8c21f-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8c21f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8c21f-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8c21f-116">Parent elements</span></span>

|<span data-ttu-id="8c21f-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8c21f-117">**Element**</span></span>|<span data-ttu-id="8c21f-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8c21f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c21f-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="8c21f-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="8c21f-120">Contém as especificações para conectar um cliente ao computador que está executando o Exchange 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="8c21f-120">Contains the specifications for connecting a client to the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8c21f-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="8c21f-121">Text value</span></span>

<span data-ttu-id="8c21f-122">O valor de texto especifica o nome principal do certificado SSL necessário para se conectar à organização do Microsoft Exchange usando SSL.</span><span class="sxs-lookup"><span data-stu-id="8c21f-122">The text value specifies the SSL certificate principal name that is required to connect to the Microsoft Exchange organization by using SSL.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8c21f-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="8c21f-123">Remarks</span></span>

<span data-ttu-id="8c21f-124">Se o elemento **CertPrincipalName** não for especificado, o padrão será definido como MSSTD: Server, onde Server é o valor especificado no elemento [Server (POX)](server-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="8c21f-124">If the **CertPrincipalName** element is not specified, the default is set to msstd:SERVER, where SERVER is the value that is specified in the [Server (POX)](server-pox.md) element.</span></span> <span data-ttu-id="8c21f-125">Por exemplo, se o servidor for especificado como example.com e **CertPrincipalName** for deixado em branco com o [SSL (POX)](ssl-pox.md) ativado, o valor padrão de **CertPrincipalName** seria msstd:example. com.</span><span class="sxs-lookup"><span data-stu-id="8c21f-125">For example, if SERVER is specified as example.com and **CertPrincipalName** is left blank with [SSL (POX)](ssl-pox.md) turned on, the default value of **CertPrincipalName** would be msstd:example.com.</span></span> 
  
<span data-ttu-id="8c21f-126">Se **nenhum** for especificado, o Windows validará o nome principal do certificado de acordo com as informações encontradas no tópico [nomes de entidade de segurança](https://go.microsoft.com/fwlink/?LinkId=93417) no msdn.</span><span class="sxs-lookup"><span data-stu-id="8c21f-126">If **none** is specified, Windows will validate the certificate principal name according to information found in the [Principal Names](https://go.microsoft.com/fwlink/?LinkId=93417) topic on MSDN.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8c21f-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="8c21f-127">See also</span></span>



[<span data-ttu-id="8c21f-128">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="8c21f-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

