---
title: Enumeração função cchksgfiles. ERR
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
description: 'Última modificação: 9 de março de 2015'
ms.openlocfilehash: dbc76601a808f79ce3ed5b5dc9fbe4cf92efb015
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455251"
---
# <a name="cchksgfileserr-enumeration"></a><span data-ttu-id="318f2-103">Enumeração função cchksgfiles. ERR</span><span class="sxs-lookup"><span data-stu-id="318f2-103">CChkSGFiles.ERR enumeration</span></span> 
  
<span data-ttu-id="318f2-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="318f2-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="318f2-105">Indica os resultados da função chamada.</span><span class="sxs-lookup"><span data-stu-id="318f2-105">Indicates the results of the called function.</span></span> <span data-ttu-id="318f2-106">Essa enumeração é retornada por muitas funções da classe **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="318f2-106">This enumeration is returned by many functions of the **CCheckSGFiles** class.</span></span> 
  
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

## <a name="values"></a><span data-ttu-id="318f2-107">Values</span><span class="sxs-lookup"><span data-stu-id="318f2-107">Values</span></span>

|<span data-ttu-id="318f2-108">**Nome do membro**</span><span class="sxs-lookup"><span data-stu-id="318f2-108">**Member name**</span></span>|<span data-ttu-id="318f2-109">**Valor**</span><span class="sxs-lookup"><span data-stu-id="318f2-109">**Value**</span></span>|<span data-ttu-id="318f2-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="318f2-110">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="318f2-111">errSuccess</span><span class="sxs-lookup"><span data-stu-id="318f2-111">errSuccess</span></span>  <br/> |<span data-ttu-id="318f2-112">,0</span><span class="sxs-lookup"><span data-stu-id="318f2-112">0</span></span>  <br/> |<span data-ttu-id="318f2-113">A função foi concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="318f2-113">The function completed without any errors.</span></span>  <br/> |
|<span data-ttu-id="318f2-114">errTaskDropped</span><span class="sxs-lookup"><span data-stu-id="318f2-114">errTaskDropped</span></span>  <br/> |<span data-ttu-id="318f2-115">-106</span><span class="sxs-lookup"><span data-stu-id="318f2-115">-106</span></span>  <br/> |<span data-ttu-id="318f2-116">Retornado pela função **ErrTerm** para indicar que nem todas as páginas do banco de dados e os arquivos de log de transações foram verificados ou que foram encontrados erros durante a verificação.</span><span class="sxs-lookup"><span data-stu-id="318f2-116">Returned by the **ErrTerm** function to indicate that not all database pages and transaction log files were checked, or that errors were encountered during the verification.</span></span>  <br/> |
|<span data-ttu-id="318f2-117">errRequiredLogFilesMissing</span><span class="sxs-lookup"><span data-stu-id="318f2-117">errRequiredLogFilesMissing</span></span>  <br/> |<span data-ttu-id="318f2-118">-543</span><span class="sxs-lookup"><span data-stu-id="318f2-118">-543</span></span>  <br/> |<span data-ttu-id="318f2-119">Um ou mais arquivos de log necessários para colocar o banco de dados em um estado de desligamento normal não foram encontrados no caminho do arquivo de log ou não tinham o nome da base de três letras especificado.</span><span class="sxs-lookup"><span data-stu-id="318f2-119">One or more log files that are required to bring the database to a clean-shutdown state was not found in the log file path, or did not have the specified three-letter base name.</span></span>  <br/> |
|<span data-ttu-id="318f2-120">errInvalidParameter</span><span class="sxs-lookup"><span data-stu-id="318f2-120">errInvalidParameter</span></span>  <br/> |<span data-ttu-id="318f2-121">-1003</span><span class="sxs-lookup"><span data-stu-id="318f2-121">-1003</span></span>  <br/> |<span data-ttu-id="318f2-122">Um ou mais parâmetros que foram passados para a função eram inválidos.</span><span class="sxs-lookup"><span data-stu-id="318f2-122">One or more parameters that were passed to the function were invalid.</span></span>  <br/> |
|<span data-ttu-id="318f2-123">errOutOfMemory</span><span class="sxs-lookup"><span data-stu-id="318f2-123">errOutOfMemory</span></span>  <br/> |<span data-ttu-id="318f2-124">-1011</span><span class="sxs-lookup"><span data-stu-id="318f2-124">-1011</span></span>  <br/> |<span data-ttu-id="318f2-125">Memória insuficiente disponível para concluir a operação solicitada.</span><span class="sxs-lookup"><span data-stu-id="318f2-125">Insufficient memory was available to complete the requested operation.</span></span>  <br/> |
|<span data-ttu-id="318f2-126">errReadVerifyFailure</span><span class="sxs-lookup"><span data-stu-id="318f2-126">errReadVerifyFailure</span></span>  <br/> |<span data-ttu-id="318f2-127">-1018</span><span class="sxs-lookup"><span data-stu-id="318f2-127">-1018</span></span>  <br/> |<span data-ttu-id="318f2-128">O checksum armazenado em uma página de banco de dados não corresponde à soma de verificação esperada.</span><span class="sxs-lookup"><span data-stu-id="318f2-128">The checksum that is stored on a database page does not match its expected checksum.</span></span>  <br/> |
|<span data-ttu-id="318f2-129">errTooManyActiveUsers</span><span class="sxs-lookup"><span data-stu-id="318f2-129">errTooManyActiveUsers</span></span>  <br/> |<span data-ttu-id="318f2-130">-1059</span><span class="sxs-lookup"><span data-stu-id="318f2-130">-1059</span></span>  <br/> |<span data-ttu-id="318f2-131">A função **ErrTerm** foi chamada enquanto o objeto ainda estava sendo usado.</span><span class="sxs-lookup"><span data-stu-id="318f2-131">The **ErrTerm** function was called while the object was still being used.</span></span> <span data-ttu-id="318f2-132">Isso pode ocorrer se **ErrTerm** for chamado antes de **ErrCheckDbPages** ou **ErrCheckLogFiles** ter retornado.</span><span class="sxs-lookup"><span data-stu-id="318f2-132">This can occur if **ErrTerm** is called before **ErrCheckDbPages** or **ErrCheckLogFiles** has returned.</span></span>  <br/> |
   
## <a name="requirements"></a><span data-ttu-id="318f2-133">Requirements</span><span class="sxs-lookup"><span data-stu-id="318f2-133">Requirements</span></span>

<span data-ttu-id="318f2-134">O Exchange Server 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="318f2-134">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="318f2-135">A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.</span><span class="sxs-lookup"><span data-stu-id="318f2-135">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

