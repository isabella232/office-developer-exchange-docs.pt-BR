---
title: Função CChkSGFiles.ErrCheckLogs
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
description: 'Modificado pela última vez: 22 de fevereiro de 2013'
ms.openlocfilehash: 5b1070de73bc23ae09ddb7835bd72c8e8a71a95f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750632"
---
# <a name="cchksgfileserrchecklogs-function"></a><span data-ttu-id="172a3-103">Função CChkSGFiles.ErrCheckLogs</span><span class="sxs-lookup"><span data-stu-id="172a3-103">CChkSGFiles.ErrCheckLogs function</span></span>

<span data-ttu-id="172a3-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="172a3-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="172a3-105">Valida os arquivos de log de todos os arquivos de banco de dados que foram especificados na função **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="172a3-105">Validates the log files of all the database files that were specified in the **ErrInit** function.</span></span> <span data-ttu-id="172a3-106">Os logs validados são aqueles que existir no caminho e que possuírem o nome do arquivo de log de base de três letras passado para **ErrInit**.</span><span class="sxs-lookup"><span data-stu-id="172a3-106">The validated logs are those that exist in the path, and that have the three-letter base log file name passed to **ErrInit**.</span></span>
  
```cs
Vitual ERRErrCheckLogs 
(
        BOOL  * const pfOnlyUnnecessaryLogsCorrup,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="172a3-107">Par�metros</span><span class="sxs-lookup"><span data-stu-id="172a3-107">Parameters</span></span>

### <a name="pfonlyunnecessarylogscorrupt"></a><span data-ttu-id="172a3-108">pfOnlyUnnecessaryLogsCorrupt</span><span class="sxs-lookup"><span data-stu-id="172a3-108">pfOnlyUnnecessaryLogsCorrupt</span></span> 
  
<span data-ttu-id="172a3-109">Parâmetro de saída.</span><span class="sxs-lookup"><span data-stu-id="172a3-109">Output parameter.</span></span> <span data-ttu-id="172a3-110">Quando **true**, esse parâmetro indica que foram encontrados erros em arquivos de log de transações, mas esses erros foram todas encontradas nos arquivos de log que não são necessários para colocar o banco de dados para um estado de desligamento sem perda de dados.</span><span class="sxs-lookup"><span data-stu-id="172a3-110">When **true**, this parameter indicates that errors were found in the transaction log files, but those errors were all found in log files that are not needed to bring the database to a clean-shutdown state without data loss.</span></span> <span data-ttu-id="172a3-111">Um valor **true** retornado neste parâmetro é válido somente quando **ErrCheckLogs** retorna **errSuccess**.</span><span class="sxs-lookup"><span data-stu-id="172a3-111">A **true** value returned in this parameter is valid only when **ErrCheckLogs** returns **errSuccess**.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="172a3-112">ulFlags</span><span class="sxs-lookup"><span data-stu-id="172a3-112">ulFlags</span></span>
  
<span data-ttu-id="172a3-113">Parâmetro de entrada opcional.</span><span class="sxs-lookup"><span data-stu-id="172a3-113">Optional input parameter.</span></span> <span data-ttu-id="172a3-114">Esse valor é reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="172a3-114">This value is reserved for future use.</span></span> <span data-ttu-id="172a3-115">O valor passado por este parâmetro deve ser de 0 (zero).</span><span class="sxs-lookup"><span data-stu-id="172a3-115">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="172a3-116">Valor retornado</span><span class="sxs-lookup"><span data-stu-id="172a3-116">Return value</span></span>

<span data-ttu-id="172a3-117">Um código de erro da enumeração [ERR](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="172a3-117">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
<span data-ttu-id="172a3-118">É importante lembrar-se de que esta função pode retornar **errSuccess** , mesmo quando são encontrados erros nos arquivos de log.</span><span class="sxs-lookup"><span data-stu-id="172a3-118">It's important to remember that this function can return **errSuccess** even when errors are found in the log files.</span></span> <span data-ttu-id="172a3-119">Portanto, quando **ErrCheckLogs** retorna **errSuccess**, o aplicativo deve também verificar o parâmetro de retorno de **pfOnlyUnnecessaryLogsCorrupt** .</span><span class="sxs-lookup"><span data-stu-id="172a3-119">Therefore, when **ErrCheckLogs** returns **errSuccess**, the application should also check the  **pfOnlyUnnecessaryLogsCorrupt** return parameter.</span></span> <span data-ttu-id="172a3-120">Se **pfOnlyUnnecessaryLogsCorrupts** for **true** quando **ErrCheckLogs** retorna **errSuccess**, isto indica que foram encontrados erros de um ou mais, mas apenas nos arquivos de log que não é necessários colocar o banco de dados atualizado.</span><span class="sxs-lookup"><span data-stu-id="172a3-120">If **pfOnlyUnnecessaryLogsCorrupts** is **true** when **ErrCheckLogs** returns **errSuccess**, this indicates that one or more errors were found, but only in log files not needed to bring the database up-to-date.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="172a3-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="172a3-121">Remarks</span></span>

<span data-ttu-id="172a3-122">A função **ErrCheckDbHeaders** deve ser chamada antes que a função **ErrCheckLogs** pode ser chamada.</span><span class="sxs-lookup"><span data-stu-id="172a3-122">The **ErrCheckDbHeaders** function must be called before the **ErrCheckLogs** function can be called.</span></span> 
  
<span data-ttu-id="172a3-123">Quando os arquivos de log de transações de banco de dados do Exchange estão sendo verificados, alguns dos arquivos de log será necessário colocar os bancos de dados no grupo de armazenamento em um estado de desligamento sem perda de dados, enquanto outros arquivos de log não podem ser necessários.</span><span class="sxs-lookup"><span data-stu-id="172a3-123">When Exchange database transaction log files are being checked, some of the log files will be necessary to bring the databases in the storage group to a clean-shutdown state without data loss, whereas other log files might not be needed.</span></span> <span data-ttu-id="172a3-124">A função **ErrCheckLogs** determina antigos e os arquivos de log mais recentes que são necessárias para tornar os bancos de dados atualizados.</span><span class="sxs-lookup"><span data-stu-id="172a3-124">The **ErrCheckLogs** function determines both the oldest and the newest log files that are needed to bring the databases up to date.</span></span> 
  
<span data-ttu-id="172a3-125">A função **ErrCheckLogs** verifica todos os arquivos de log nos caminhos especificados que também tenham o nome de arquivo especificado de base de três letras, como passados para a função **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="172a3-125">The **ErrCheckLogs** function verifies all the log files in the specified paths that also have the specified three-letter base file name, as passed to the **ErrInit** function.</span></span> 
  
<span data-ttu-id="172a3-126">Se nenhum erro for encontrado nos arquivos de log, **ErrCheckLogs** retorna **errSuccess**.</span><span class="sxs-lookup"><span data-stu-id="172a3-126">If no errors are found in the log files, **ErrCheckLogs** returns **errSuccess**.</span></span> 
  
<span data-ttu-id="172a3-127">Se qualquer um dos arquivos de log exigidos forem encontradas corrompido, **ErrCheckLogs** retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="172a3-127">If any of the required log files are found to be corrupted, **ErrCheckLogs** returns an error.</span></span> 
  
<span data-ttu-id="172a3-128">Se houver erros apenas nos arquivos de log mais antigas que a primeira aqueles necessários, a função retorna **errSuccess** e define o parâmetro de retorno **pfOnlyUnnecessaryLogCorrupt** como **true**.</span><span class="sxs-lookup"><span data-stu-id="172a3-128">If errors are found only in log files that are older than the earliest ones needed, the function returns **errSuccess** and sets the return parameter **pfOnlyUnnecessaryLogCorrupt** to **true**.</span></span> <span data-ttu-id="172a3-129">O aplicativo deve reconhecer que há erros em alguns desses arquivos de log antigo e, em caso afirmativo, ele irá alertá possivelmente o usuário.</span><span class="sxs-lookup"><span data-stu-id="172a3-129">The application should recognize that there are errors in some of those old log files, and if so, it will possibly alert the user.</span></span> <span data-ttu-id="172a3-130">Em qualquer caso, esses erros não devem afetar a integridade geral do banco de dados ou afetam se reproduzir os logs de encaminhar terá êxito.</span><span class="sxs-lookup"><span data-stu-id="172a3-130">In any case, those errors should not affect the overall integrity of the database or affect whether playing the logs forward will succeed.</span></span>
  
<span data-ttu-id="172a3-131">Se houver erros em qualquer arquivo de log criado após a primeira log **ErrCheckLogs** determina é necessária, a função retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="172a3-131">If errors are found in any log file created after the earliest log that **ErrCheckLogs** determines is needed, the function returns an error.</span></span> <span data-ttu-id="172a3-132">O erro será retornado até mesmo se o erro de arquivo de log foi encontrado em um arquivo de log gerado mais recente do que o que é precisava colocar o banco de dados atualizado.</span><span class="sxs-lookup"><span data-stu-id="172a3-132">The error will be returned even if the log file error was found in a log file that was generated later than what is needed to bring the database up to date.</span></span> <span data-ttu-id="172a3-133">Embora seria possível trazer os bancos de dados para um estado de desligamento usando os arquivos de log identificados, especificadas nos arquivos de posteriormente corrompidos log de transações não seriam aplicadas, resultando em perda de dados quando o banco de dados for restaurado.</span><span class="sxs-lookup"><span data-stu-id="172a3-133">Although it would be possible to bring the databases to a clean-shutdown state by using the identified log files, transactions specified in the later corrupted log files would not be applied, resulting in data loss when the database is restored.</span></span> 
  
<span data-ttu-id="172a3-134">O objeto **CChkSGFiles** determina se todos os arquivos de log registrados com a função **ErrInit** realmente marcados.</span><span class="sxs-lookup"><span data-stu-id="172a3-134">The **CChkSGFiles** object determines whether all of the log files registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="172a3-135">Se não todos os logs não foram verificada com êxito, a função **ErrTerm** retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="172a3-135">If not all of the logs were not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="172a3-136">Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você pode chamar a função **ErrCheckLogs** na parte multithread do aplicativo, mas você poderá chamá-lo apenas uma vez para cada objeto **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="172a3-136">If you're using CHKSGFILES in a multithreaded application, you can call the **ErrCheckLogs** function in the multithreaded portion of the application, but you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="172a3-137">Requisitos</span><span class="sxs-lookup"><span data-stu-id="172a3-137">Requirements</span></span>

<span data-ttu-id="172a3-138">Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="172a3-138">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="172a3-139">A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.</span><span class="sxs-lookup"><span data-stu-id="172a3-139">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

