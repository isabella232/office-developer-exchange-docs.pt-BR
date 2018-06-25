---
title: Função CChkSGFiles.ErrInit
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrInit
api_type:
- dllExport
ms.assetid: 61bb3af1-8b51-4bae-8e25-90a4dc1226c5
description: 'Modificado pela última vez: 03 de março de 2013'
ms.openlocfilehash: d4b76933a747fe4bf084061cf080bc68264132ed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750628"
---
# <a name="cchksgfileserrinit-function"></a><span data-ttu-id="893b0-103">Função CChkSGFiles.ErrInit</span><span class="sxs-lookup"><span data-stu-id="893b0-103">CChkSGFiles.ErrInit function</span></span>
  
<span data-ttu-id="893b0-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="893b0-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="893b0-105">Inicializa o objeto **CChkSGFiles** especificando os bancos de dados a ser verificado e o caminho e nome de base dos arquivos de log de transação a ser verificado.</span><span class="sxs-lookup"><span data-stu-id="893b0-105">Initializes the **CChkSGFiles** object by specifying the databases to be checked and the path and base name of the transaction log files to be checked.</span></span> <span data-ttu-id="893b0-106">Aplicativos devem chamar essa função imediatamente após chamar com êxito a função de **New** .</span><span class="sxs-lookup"><span data-stu-id="893b0-106">Applications should call this function immediately after successfully calling the **New** function.</span></span> 
  
```cs
Vitual ERRErrInit  
(
    Const WCHAR  * const rgwszDb[],
    Const ULONGcDB,
    __in_z const WCHAR  * const wszLogPath,
    __in_z const WCHAR  * const wszBaseName,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="893b0-107">Par�metros</span><span class="sxs-lookup"><span data-stu-id="893b0-107">Parameters</span></span>

### <a name="rgwszdb"></a><span data-ttu-id="893b0-108">[] de rgwszDb</span><span class="sxs-lookup"><span data-stu-id="893b0-108">rgwszDb[]</span></span>
  
<span data-ttu-id="893b0-109">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="893b0-109">Input parameter.</span></span> <span data-ttu-id="893b0-110">Uma matriz que especifica os bancos de dados a ser verificado.</span><span class="sxs-lookup"><span data-stu-id="893b0-110">An array that specifies the databases to be checked.</span></span> <span data-ttu-id="893b0-111">Cada elemento da matriz é uma cadeia de Unicode terminada em nulo que contém o nome de arquivo e o caminho de um banco de dados a ser verificado.</span><span class="sxs-lookup"><span data-stu-id="893b0-111">Each array element is a null-terminated Unicode string that contains the path and file name of a database to be checked.</span></span>
    
### <a name="cdb"></a><span data-ttu-id="893b0-112">cDB</span><span class="sxs-lookup"><span data-stu-id="893b0-112">cDB</span></span>
  
<span data-ttu-id="893b0-113">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="893b0-113">Input parameter.</span></span> <span data-ttu-id="893b0-114">O número de elementos na matriz **rgwszDb** do caminho de banco de dados válido.</span><span class="sxs-lookup"><span data-stu-id="893b0-114">The number of valid database path elements in the **rgwszDb** array.</span></span> 
    
#### <a name="wszlogpath"></a><span data-ttu-id="893b0-115">wszLogPath</span><span class="sxs-lookup"><span data-stu-id="893b0-115">wszLogPath</span></span>
  
<span data-ttu-id="893b0-116">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="893b0-116">Input parameter.</span></span> <span data-ttu-id="893b0-117">O caminho completo dos arquivos de log de transações a serem verificados, na forma de uma cadeia de caracteres Unicode terminada em nulo.</span><span class="sxs-lookup"><span data-stu-id="893b0-117">The full path of the transaction log files to be checked, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="wszbasename"></a><span data-ttu-id="893b0-118">wszBaseName</span><span class="sxs-lookup"><span data-stu-id="893b0-118">wszBaseName</span></span>
  
<span data-ttu-id="893b0-119">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="893b0-119">Input parameter.</span></span> <span data-ttu-id="893b0-120">O nome de base três letras dos arquivos de log de transação do Exchange, na forma de uma cadeia de caracteres Unicode terminada em nulo.</span><span class="sxs-lookup"><span data-stu-id="893b0-120">The three-letter base name of the Exchange transaction log files, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="ulflags"></a><span data-ttu-id="893b0-121">ulFlags</span><span class="sxs-lookup"><span data-stu-id="893b0-121">ulFlags</span></span>
  
<span data-ttu-id="893b0-122">Parâmetro de entrada opcional.</span><span class="sxs-lookup"><span data-stu-id="893b0-122">Optional input parameter.</span></span> <span data-ttu-id="893b0-123">Esse valor é reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="893b0-123">This value is reserved for future use.</span></span> <span data-ttu-id="893b0-124">O valor passado por este parâmetro deve ser de 0 (zero).</span><span class="sxs-lookup"><span data-stu-id="893b0-124">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="893b0-125">Valor retornado</span><span class="sxs-lookup"><span data-stu-id="893b0-125">Return value</span></span>

<span data-ttu-id="893b0-126">Um código de erro da enumeração [ERR](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="893b0-126">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="893b0-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="893b0-127">Remarks</span></span>

<span data-ttu-id="893b0-128">A função **ErrInit** registra os bancos de dados e arquivos de log a serem verificados.</span><span class="sxs-lookup"><span data-stu-id="893b0-128">The **ErrInit** function registers the databases and log files that are to be checked.</span></span> <span data-ttu-id="893b0-129">Esta função deve ser chamada após a função **New** é chamada, mas antes de qualquer outro **ChkSGFiles** é chamada de função.</span><span class="sxs-lookup"><span data-stu-id="893b0-129">This function must be called after the **New** function is called but before any other **ChkSGFiles** function is called.</span></span> 
  
<span data-ttu-id="893b0-130">Você deve fornecer o nome de base, o caminho do arquivo de log e todos os nomes de banco de dados como sequências de caracteres de Unicode terminada em nulo.</span><span class="sxs-lookup"><span data-stu-id="893b0-130">You must provide all the database names, the log file path, and the base name as null-terminated Unicode strings.</span></span>
  
<span data-ttu-id="893b0-131">Você pode verificar somente os arquivos de banco de dados, somente os arquivos de log, ou os arquivos de log e de banco de dados.</span><span class="sxs-lookup"><span data-stu-id="893b0-131">You can check only the database files, only the log files, or both the database and log files.</span></span> <span data-ttu-id="893b0-132">No entanto, ao chamar essa função, o aplicativo deve especificar pelo menos uma entidade a ser verificado.</span><span class="sxs-lookup"><span data-stu-id="893b0-132">However, when calling this function, the application must specify at least one entity to be checked.</span></span> <span data-ttu-id="893b0-133">Passar 0 (zero) para **cDB** e NULL para **wszLogPath** retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="893b0-133">Passing 0 (zero) for  **cDB**  and NULL for  **wszLogPath**  will return an error.</span></span> 
  
<span data-ttu-id="893b0-134">Se o valor da **cDB** for diferente de 0 (zero), passar NULL para **rgwszDb** resultará em erro.</span><span class="sxs-lookup"><span data-stu-id="893b0-134">If the value of  **cDB**  is other than 0 (zero), passing NULL for  **rgwszDb**  will result in an error.</span></span> <span data-ttu-id="893b0-135">Para verificar se os arquivos de banco de dados, o aplicativo deve fornecer os nomes de banco de dados.</span><span class="sxs-lookup"><span data-stu-id="893b0-135">To check the database files, the application must provide the database names.</span></span> 
  
<span data-ttu-id="893b0-136">Se NULL é passado para **wszBaseName** , mas **wszLogPath** não for nula, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="893b0-136">If NULL is passed for  **wszBaseName**  but  **wszLogPath**  is not NULL, an error will be returned.</span></span> <span data-ttu-id="893b0-137">Um nome de arquivo de log base é sempre necessário ao verificar arquivos de log.</span><span class="sxs-lookup"><span data-stu-id="893b0-137">A log file base name is always required when checking log files.</span></span> 
  
<span data-ttu-id="893b0-138">Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você deve chamar a função **ErrInit** na parte com um único segmento do aplicativo e você poderá chamá-lo apenas uma vez para cada objeto **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="893b0-138">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrInit** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="893b0-139">Requisitos</span><span class="sxs-lookup"><span data-stu-id="893b0-139">Requirements</span></span>

<span data-ttu-id="893b0-140">Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="893b0-140">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="893b0-141">A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.</span><span class="sxs-lookup"><span data-stu-id="893b0-141">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

