---
title: EncryptionMethod (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: bc632c85-ec74-4a00-baec-df5973e032fa
description: O elemento EncryptionMethod representa o método de criptografia que é usado para os protocolos POP, IMAP e SMTP.
ms.openlocfilehash: 5062d357a54019a576e391e1be4d4e8dfcc6e38d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752042"
---
# <a name="encryptionmethod-soap"></a><span data-ttu-id="d9a07-103">EncryptionMethod (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d9a07-103">EncryptionMethod (SOAP)</span></span>

<span data-ttu-id="d9a07-104">O elemento **EncryptionMethod** representa o método de criptografia que é usado para os protocolos POP, IMAP e SMTP.</span><span class="sxs-lookup"><span data-stu-id="d9a07-104">The **EncryptionMethod** element represents the cryptographic method that is used for the POP, IMAP, and SMTP protocols.</span></span> 
  
```XML
<EncryptionMethod/>
```

 <span data-ttu-id="d9a07-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="d9a07-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9a07-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d9a07-106">Attributes and elements</span></span>

<span data-ttu-id="d9a07-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d9a07-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9a07-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d9a07-108">Attributes</span></span>

<span data-ttu-id="d9a07-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d9a07-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9a07-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d9a07-110">Child elements</span></span>

<span data-ttu-id="d9a07-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d9a07-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d9a07-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d9a07-112">Parent elements</span></span>

|<span data-ttu-id="d9a07-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d9a07-113">**Element**</span></span>|<span data-ttu-id="d9a07-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d9a07-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9a07-115">ProtocolConnection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d9a07-115">ProtocolConnection (SOAP)</span></span>](protocolconnection-soap.md) <br/> |<span data-ttu-id="d9a07-116">Representa a conexão de protocolo do cliente da Web do servidor.</span><span class="sxs-lookup"><span data-stu-id="d9a07-116">Represents the protocol connection of the server Web client.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d9a07-117">Text value</span><span class="sxs-lookup"><span data-stu-id="d9a07-117">Text value</span></span>

<span data-ttu-id="d9a07-118">O valor de texto para esse elemento é o método de criptografia que é usado para os protocolos POP, IMAP e SMTP.</span><span class="sxs-lookup"><span data-stu-id="d9a07-118">The text value for this element is the cryptographic method that is used for the POP, IMAP, and SMTP protocols.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9a07-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d9a07-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9a07-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="d9a07-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d9a07-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d9a07-121">Schema Name</span></span>  <br/> |<span data-ttu-id="d9a07-122">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="d9a07-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d9a07-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d9a07-123">Validation File</span></span>  <br/> |<span data-ttu-id="d9a07-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d9a07-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d9a07-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d9a07-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9a07-126">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="d9a07-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9a07-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="d9a07-127">See also</span></span>

- [<span data-ttu-id="d9a07-128">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d9a07-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

