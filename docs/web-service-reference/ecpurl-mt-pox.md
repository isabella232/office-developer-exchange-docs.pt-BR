---
title: EcpUrl-MT (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 5221745b-572c-44a5-afdb-41b58af44971
description: O elemento EcpUrl-MT especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl (POX) para gerar uma URL que possa ser usada para acessar as configurações de controle de mensagens de email de um usuário habilitado para email.
ms.openlocfilehash: 097811add5635bca14c659814652bca244a1398d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458709"
---
# <a name="ecpurl-mt-pox"></a><span data-ttu-id="6bb93-103">EcpUrl-MT (POX)</span><span class="sxs-lookup"><span data-stu-id="6bb93-103">EcpUrl-mt (POX)</span></span>

<span data-ttu-id="6bb93-104">O elemento **EcpUrl-MT** especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para acessar as configurações de controle de mensagens de email de um usuário habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="6bb93-104">The **EcpUrl-mt** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email message tracking settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="6bb93-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="6bb93-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="6bb93-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="6bb93-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="6bb93-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="6bb93-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="6bb93-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="6bb93-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="6bb93-109">EcpUrl-MT (POX)</span><span class="sxs-lookup"><span data-stu-id="6bb93-109">EcpUrl-mt (POX)</span></span>](ecpurl-mt-pox.md)
  
```XML
<EcpUrl-mt/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="6bb93-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6bb93-110">Attributes and elements</span></span>

<span data-ttu-id="6bb93-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6bb93-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6bb93-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="6bb93-112">Attributes</span></span>

<span data-ttu-id="6bb93-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6bb93-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6bb93-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6bb93-114">Child elements</span></span>

<span data-ttu-id="6bb93-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6bb93-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6bb93-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6bb93-116">Parent elements</span></span>

|<span data-ttu-id="6bb93-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6bb93-117">**Element**</span></span>|<span data-ttu-id="6bb93-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6bb93-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6bb93-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="6bb93-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="6bb93-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="6bb93-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6bb93-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="6bb93-121">Text value</span></span>

<span data-ttu-id="6bb93-122">O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para acessar as configurações de controle de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="6bb93-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email tracking settings for the user.</span></span> <span data-ttu-id="6bb93-123">O valor do elemento **EcpUrl-MT** contém parâmetros contidos nos caracteres ' < ' e ' > ' que são substituídos pelo cliente, conforme mostrado na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="6bb93-123">The value of the **EcpUrl-mt** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="6bb93-124">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="6bb93-124">**Parameter**</span></span>|<span data-ttu-id="6bb93-125">**Substituir por**</span><span class="sxs-lookup"><span data-stu-id="6bb93-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="6bb93-126">_IsOwa_</span><span class="sxs-lookup"><span data-stu-id="6bb93-126">_IsOwa_</span></span> <br/> |<span data-ttu-id="6bb93-127">n</span><span class="sxs-lookup"><span data-stu-id="6bb93-127">n</span></span>  <br/> |
| <span data-ttu-id="6bb93-128">_MsgID_</span><span class="sxs-lookup"><span data-stu-id="6bb93-128">_MsgID_</span></span> <br/> |<span data-ttu-id="6bb93-129">Identificador de mensagem da Internet da mensagem a ser rastreada conforme especificado pelo cabeçalho Message-ID.</span><span class="sxs-lookup"><span data-stu-id="6bb93-129">Internet message identifier of the message to be tracked as specified by the Message-ID header.</span></span>  <br/> |
| <span data-ttu-id="6bb93-130">_MBX_</span><span class="sxs-lookup"><span data-stu-id="6bb93-130">_Mbx_</span></span> <br/> |<span data-ttu-id="6bb93-131">O endereço SMTP do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6bb93-131">The SMTP address of the mailbox owner.</span></span>  <br/> |
| <span data-ttu-id="6bb93-132">_Sender_</span><span class="sxs-lookup"><span data-stu-id="6bb93-132">_Sender_</span></span> <br/> |<span data-ttu-id="6bb93-133">O endereço SMTP do remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="6bb93-133">The SMTP address of the message's sender.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6bb93-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="6bb93-134">Remarks</span></span>

<span data-ttu-id="6bb93-135">O elemento **EcpUrl-MT** é um elemento filho opcional do elemento **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="6bb93-135">The **EcpUrl-mt** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="6bb93-136">Também consulte</span><span class="sxs-lookup"><span data-stu-id="6bb93-136">See also</span></span>



[<span data-ttu-id="6bb93-137">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="6bb93-137">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

