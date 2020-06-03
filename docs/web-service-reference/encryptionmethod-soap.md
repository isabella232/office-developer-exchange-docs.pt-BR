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
description: O elemento EncryptionMethod representa o método criptográfico que é usado para os protocolos POP, IMAP e SMTP.
ms.openlocfilehash: 26236d9b08eae1bcabfd9aac59f5b01714ba9841
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530653"
---
# <a name="encryptionmethod-soap"></a><span data-ttu-id="5cd4f-103">EncryptionMethod (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5cd4f-103">EncryptionMethod (SOAP)</span></span>

<span data-ttu-id="5cd4f-104">O elemento **EncryptionMethod** representa o método criptográfico que é usado para os protocolos pop, IMAP e SMTP.</span><span class="sxs-lookup"><span data-stu-id="5cd4f-104">The **EncryptionMethod** element represents the cryptographic method that is used for the POP, IMAP, and SMTP protocols.</span></span> 
  
```XML
<EncryptionMethod/>
```

 <span data-ttu-id="5cd4f-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="5cd4f-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5cd4f-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5cd4f-106">Attributes and elements</span></span>

<span data-ttu-id="5cd4f-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5cd4f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5cd4f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5cd4f-108">Attributes</span></span>

<span data-ttu-id="5cd4f-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5cd4f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5cd4f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5cd4f-110">Child elements</span></span>

<span data-ttu-id="5cd4f-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5cd4f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5cd4f-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5cd4f-112">Parent elements</span></span>

|<span data-ttu-id="5cd4f-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5cd4f-113">**Element**</span></span>|<span data-ttu-id="5cd4f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5cd4f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cd4f-115">ProtocolConnection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5cd4f-115">ProtocolConnection (SOAP)</span></span>](protocolconnection-soap.md) <br/> |<span data-ttu-id="5cd4f-116">Representa a conexão de protocolo do cliente Web do servidor.</span><span class="sxs-lookup"><span data-stu-id="5cd4f-116">Represents the protocol connection of the server Web client.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5cd4f-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5cd4f-117">Text value</span></span>

<span data-ttu-id="5cd4f-118">O valor de texto para esse elemento é o método criptográfico que é usado para os protocolos POP, IMAP e SMTP.</span><span class="sxs-lookup"><span data-stu-id="5cd4f-118">The text value for this element is the cryptographic method that is used for the POP, IMAP, and SMTP protocols.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5cd4f-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5cd4f-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5cd4f-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="5cd4f-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="5cd4f-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5cd4f-121">Schema Name</span></span>  <br/> |<span data-ttu-id="5cd4f-122">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="5cd4f-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="5cd4f-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5cd4f-123">Validation File</span></span>  <br/> |<span data-ttu-id="5cd4f-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5cd4f-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5cd4f-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5cd4f-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="5cd4f-126">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="5cd4f-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5cd4f-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="5cd4f-127">See also</span></span>

- [<span data-ttu-id="5cd4f-128">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5cd4f-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

