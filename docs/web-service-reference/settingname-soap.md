---
title: SettingName (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8bcb0411-58b0-4e37-b97e-00c07dcbecb1
description: O elemento SettingName representa o nome de uma configuração na resposta.
ms.openlocfilehash: d492b82b7385d6403f15c08356db5d0503792d54
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466721"
---
# <a name="settingname-soap"></a><span data-ttu-id="c89ec-103">SettingName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c89ec-103">SettingName (SOAP)</span></span>

<span data-ttu-id="c89ec-104">O elemento **SettingName** representa o nome de uma configuração na resposta.</span><span class="sxs-lookup"><span data-stu-id="c89ec-104">The **SettingName** element represents the name of a setting in the response.</span></span> 
  
```XML
<SettingName/>
```

 <span data-ttu-id="c89ec-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="c89ec-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c89ec-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c89ec-106">Attributes and elements</span></span>

<span data-ttu-id="c89ec-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c89ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c89ec-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c89ec-108">Attributes</span></span>

<span data-ttu-id="c89ec-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c89ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c89ec-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c89ec-110">Child elements</span></span>

<span data-ttu-id="c89ec-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c89ec-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c89ec-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c89ec-112">Parent elements</span></span>

|<span data-ttu-id="c89ec-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c89ec-113">**Element**</span></span>|<span data-ttu-id="c89ec-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c89ec-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c89ec-115">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c89ec-115">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="c89ec-116">Representa um erro retornado ao recuperar uma configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="c89ec-116">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="c89ec-117">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c89ec-117">DomainSettingError (SOAP)</span></span>](domainsettingerror-soap.md) <br/> |<span data-ttu-id="c89ec-118">Representa um erro que ocorreu ao recuperar uma configuração de domínio.</span><span class="sxs-lookup"><span data-stu-id="c89ec-118">Represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="c89ec-119">Isso representa um erro de uma solicitação **GetDomainSettings** .</span><span class="sxs-lookup"><span data-stu-id="c89ec-119">This represents an error from a **GetDomainSettings** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c89ec-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c89ec-120">Text value</span></span>

<span data-ttu-id="c89ec-121">O valor do elemento **SettingName** representa o nome de uma configuração em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="c89ec-121">The value of the **SettingName** element represents the name of a setting in a response.</span></span> 
  
<span data-ttu-id="c89ec-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c89ec-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c89ec-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c89ec-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c89ec-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="c89ec-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c89ec-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c89ec-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c89ec-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="c89ec-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c89ec-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c89ec-127">Validation File</span></span>  <br/> |<span data-ttu-id="c89ec-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c89ec-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c89ec-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c89ec-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="c89ec-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="c89ec-130">True</span></span>  <br/> |
   

