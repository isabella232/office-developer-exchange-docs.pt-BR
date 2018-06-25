---
title: EcpUrl-mt POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 5221745b-572c-44a5-afdb-41b58af44971
description: O elemento EcpUrl-mt Especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl POX () para gerar uma URL que pode ser usada para acessar as configurações para um usuário habilitado para email de acompanhamento de mensagens de email.
ms.openlocfilehash: 13954a4dab8e81f4ba75b3578e6ba7f67f4b8b96
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751944"
---
# <a name="ecpurl-mt-pox"></a><span data-ttu-id="70856-103">EcpUrl-mt POX)</span><span class="sxs-lookup"><span data-stu-id="70856-103">EcpUrl-mt (POX)</span></span>

<span data-ttu-id="70856-104">O elemento **EcpUrl-mt** Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar as configurações para um usuário habilitado para email de acompanhamento de mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="70856-104">The **EcpUrl-mt** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email message tracking settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="70856-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="70856-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="70856-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="70856-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="70856-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="70856-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="70856-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="70856-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="70856-109">EcpUrl-mt POX)</span><span class="sxs-lookup"><span data-stu-id="70856-109">EcpUrl-mt (POX)</span></span>](ecpurl-mt-pox.md)
  
```XML
<EcpUrl-mt/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="70856-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="70856-110">Attributes and elements</span></span>

<span data-ttu-id="70856-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="70856-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70856-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="70856-112">Attributes</span></span>

<span data-ttu-id="70856-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="70856-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70856-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="70856-114">Child elements</span></span>

<span data-ttu-id="70856-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="70856-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="70856-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="70856-116">Parent elements</span></span>

|<span data-ttu-id="70856-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="70856-117">**Element**</span></span>|<span data-ttu-id="70856-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="70856-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70856-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="70856-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="70856-120">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="70856-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="70856-121">Text value</span><span class="sxs-lookup"><span data-stu-id="70856-121">Text value</span></span>

<span data-ttu-id="70856-122">O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar as configurações do usuário de acompanhamento de email.</span><span class="sxs-lookup"><span data-stu-id="70856-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email tracking settings for the user.</span></span> <span data-ttu-id="70856-123">O valor do elemento **EcpUrl-mt** contém parâmetros contidos ' <' e ' >' caracteres que são substituídas pelo cliente, conforme mostrado na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="70856-123">The value of the **EcpUrl-mt** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="70856-124">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="70856-124">**Parameter**</span></span>|<span data-ttu-id="70856-125">**Substituir com**</span><span class="sxs-lookup"><span data-stu-id="70856-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="70856-126">_IsOwa_</span><span class="sxs-lookup"><span data-stu-id="70856-126">_IsOwa_</span></span> <br/> |<span data-ttu-id="70856-127">m</span><span class="sxs-lookup"><span data-stu-id="70856-127">n</span></span>  <br/> |
| <span data-ttu-id="70856-128">_MsgID_</span><span class="sxs-lookup"><span data-stu-id="70856-128">_MsgID_</span></span> <br/> |<span data-ttu-id="70856-129">Identificador de mensagens da Internet da mensagem a serem rastreados conforme especificações de HttpCachePolicy o cabeçalho de ID da mensagem.</span><span class="sxs-lookup"><span data-stu-id="70856-129">Internet message identifier of the message to be tracked as specified by the Message-ID header.</span></span>  <br/> |
| <span data-ttu-id="70856-130">_Mbx_</span><span class="sxs-lookup"><span data-stu-id="70856-130">_Mbx_</span></span> <br/> |<span data-ttu-id="70856-131">O endereço SMTP do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="70856-131">The SMTP address of the mailbox owner.</span></span>  <br/> |
| <span data-ttu-id="70856-132">_Sender_</span><span class="sxs-lookup"><span data-stu-id="70856-132">_Sender_</span></span> <br/> |<span data-ttu-id="70856-133">O endereço de SMTP do remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="70856-133">The SMTP address of the message's sender.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="70856-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="70856-134">Remarks</span></span>

<span data-ttu-id="70856-135">O **EcpUrl-mt** é um elemento filho opcionais do elemento de **protocolo** .</span><span class="sxs-lookup"><span data-stu-id="70856-135">The **EcpUrl-mt** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="70856-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="70856-136">See also</span></span>



[<span data-ttu-id="70856-137">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="70856-137">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

