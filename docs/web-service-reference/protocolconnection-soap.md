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
description: O elemento ProtocolConnection representa a conexão de protocolo do cliente da Web do servidor.
ms.openlocfilehash: 8b5396821cd959e41d24fcf7a94c519f9c634a1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824915"
---
# <a name="protocolconnection-soap"></a><span data-ttu-id="74898-103">ProtocolConnection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74898-103">ProtocolConnection (SOAP)</span></span>

<span data-ttu-id="74898-104">O elemento **ProtocolConnection** representa a conexão de protocolo do cliente da Web do servidor.</span><span class="sxs-lookup"><span data-stu-id="74898-104">The **ProtocolConnection** element represents the protocol connection of the server Web client.</span></span> 
  
```XML
<ProtocolConnection>
   <Hostname/>
   <Port/>
   <EncryptionMethod/>
</ProtocolConnection>
```

 <span data-ttu-id="74898-105">**ProtocolConnection**</span><span class="sxs-lookup"><span data-stu-id="74898-105">**ProtocolConnection**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74898-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="74898-106">Attributes and elements</span></span>

<span data-ttu-id="74898-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="74898-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74898-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="74898-108">Attributes</span></span>

<span data-ttu-id="74898-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="74898-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74898-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="74898-110">Child elements</span></span>

|<span data-ttu-id="74898-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="74898-111">**Element**</span></span>|<span data-ttu-id="74898-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="74898-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74898-113">O nome de host (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74898-113">Hostname (SOAP)</span></span>](hostname-soap.md) <br/> |<span data-ttu-id="74898-114">Representa a parte do nome de host do nome completo do computador do computador.</span><span class="sxs-lookup"><span data-stu-id="74898-114">Represents the host name portion of the full computer name of the computer.</span></span>  <br/> |
|[<span data-ttu-id="74898-115">Porta (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74898-115">Port (SOAP)</span></span>](port-soap.md) <br/> |<span data-ttu-id="74898-116">Representa o número da porta a ser usado para o protocolo.</span><span class="sxs-lookup"><span data-stu-id="74898-116">Represents the port number to use for the protocol.</span></span>  <br/> |
|[<span data-ttu-id="74898-117">EncryptionMethod (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74898-117">EncryptionMethod (SOAP)</span></span>](encryptionmethod-soap.md) <br/> |<span data-ttu-id="74898-118">Representa o método de criptografia que é usado para os protocolos POP, IMAP e SMTP.</span><span class="sxs-lookup"><span data-stu-id="74898-118">Represents the cryptographic method that is used for the POP, IMAP, and SMTP protocols.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="74898-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="74898-119">Parent elements</span></span>

|<span data-ttu-id="74898-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="74898-120">**Element**</span></span>|<span data-ttu-id="74898-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="74898-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74898-122">ProtocolConnections (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74898-122">ProtocolConnections (SOAP)</span></span>](protocolconnections-soap.md) <br/> |<span data-ttu-id="74898-123">Contém as conexões de protocolo de zero ou mais.</span><span class="sxs-lookup"><span data-stu-id="74898-123">Contains zero or more protocol connections.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="74898-124">Text value</span><span class="sxs-lookup"><span data-stu-id="74898-124">Text value</span></span>

<span data-ttu-id="74898-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="74898-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74898-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="74898-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74898-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="74898-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="74898-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="74898-128">Schema Name</span></span>  <br/> |<span data-ttu-id="74898-129">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="74898-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="74898-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="74898-130">Validation File</span></span>  <br/> |<span data-ttu-id="74898-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="74898-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74898-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="74898-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="74898-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="74898-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74898-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="74898-134">See also</span></span>



[<span data-ttu-id="74898-135">ProtocolConnectionCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74898-135">ProtocolConnectionCollectionSetting (SOAP)</span></span>](protocolconnectioncollectionsetting-soap.md)

