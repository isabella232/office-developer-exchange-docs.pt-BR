---
title: Função função cchksgfiles. ErrInit
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
description: 'Última modificação: 03 de março de 2013'
ms.openlocfilehash: c881691e7c1ba83a396e659f6aac0328625e49a5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457008"
---
# <a name="cchksgfileserrinit-function"></a><span data-ttu-id="04637-103">Função função cchksgfiles. ErrInit</span><span class="sxs-lookup"><span data-stu-id="04637-103">CChkSGFiles.ErrInit function</span></span>
  
<span data-ttu-id="04637-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="04637-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="04637-105">Inicializa o objeto **função cchksgfiles** especificando os bancos de dados a serem verificados e o caminho e o nome base dos arquivos de log de transações a serem verificados.</span><span class="sxs-lookup"><span data-stu-id="04637-105">Initializes the **CChkSGFiles** object by specifying the databases to be checked and the path and base name of the transaction log files to be checked.</span></span> <span data-ttu-id="04637-106">Os aplicativos devem chamar essa função imediatamente após chamarem com êxito a **nova** função.</span><span class="sxs-lookup"><span data-stu-id="04637-106">Applications should call this function immediately after successfully calling the **New** function.</span></span> 
  
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

## <a name="parameters"></a><span data-ttu-id="04637-107">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="04637-107">Parameters</span></span>

### <a name="rgwszdb"></a><span data-ttu-id="04637-108">rgwszDb[]</span><span class="sxs-lookup"><span data-stu-id="04637-108">rgwszDb[]</span></span>
  
<span data-ttu-id="04637-109">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="04637-109">Input parameter.</span></span> <span data-ttu-id="04637-110">Uma matriz que especifica os bancos de dados a serem verificados.</span><span class="sxs-lookup"><span data-stu-id="04637-110">An array that specifies the databases to be checked.</span></span> <span data-ttu-id="04637-111">Cada elemento da matriz é uma cadeia de caracteres Unicode terminada em nulo que contém o caminho e o nome de arquivo de um banco de dados a ser verificado.</span><span class="sxs-lookup"><span data-stu-id="04637-111">Each array element is a null-terminated Unicode string that contains the path and file name of a database to be checked.</span></span>
    
### <a name="cdb"></a><span data-ttu-id="04637-112">cDB</span><span class="sxs-lookup"><span data-stu-id="04637-112">cDB</span></span>
  
<span data-ttu-id="04637-113">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="04637-113">Input parameter.</span></span> <span data-ttu-id="04637-114">O número de elementos de caminho de banco de dados válidos na matriz **rgwszDb** .</span><span class="sxs-lookup"><span data-stu-id="04637-114">The number of valid database path elements in the **rgwszDb** array.</span></span> 
    
#### <a name="wszlogpath"></a><span data-ttu-id="04637-115">wszLogPath</span><span class="sxs-lookup"><span data-stu-id="04637-115">wszLogPath</span></span>
  
<span data-ttu-id="04637-116">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="04637-116">Input parameter.</span></span> <span data-ttu-id="04637-117">O caminho completo dos arquivos de log de transações a serem verificados, na forma de uma cadeia de caracteres Unicode terminada em nulo.</span><span class="sxs-lookup"><span data-stu-id="04637-117">The full path of the transaction log files to be checked, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="wszbasename"></a><span data-ttu-id="04637-118">wszBaseName</span><span class="sxs-lookup"><span data-stu-id="04637-118">wszBaseName</span></span>
  
<span data-ttu-id="04637-119">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="04637-119">Input parameter.</span></span> <span data-ttu-id="04637-120">O nome base de três letras dos arquivos de log de transações do Exchange, na forma de uma cadeia de caracteres Unicode terminada em nulo.</span><span class="sxs-lookup"><span data-stu-id="04637-120">The three-letter base name of the Exchange transaction log files, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="ulflags"></a><span data-ttu-id="04637-121">ulFlags</span><span class="sxs-lookup"><span data-stu-id="04637-121">ulFlags</span></span>
  
<span data-ttu-id="04637-122">Parâmetro de entrada opcional.</span><span class="sxs-lookup"><span data-stu-id="04637-122">Optional input parameter.</span></span> <span data-ttu-id="04637-123">Esse valor é reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="04637-123">This value is reserved for future use.</span></span> <span data-ttu-id="04637-124">O valor passado por esse parâmetro deve ser 0 (zero).</span><span class="sxs-lookup"><span data-stu-id="04637-124">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="04637-125">Valor de retorno</span><span class="sxs-lookup"><span data-stu-id="04637-125">Return value</span></span>

<span data-ttu-id="04637-126">Um código de erro da enumeração [Err](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="04637-126">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="04637-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="04637-127">Remarks</span></span>

<span data-ttu-id="04637-128">A função **ErrInit** registra os bancos de dados e arquivos de log que devem ser verificados.</span><span class="sxs-lookup"><span data-stu-id="04637-128">The **ErrInit** function registers the databases and log files that are to be checked.</span></span> <span data-ttu-id="04637-129">Essa função deve ser chamada depois que a **nova** função é chamada, mas antes de qualquer outra função de **ChkSGFiles** ser chamada.</span><span class="sxs-lookup"><span data-stu-id="04637-129">This function must be called after the **New** function is called but before any other **ChkSGFiles** function is called.</span></span> 
  
<span data-ttu-id="04637-130">Você deve fornecer todos os nomes de banco de dados, o caminho do arquivo de log e o nome base como cadeias de caracteres Unicode terminadas por caractere nulo.</span><span class="sxs-lookup"><span data-stu-id="04637-130">You must provide all the database names, the log file path, and the base name as null-terminated Unicode strings.</span></span>
  
<span data-ttu-id="04637-131">Você pode verificar somente os arquivos de banco de dados, somente os arquivos de log ou os arquivos de log e de banco de dados.</span><span class="sxs-lookup"><span data-stu-id="04637-131">You can check only the database files, only the log files, or both the database and log files.</span></span> <span data-ttu-id="04637-132">No entanto, ao chamar essa função, o aplicativo deve especificar pelo menos uma entidade a ser verificada.</span><span class="sxs-lookup"><span data-stu-id="04637-132">However, when calling this function, the application must specify at least one entity to be checked.</span></span> <span data-ttu-id="04637-133">Passar 0 (zero) para **cDB** e NULL para **wszLogPath** retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="04637-133">Passing 0 (zero) for  **cDB**  and NULL for  **wszLogPath**  will return an error.</span></span> 
  
<span data-ttu-id="04637-134">Se o valor de **cDB** for diferente de 0 (zero), passar NULL para **rgwszDb** resultará em um erro.</span><span class="sxs-lookup"><span data-stu-id="04637-134">If the value of  **cDB**  is other than 0 (zero), passing NULL for  **rgwszDb**  will result in an error.</span></span> <span data-ttu-id="04637-135">Para verificar os arquivos do banco de dados, o aplicativo deve fornecer os nomes do banco de dados.</span><span class="sxs-lookup"><span data-stu-id="04637-135">To check the database files, the application must provide the database names.</span></span> 
  
<span data-ttu-id="04637-136">Se NULL for passado para **wszBaseName** mas **WSZLOGPATH** não for nulo, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="04637-136">If NULL is passed for  **wszBaseName**  but  **wszLogPath**  is not NULL, an error will be returned.</span></span> <span data-ttu-id="04637-137">Um nome base de arquivo de log sempre é necessário ao verificar arquivos de log.</span><span class="sxs-lookup"><span data-stu-id="04637-137">A log file base name is always required when checking log files.</span></span> 
  
<span data-ttu-id="04637-138">Se você estiver usando o CHKSGFILES em um aplicativo multi-threaded, deverá chamar a função **ErrInit** na parte de thread único do aplicativo, e poderá chamá-la somente uma vez para cada objeto **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="04637-138">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrInit** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="04637-139">Requirements</span><span class="sxs-lookup"><span data-stu-id="04637-139">Requirements</span></span>

<span data-ttu-id="04637-140">O Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="04637-140">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="04637-141">A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.</span><span class="sxs-lookup"><span data-stu-id="04637-141">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

