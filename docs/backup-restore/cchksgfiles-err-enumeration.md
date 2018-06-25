---
title: Enumeração CChkSGFiles.ERR
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ERR
api_type:
- dllExport
ms.assetid: f0efe195-91c3-4f3a-8c7d-e5dba336465a
description: '�ltima altera��o: segunda-feira, 9 de mar�o de 2015'
ms.openlocfilehash: 20f10c43e3b92604bb51e1aa5f896a8bd7c4b335
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751575"
---
# <a name="cchksgfileserr-enumeration"></a><span data-ttu-id="23a30-103">Enumeração CChkSGFiles.ERR</span><span class="sxs-lookup"><span data-stu-id="23a30-103">CChkSGFiles.ERR enumeration</span></span> 
  
<span data-ttu-id="23a30-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="23a30-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="23a30-105">Indica os resultados da função chamada.</span><span class="sxs-lookup"><span data-stu-id="23a30-105">Indicates the results of the called function.</span></span> <span data-ttu-id="23a30-106">Esta enumeração é retornada por muitas funções da classe **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="23a30-106">This enumeration is returned by many functions of the **CCheckSGFiles** class.</span></span> 
  
```cs
Enum ERR  
{
        errSuccess = 0,
        errTaskDropped = -106,
        errRequiredLogFilesMissing = -543,
        errInvalidParameter = -1003,
        errOutOfMemory = -1011,
        errReadVerifyFailure = -1018,
        errTooManyActiveUsers = -1059,
        errDatabaseCorrupted = -1206
}

```

## <a name="values"></a><span data-ttu-id="23a30-107">Valores</span><span class="sxs-lookup"><span data-stu-id="23a30-107">Values</span></span>

|<span data-ttu-id="23a30-108">**Nome do membro**</span><span class="sxs-lookup"><span data-stu-id="23a30-108">**Member name**</span></span>|<span data-ttu-id="23a30-109">**Valor**</span><span class="sxs-lookup"><span data-stu-id="23a30-109">**Value**</span></span>|<span data-ttu-id="23a30-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="23a30-110">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="23a30-111">errSuccess</span><span class="sxs-lookup"><span data-stu-id="23a30-111">errSuccess</span></span>  <br/> |<span data-ttu-id="23a30-112">0</span><span class="sxs-lookup"><span data-stu-id="23a30-112">0</span></span>  <br/> |<span data-ttu-id="23a30-113">A função concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="23a30-113">The function completed without any errors.</span></span>  <br/> |
|<span data-ttu-id="23a30-114">errTaskDropped</span><span class="sxs-lookup"><span data-stu-id="23a30-114">errTaskDropped</span></span>  <br/> |<span data-ttu-id="23a30-115">-106</span><span class="sxs-lookup"><span data-stu-id="23a30-115">-106</span></span>  <br/> |<span data-ttu-id="23a30-116">Retornado pela função **ErrTerm** para indicar que nem todas as páginas do banco de dados e arquivos de log de transações marcados ou que foram encontrados erros durante a verificação.</span><span class="sxs-lookup"><span data-stu-id="23a30-116">Returned by the **ErrTerm** function to indicate that not all database pages and transaction log files were checked, or that errors were encountered during the verification.</span></span>  <br/> |
|<span data-ttu-id="23a30-117">errRequiredLogFilesMissing</span><span class="sxs-lookup"><span data-stu-id="23a30-117">errRequiredLogFilesMissing</span></span>  <br/> |<span data-ttu-id="23a30-118">-543</span><span class="sxs-lookup"><span data-stu-id="23a30-118">-543</span></span>  <br/> |<span data-ttu-id="23a30-119">Um ou mais arquivos de log que são necessários para que o banco de dados para um estado de desligamento não foi encontrado no caminho do arquivo de log ou não tinha o nome de base de três letras especificado.</span><span class="sxs-lookup"><span data-stu-id="23a30-119">One or more log files that are required to bring the database to a clean-shutdown state was not found in the log file path, or did not have the specified three-letter base name.</span></span>  <br/> |
|<span data-ttu-id="23a30-120">errInvalidParameter</span><span class="sxs-lookup"><span data-stu-id="23a30-120">errInvalidParameter</span></span>  <br/> |<span data-ttu-id="23a30-121">-1003</span><span class="sxs-lookup"><span data-stu-id="23a30-121">-1003</span></span>  <br/> |<span data-ttu-id="23a30-122">Um ou mais parâmetros que foram passados para a função eram inválidos.</span><span class="sxs-lookup"><span data-stu-id="23a30-122">One or more parameters that were passed to the function were invalid.</span></span>  <br/> |
|<span data-ttu-id="23a30-123">errOutOfMemory</span><span class="sxs-lookup"><span data-stu-id="23a30-123">errOutOfMemory</span></span>  <br/> |<span data-ttu-id="23a30-124">-1011</span><span class="sxs-lookup"><span data-stu-id="23a30-124">-1011</span></span>  <br/> |<span data-ttu-id="23a30-125">Memória insuficiente estava disponível para concluir a operação solicitada.</span><span class="sxs-lookup"><span data-stu-id="23a30-125">Insufficient memory was available to complete the requested operation.</span></span>  <br/> |
|<span data-ttu-id="23a30-126">errReadVerifyFailure</span><span class="sxs-lookup"><span data-stu-id="23a30-126">errReadVerifyFailure</span></span>  <br/> |<span data-ttu-id="23a30-127">-1018</span><span class="sxs-lookup"><span data-stu-id="23a30-127">-1018</span></span>  <br/> |<span data-ttu-id="23a30-128">A soma de verificação que é armazenada em uma página de banco de dados não coincide com sua soma de verificação esperada.</span><span class="sxs-lookup"><span data-stu-id="23a30-128">The checksum that is stored on a database page does not match its expected checksum.</span></span>  <br/> |
|<span data-ttu-id="23a30-129">errTooManyActiveUsers</span><span class="sxs-lookup"><span data-stu-id="23a30-129">errTooManyActiveUsers</span></span>  <br/> |<span data-ttu-id="23a30-130">-1059</span><span class="sxs-lookup"><span data-stu-id="23a30-130">-1059</span></span>  <br/> |<span data-ttu-id="23a30-131">A função **ErrTerm** foi chamada enquanto o objeto ainda estava sendo usado.</span><span class="sxs-lookup"><span data-stu-id="23a30-131">The **ErrTerm** function was called while the object was still being used.</span></span> <span data-ttu-id="23a30-132">Isso pode ocorrer se **ErrTerm** é chamado antes **ErrCheckDbPages** ou **ErrCheckLogFiles** ter retornado.</span><span class="sxs-lookup"><span data-stu-id="23a30-132">This can occur if **ErrTerm** is called before **ErrCheckDbPages** or **ErrCheckLogFiles** has returned.</span></span>  <br/> |
   
## <a name="requirements"></a><span data-ttu-id="23a30-133">Requisitos</span><span class="sxs-lookup"><span data-stu-id="23a30-133">Requirements</span></span>

<span data-ttu-id="23a30-134">Exchange Server 2013 apenas inclui uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="23a30-134">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="23a30-135">A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.</span><span class="sxs-lookup"><span data-stu-id="23a30-135">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

