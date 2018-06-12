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
ms.openlocfilehash: 9bf7c8197693bc6887a99ffcbeb2240e1f4c3b20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825468"
---
# <a name="settingname-soap"></a><span data-ttu-id="7eddc-103">SettingName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7eddc-103">SettingName (SOAP)</span></span>

<span data-ttu-id="7eddc-104">O elemento **SettingName** representa o nome de uma configuração na resposta.</span><span class="sxs-lookup"><span data-stu-id="7eddc-104">The **SettingName** element represents the name of a setting in the response.</span></span> 
  
```XML
<SettingName/>
```

 <span data-ttu-id="7eddc-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="7eddc-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7eddc-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7eddc-106">Attributes and elements</span></span>

<span data-ttu-id="7eddc-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7eddc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7eddc-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7eddc-108">Attributes</span></span>

<span data-ttu-id="7eddc-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7eddc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7eddc-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7eddc-110">Child elements</span></span>

<span data-ttu-id="7eddc-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7eddc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7eddc-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7eddc-112">Parent elements</span></span>

|<span data-ttu-id="7eddc-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7eddc-113">**Element**</span></span>|<span data-ttu-id="7eddc-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7eddc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7eddc-115">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7eddc-115">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="7eddc-116">Representa um erro retornado ao recuperar uma configuração de usuário.</span><span class="sxs-lookup"><span data-stu-id="7eddc-116">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="7eddc-117">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7eddc-117">DomainSettingError (SOAP)</span></span>](domainsettingerror-soap.md) <br/> |<span data-ttu-id="7eddc-118">Representa um erro que ocorreu durante a recuperação de uma configuração de domínio.</span><span class="sxs-lookup"><span data-stu-id="7eddc-118">Represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="7eddc-119">Isso representa um erro de uma solicitação de **GetDomainSettings** .</span><span class="sxs-lookup"><span data-stu-id="7eddc-119">This represents an error from a **GetDomainSettings** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7eddc-120">Text value</span><span class="sxs-lookup"><span data-stu-id="7eddc-120">Text value</span></span>

<span data-ttu-id="7eddc-121">O valor do elemento **SettingName** representa o nome de uma configuração em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="7eddc-121">The value of the **SettingName** element represents the name of a setting in a response.</span></span> 
  
<span data-ttu-id="7eddc-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7eddc-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7eddc-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7eddc-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7eddc-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="7eddc-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="7eddc-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7eddc-125">Schema Name</span></span>  <br/> |<span data-ttu-id="7eddc-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="7eddc-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="7eddc-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7eddc-127">Validation File</span></span>  <br/> |<span data-ttu-id="7eddc-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7eddc-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7eddc-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7eddc-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="7eddc-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="7eddc-130">True</span></span>  <br/> |
   

