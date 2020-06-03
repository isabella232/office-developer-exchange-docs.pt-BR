---
title: Função função cchksgfiles. ErrCheckLogs
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckLogs
api_type:
- dllExport
ms.assetid: cec0df4b-4679-4682-bacf-69b4f4aef343
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: 71e21bb3a748a532f9e3167e0b36898acde71b02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526715"
---
# <a name="cchksgfileserrchecklogs-function"></a><span data-ttu-id="8899d-103">Função função cchksgfiles. ErrCheckLogs</span><span class="sxs-lookup"><span data-stu-id="8899d-103">CChkSGFiles.ErrCheckLogs function</span></span>

<span data-ttu-id="8899d-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="8899d-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="8899d-105">Valida os arquivos de log de todos os arquivos de banco de dados que foram especificados na função **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="8899d-105">Validates the log files of all the database files that were specified in the **ErrInit** function.</span></span> <span data-ttu-id="8899d-106">Os logs validados são aqueles que existem no caminho e que têm o nome do arquivo de log base de três letras passado para **ErrInit**.</span><span class="sxs-lookup"><span data-stu-id="8899d-106">The validated logs are those that exist in the path, and that have the three-letter base log file name passed to **ErrInit**.</span></span>
  
```cs
Vitual ERRErrCheckLogs 
(
        BOOL  * const pfOnlyUnnecessaryLogsCorrup,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="8899d-107">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="8899d-107">Parameters</span></span>

### <a name="pfonlyunnecessarylogscorrupt"></a><span data-ttu-id="8899d-108">pfOnlyUnnecessaryLogsCorrupt</span><span class="sxs-lookup"><span data-stu-id="8899d-108">pfOnlyUnnecessaryLogsCorrupt</span></span> 
  
<span data-ttu-id="8899d-109">Parâmetro de saída.</span><span class="sxs-lookup"><span data-stu-id="8899d-109">Output parameter.</span></span> <span data-ttu-id="8899d-110">Quando **true**, este parâmetro indica que foram encontrados erros nos arquivos de log de transações, mas esses erros foram encontrados nos arquivos de log que não são necessários para trazer o banco de dados para um estado de desligamento normal sem perda de dados.</span><span class="sxs-lookup"><span data-stu-id="8899d-110">When **true**, this parameter indicates that errors were found in the transaction log files, but those errors were all found in log files that are not needed to bring the database to a clean-shutdown state without data loss.</span></span> <span data-ttu-id="8899d-111">Um valor **true** retornado nesse parâmetro é válido somente quando **ErrCheckLogs** retorna **errSuccess**.</span><span class="sxs-lookup"><span data-stu-id="8899d-111">A **true** value returned in this parameter is valid only when **ErrCheckLogs** returns **errSuccess**.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="8899d-112">ulFlags</span><span class="sxs-lookup"><span data-stu-id="8899d-112">ulFlags</span></span>
  
<span data-ttu-id="8899d-113">Parâmetro de entrada opcional.</span><span class="sxs-lookup"><span data-stu-id="8899d-113">Optional input parameter.</span></span> <span data-ttu-id="8899d-114">Esse valor é reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="8899d-114">This value is reserved for future use.</span></span> <span data-ttu-id="8899d-115">O valor passado por esse parâmetro deve ser 0 (zero).</span><span class="sxs-lookup"><span data-stu-id="8899d-115">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="8899d-116">Valor de retorno</span><span class="sxs-lookup"><span data-stu-id="8899d-116">Return value</span></span>

<span data-ttu-id="8899d-117">Um código de erro da enumeração [Err](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="8899d-117">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
<span data-ttu-id="8899d-118">É importante lembrar que essa função pode retornar **errSuccess** mesmo quando são encontrados erros nos arquivos de log.</span><span class="sxs-lookup"><span data-stu-id="8899d-118">It's important to remember that this function can return **errSuccess** even when errors are found in the log files.</span></span> <span data-ttu-id="8899d-119">Portanto, quando **ErrCheckLogs** retornar **errSuccess**, o aplicativo também deverá verificar o parâmetro de retorno **pfOnlyUnnecessaryLogsCorrupt** .</span><span class="sxs-lookup"><span data-stu-id="8899d-119">Therefore, when **ErrCheckLogs** returns **errSuccess**, the application should also check the  **pfOnlyUnnecessaryLogsCorrupt** return parameter.</span></span> <span data-ttu-id="8899d-120">Se **pfOnlyUnnecessaryLogsCorrupts** for **true** quando **ErrCheckLogs** retornar **errSuccess**, isso indica que um ou mais erros foram encontrados, mas apenas em arquivos de log não são necessários para atualizar o banco de dados.</span><span class="sxs-lookup"><span data-stu-id="8899d-120">If **pfOnlyUnnecessaryLogsCorrupts** is **true** when **ErrCheckLogs** returns **errSuccess**, this indicates that one or more errors were found, but only in log files not needed to bring the database up-to-date.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8899d-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="8899d-121">Remarks</span></span>

<span data-ttu-id="8899d-122">A função **ErrCheckDbHeaders** deve ser chamada para que a função **ErrCheckLogs** possa ser chamada.</span><span class="sxs-lookup"><span data-stu-id="8899d-122">The **ErrCheckDbHeaders** function must be called before the **ErrCheckLogs** function can be called.</span></span> 
  
<span data-ttu-id="8899d-123">Quando os arquivos de log de transações do banco de dados do Exchange estiverem sendo verificados, alguns dos arquivos de log serão necessários para colocar os bancos de dados no grupo de armazenamento em um estado de desligamento normal sem perda de dados, enquanto outros arquivos de log podem não ser necessários.</span><span class="sxs-lookup"><span data-stu-id="8899d-123">When Exchange database transaction log files are being checked, some of the log files will be necessary to bring the databases in the storage group to a clean-shutdown state without data loss, whereas other log files might not be needed.</span></span> <span data-ttu-id="8899d-124">A função **ErrCheckLogs** determina tanto os arquivos de log mais antigos quanto os mais recentes necessários para atualizar os bancos de dados.</span><span class="sxs-lookup"><span data-stu-id="8899d-124">The **ErrCheckLogs** function determines both the oldest and the newest log files that are needed to bring the databases up to date.</span></span> 
  
<span data-ttu-id="8899d-125">A função **ErrCheckLogs** verifica todos os arquivos de log nos caminhos especificados que também têm o nome de arquivo base de três letras especificado, conforme passado para a função **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="8899d-125">The **ErrCheckLogs** function verifies all the log files in the specified paths that also have the specified three-letter base file name, as passed to the **ErrInit** function.</span></span> 
  
<span data-ttu-id="8899d-126">Se nenhum erro for encontrado nos arquivos de log, **ErrCheckLogs** retornará **errSuccess**.</span><span class="sxs-lookup"><span data-stu-id="8899d-126">If no errors are found in the log files, **ErrCheckLogs** returns **errSuccess**.</span></span> 
  
<span data-ttu-id="8899d-127">Se qualquer um dos arquivos de log necessários estiver corrompido, **ErrCheckLogs** retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="8899d-127">If any of the required log files are found to be corrupted, **ErrCheckLogs** returns an error.</span></span> 
  
<span data-ttu-id="8899d-128">Se forem encontrados erros somente nos arquivos de log que sejam mais antigos do que o mais antigo necessário, a função retornará **errSuccess** e definirá o parâmetro de retorno **pfOnlyUnnecessaryLogCorrupt** como **true**.</span><span class="sxs-lookup"><span data-stu-id="8899d-128">If errors are found only in log files that are older than the earliest ones needed, the function returns **errSuccess** and sets the return parameter **pfOnlyUnnecessaryLogCorrupt** to **true**.</span></span> <span data-ttu-id="8899d-129">O aplicativo deve reconhecer que há erros em alguns desses arquivos de log antigos e, em caso afirmativo, ele possivelmente alertará o usuário.</span><span class="sxs-lookup"><span data-stu-id="8899d-129">The application should recognize that there are errors in some of those old log files, and if so, it will possibly alert the user.</span></span> <span data-ttu-id="8899d-130">Em qualquer caso, esses erros não devem afetar a integridade geral do banco de dados ou afetam se a execução do envio dos logs será bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="8899d-130">In any case, those errors should not affect the overall integrity of the database or affect whether playing the logs forward will succeed.</span></span>
  
<span data-ttu-id="8899d-131">Se forem encontrados erros em qualquer arquivo de log criado depois que o primeiro log que **ErrCheckLogs** determina for necessário, a função retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="8899d-131">If errors are found in any log file created after the earliest log that **ErrCheckLogs** determines is needed, the function returns an error.</span></span> <span data-ttu-id="8899d-132">O erro será retornado mesmo se o erro do arquivo de log foi encontrado em um arquivo de log que foi gerado mais tarde do que o necessário para atualizar o banco de dados.</span><span class="sxs-lookup"><span data-stu-id="8899d-132">The error will be returned even if the log file error was found in a log file that was generated later than what is needed to bring the database up to date.</span></span> <span data-ttu-id="8899d-133">Embora seja possível trazer os bancos de dados para um estado de desligamento normal usando os arquivos de log identificados, as transações especificadas nos arquivos de log corrompidos posteriormente não seriam aplicadas, resultando em perda de dados quando o banco de dados é restaurado.</span><span class="sxs-lookup"><span data-stu-id="8899d-133">Although it would be possible to bring the databases to a clean-shutdown state by using the identified log files, transactions specified in the later corrupted log files would not be applied, resulting in data loss when the database is restored.</span></span> 
  
<span data-ttu-id="8899d-134">O objeto **função cchksgfiles** determina se todos os arquivos de log registrados na função **ErrInit** foram realmente verificados.</span><span class="sxs-lookup"><span data-stu-id="8899d-134">The **CChkSGFiles** object determines whether all of the log files registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="8899d-135">Se nem todos os logs não foram verificados com êxito, a função **ErrTerm** retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="8899d-135">If not all of the logs were not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="8899d-136">Se você estiver usando o CHKSGFILES em um aplicativo multi-threaded, poderá chamar a função **ErrCheckLogs** na parte multithread do aplicativo, mas poderá chamá-la apenas uma vez para cada objeto **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="8899d-136">If you're using CHKSGFILES in a multithreaded application, you can call the **ErrCheckLogs** function in the multithreaded portion of the application, but you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="8899d-137">Requirements</span><span class="sxs-lookup"><span data-stu-id="8899d-137">Requirements</span></span>

<span data-ttu-id="8899d-138">O Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="8899d-138">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="8899d-139">A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.</span><span class="sxs-lookup"><span data-stu-id="8899d-139">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

