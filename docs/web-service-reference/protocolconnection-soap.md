---
title: ProtocolConnection (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6eef2188-6194-48f1-ad7e-46104aecdf56
description: O elemento ProtocolConnection representa a conexão de protocolo do cliente Web do servidor.
ms.openlocfilehash: b9df3febe36db53d7c5bf0610ba857f13aa96abc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528857"
---
# <a name="protocolconnection-soap"></a><span data-ttu-id="dfc82-103">ProtocolConnection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dfc82-103">ProtocolConnection (SOAP)</span></span>

<span data-ttu-id="dfc82-104">O elemento **ProtocolConnection** representa a conexão de protocolo do cliente Web do servidor.</span><span class="sxs-lookup"><span data-stu-id="dfc82-104">The **ProtocolConnection** element represents the protocol connection of the server Web client.</span></span> 
  
```XML
<ProtocolConnection>
   <Hostname/>
   <Port/>
   <EncryptionMethod/>
</ProtocolConnection>
```

 <span data-ttu-id="dfc82-105">**ProtocolConnection**</span><span class="sxs-lookup"><span data-stu-id="dfc82-105">**ProtocolConnection**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dfc82-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="dfc82-106">Attributes and elements</span></span>

<span data-ttu-id="dfc82-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dfc82-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dfc82-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="dfc82-108">Attributes</span></span>

<span data-ttu-id="dfc82-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dfc82-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dfc82-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dfc82-110">Child elements</span></span>

|<span data-ttu-id="dfc82-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dfc82-111">**Element**</span></span>|<span data-ttu-id="dfc82-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dfc82-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dfc82-113">Nome do host (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dfc82-113">Hostname (SOAP)</span></span>](hostname-soap.md) <br/> |<span data-ttu-id="dfc82-114">Representa a parte do nome do host do nome completo do computador.</span><span class="sxs-lookup"><span data-stu-id="dfc82-114">Represents the host name portion of the full computer name of the computer.</span></span>  <br/> |
|[<span data-ttu-id="dfc82-115">Porta (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dfc82-115">Port (SOAP)</span></span>](port-soap.md) <br/> |<span data-ttu-id="dfc82-116">Representa o número da porta a ser usado para o protocolo.</span><span class="sxs-lookup"><span data-stu-id="dfc82-116">Represents the port number to use for the protocol.</span></span>  <br/> |
|[<span data-ttu-id="dfc82-117">EncryptionMethod (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dfc82-117">EncryptionMethod (SOAP)</span></span>](encryptionmethod-soap.md) <br/> |<span data-ttu-id="dfc82-118">Representa o método criptográfico que é usado para os protocolos POP, IMAP e SMTP.</span><span class="sxs-lookup"><span data-stu-id="dfc82-118">Represents the cryptographic method that is used for the POP, IMAP, and SMTP protocols.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dfc82-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dfc82-119">Parent elements</span></span>

|<span data-ttu-id="dfc82-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dfc82-120">**Element**</span></span>|<span data-ttu-id="dfc82-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dfc82-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dfc82-122">ProtocolConnections (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dfc82-122">ProtocolConnections (SOAP)</span></span>](protocolconnections-soap.md) <br/> |<span data-ttu-id="dfc82-123">Contém zero ou mais conexões de protocolo.</span><span class="sxs-lookup"><span data-stu-id="dfc82-123">Contains zero or more protocol connections.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dfc82-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="dfc82-124">Text value</span></span>

<span data-ttu-id="dfc82-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dfc82-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dfc82-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="dfc82-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dfc82-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="dfc82-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="dfc82-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dfc82-128">Schema Name</span></span>  <br/> |<span data-ttu-id="dfc82-129">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="dfc82-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="dfc82-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dfc82-130">Validation File</span></span>  <br/> |<span data-ttu-id="dfc82-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dfc82-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dfc82-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="dfc82-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="dfc82-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="dfc82-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dfc82-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="dfc82-134">See also</span></span>



[<span data-ttu-id="dfc82-135">ProtocolConnectionCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dfc82-135">ProtocolConnectionCollectionSetting (SOAP)</span></span>](protocolconnectioncollectionsetting-soap.md)

