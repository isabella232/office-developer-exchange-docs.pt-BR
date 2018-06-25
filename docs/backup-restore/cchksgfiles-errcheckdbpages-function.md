---
title: Função CChkSGFiles.ErrCheckDbPages
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckDbPages
api_type:
- dllExport
ms.assetid: 5e981a7c-28cd-470c-b7eb-606463e9dd05
description: 'Modificado pela última vez: 22 de fevereiro de 2013'
ms.openlocfilehash: f1588b1dbc4bd7e83683fa4432a175405ad17903
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750629"
---
# <a name="cchksgfileserrcheckdbpages-function"></a><span data-ttu-id="780d5-103">Função CChkSGFiles.ErrCheckDbPages</span><span class="sxs-lookup"><span data-stu-id="780d5-103">CChkSGFiles.ErrCheckDbPages function</span></span>

<span data-ttu-id="780d5-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="780d5-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="780d5-105">Valida um intervalo de páginas em um banco de dados especificado.</span><span class="sxs-lookup"><span data-stu-id="780d5-105">Validates a range of pages in a specified database.</span></span> 
  
```cs
Vitual ERRErrCheckDbPages  
(
    Const ULONGiDb,
    Const VOID  * const pvPageBuffer,
    Const ULONGcbPageBuffer,
    PAGE_INFOrgPageInfo[],
    Const ULONGcPageInfo,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="780d5-106">Par�metros</span><span class="sxs-lookup"><span data-stu-id="780d5-106">Parameters</span></span>

### <a name="idb"></a><span data-ttu-id="780d5-107">iDb</span><span class="sxs-lookup"><span data-stu-id="780d5-107">iDb</span></span>
  
<span data-ttu-id="780d5-108">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="780d5-108">Input parameter.</span></span> <span data-ttu-id="780d5-109">Um índice na matriz de bancos de dados especificado no parâmetro **[] de rgwszDb** para a função **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="780d5-109">An index into the array of databases specified in the **rgwszDb[]** parameter to the **ErrInit** function.</span></span> <span data-ttu-id="780d5-110">O banco de dados indexado por esse parâmetro será verificado.</span><span class="sxs-lookup"><span data-stu-id="780d5-110">The database indexed by this parameter will be checked.</span></span> 
    
### <a name="pvpagebuffer"></a><span data-ttu-id="780d5-111">pvPageBuffer</span><span class="sxs-lookup"><span data-stu-id="780d5-111">pvPageBuffer</span></span> 
  
<span data-ttu-id="780d5-112">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="780d5-112">Input parameter.</span></span> <span data-ttu-id="780d5-113">Um ponteiro para um buffer que contém uma ou mais páginas de banco de dados a ser verificado.</span><span class="sxs-lookup"><span data-stu-id="780d5-113">A pointer to a buffer containing one or more database pages to be checked.</span></span> <span data-ttu-id="780d5-114">O tamanho do buffer deve ser um múltiplo do tamanho de página do banco de dados, conforme retornado no parâmetro **pcbDbPageSize** pela função **ErrCheckDbHeaders** .</span><span class="sxs-lookup"><span data-stu-id="780d5-114">The size of the buffer must be a multiple of the database page size, as returned in the **pcbDbPageSize** parameter by the **ErrCheckDbHeaders** function.</span></span> <span data-ttu-id="780d5-115">O aplicativo de chamada deve espaço em buffer com o conteúdo de página do banco de dados antes de chamar **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="780d5-115">The calling application must fill the buffer with the database page contents before calling **ErrCheckDbPages**.</span></span>
    
### <a name="cbpagebuffer"></a><span data-ttu-id="780d5-116">cbPageBuffer</span><span class="sxs-lookup"><span data-stu-id="780d5-116">cbPageBuffer</span></span>
  
<span data-ttu-id="780d5-117">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="780d5-117">Input parameter.</span></span> <span data-ttu-id="780d5-118">O tamanho do parâmetro **pvPageBuffer** , em bytes.</span><span class="sxs-lookup"><span data-stu-id="780d5-118">The size of the **pvPageBuffer** parameter, in bytes.</span></span> <span data-ttu-id="780d5-119">Este valor deve ser um múltiplo do tamanho de página do banco de dados, conforme retornado no parâmetro **pcbDbPageSize** pela função **ErrCheckDbHeaders** .</span><span class="sxs-lookup"><span data-stu-id="780d5-119">This value must be a multiple of the database page size, as returned in the **pcbDbPageSize** parameter by the **ErrCheckDbHeaders** function.</span></span> 
    
### <a name="rgpageinfo"></a><span data-ttu-id="780d5-120">[] de rgPageInfo</span><span class="sxs-lookup"><span data-stu-id="780d5-120">rgPageInfo[]</span></span> 
  
<span data-ttu-id="780d5-121">Parâmetro de entrada/saída.</span><span class="sxs-lookup"><span data-stu-id="780d5-121">Input/output parameter.</span></span> <span data-ttu-id="780d5-122">Uma matriz de **página\_INFO** detalhada de estruturas **ErrCheckDbPages** preenche com resultados de cada página de banco de dados que está marcada.</span><span class="sxs-lookup"><span data-stu-id="780d5-122">An array of **PAGE\_INFO** structures that **ErrCheckDbPages** fills with detailed results of each database page that is checked.</span></span> <span data-ttu-id="780d5-123">A matriz deve ter um elemento para cada página de banco de dados passado para o parâmetro **pvPageBuffer** e o campo **ulPgno** em cada **página\_INFO** estrutura deve ser definida como o número de página lógica que corresponde à página de banco de dados.</span><span class="sxs-lookup"><span data-stu-id="780d5-123">The array must have one element for each database page passed in the **pvPageBuffer** parameter, and the **ulPgno** field in each **PAGE\_INFO** structure must be set to the logical page number that corresponds to the database page.</span></span> <span data-ttu-id="780d5-124">Para obter mais informações, consulte "Comentários" mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="780d5-124">For more information, see "Remarks" later in this topic.</span></span> 
    
### <a name="cpageinfo"></a><span data-ttu-id="780d5-125">cPageInfo</span><span class="sxs-lookup"><span data-stu-id="780d5-125">cPageInfo</span></span>
  
<span data-ttu-id="780d5-126">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="780d5-126">Input parameter.</span></span> <span data-ttu-id="780d5-127">O número de entradas na matriz **[] de rgPageInfo** .</span><span class="sxs-lookup"><span data-stu-id="780d5-127">The number of entries in the **rgPageInfo[]** array.</span></span> <span data-ttu-id="780d5-128">Este valor deve ser igual ao número de páginas de banco de dados passada no parâmetro **pvPageBuffer** .</span><span class="sxs-lookup"><span data-stu-id="780d5-128">This value must be equal to the number of database pages passed in the **pvPageBuffer** parameter.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="780d5-129">ulFlags</span><span class="sxs-lookup"><span data-stu-id="780d5-129">ulFlags</span></span> 
  
<span data-ttu-id="780d5-130">Parâmetro de entrada opcional.</span><span class="sxs-lookup"><span data-stu-id="780d5-130">Optional input parameter.</span></span> <span data-ttu-id="780d5-131">Esse valor é reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="780d5-131">This value is reserved for future use.</span></span> <span data-ttu-id="780d5-132">O valor passado neste parâmetro deve ser de 0 (zero).</span><span class="sxs-lookup"><span data-stu-id="780d5-132">The value passed in this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="780d5-133">Valor retornado</span><span class="sxs-lookup"><span data-stu-id="780d5-133">Return value</span></span>

<span data-ttu-id="780d5-134">Um código de erro da enumeração [ERR](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="780d5-134">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="780d5-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="780d5-135">Remarks</span></span>

<span data-ttu-id="780d5-136">Observe que você precisa especificar o banco de dados na matriz de bancos de dados passado para a função **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="780d5-136">Note that you need to have specified the database in the array of databases passed to the **ErrInit** function.</span></span> <span data-ttu-id="780d5-137">Além disso, **ErrCheckDbHeaders** deve ser chamado antes de **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="780d5-137">Also, **ErrCheckDbHeaders** must be called before **ErrCheckDbPages**.</span></span>
  
<span data-ttu-id="780d5-138">O aplicativo de chamada deve alocar um buffer de memória que é grande o suficiente para armazenar as páginas do banco de dados a ser verificado.</span><span class="sxs-lookup"><span data-stu-id="780d5-138">The calling application must allocate a memory buffer that is large enough to hold the database pages to be checked.</span></span> <span data-ttu-id="780d5-139">O aplicativo é responsável por preencher o buffer com o conteúdo de uma ou mais dessas páginas de banco de dados.</span><span class="sxs-lookup"><span data-stu-id="780d5-139">The application is responsible for filling the buffer with the contents of one or more such database pages.</span></span> 
  
<span data-ttu-id="780d5-140">O aplicativo de chamada deve chamar **ErrCheckDbHeaders** antes de chamar **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="780d5-140">The calling application must call **ErrCheckDbHeaders** before calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="780d5-141">Esta função pode ser chamada quantas vezes forem necessárias para cobrir todas as páginas em todos os arquivos de banco de dados que devem ser verificado.</span><span class="sxs-lookup"><span data-stu-id="780d5-141">This function can be called as many times as necessary to cover all the pages in all database files that are to be checked.</span></span>
  
<span data-ttu-id="780d5-142">No parâmetro **[] de rgPageInfo** , cada elemento retornado contém informações sobre a página de banco de dados em um **página\_INFO** estrutura.</span><span class="sxs-lookup"><span data-stu-id="780d5-142">In the **rgPageInfo[]** parameter, each element returned contains information about the database page in a **PAGE\_INFO** structure.</span></span> <span data-ttu-id="780d5-143">Se a função de **ErrCheckDbPages** retornará um erro, o aplicativo deve verificar cada **página\_INFO** estrutura para determinar em qual página o erro foi encontrado.</span><span class="sxs-lookup"><span data-stu-id="780d5-143">If the **ErrCheckDbPages** function returns an error, the application should check each **PAGE\_INFO** structure to determine on which page the error was found.</span></span> <span data-ttu-id="780d5-144">Por exemplo, comparar os valores **checksumActual** e **checksumExpected** indicará se foi detectado um erro de soma de verificação nessa página de banco de dados.</span><span class="sxs-lookup"><span data-stu-id="780d5-144">For example, comparing the **checksumActual** and **checksumExpected** values will indicate whether a checksum error was detected on that database page.</span></span> 
  
<span data-ttu-id="780d5-145">Se **ErrCheckDbPages** detecta quaisquer erros no conteúdo do banco de dados, ele cria uma entrada de log de eventos de erro do Windows.</span><span class="sxs-lookup"><span data-stu-id="780d5-145">If **ErrCheckDbPages** detects any errors in the database content, it will create a Windows Error event log entry.</span></span> 
  
<span data-ttu-id="780d5-146">O objeto **CChkSGFiles** determina se todos os bancos de dados registrados com a função **ErrInit** realmente marcados.</span><span class="sxs-lookup"><span data-stu-id="780d5-146">The **CChkSGFiles** object determines whether all the databases registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="780d5-147">Especificamente, **CChkSGFiles** usa a função **ErrCheckDbPages** para determinar se o mesmo número de páginas de banco de dados indicado pelo **ErrCheckDbHeaders** realmente foram verificado.</span><span class="sxs-lookup"><span data-stu-id="780d5-147">Specifically, **CChkSGFiles** uses the **ErrCheckDbPages** function to determine whether the same number of database pages indicated by **ErrCheckDbHeaders** were actually verified.</span></span> <span data-ttu-id="780d5-148">Se o número correto das páginas em cada banco de dados não foram verificado com êxito, a função de **ErrTerm** retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="780d5-148">If the correct number of pages in each database were not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="780d5-149">Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você pode chamar a função **ErrCheckDbPages** na parte multithread do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="780d5-149">If you're using CHKSGFILES in a multithreaded application, you can call the **ErrCheckDbPages** function in the multithreaded portion of the application.</span></span> <span data-ttu-id="780d5-150">Observe que **ErrCheckDbPages** é geralmente chamado várias vezes para cada banco de dados está marcado.</span><span class="sxs-lookup"><span data-stu-id="780d5-150">Note that **ErrCheckDbPages** is typically called multiple times for each database that is checked.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="780d5-151">Requisitos</span><span class="sxs-lookup"><span data-stu-id="780d5-151">Requirements</span></span>

<span data-ttu-id="780d5-152">Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="780d5-152">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="780d5-153">A conta que o aplicativo está sendo executado em deve ter permissões de leitura para os arquivos de log e de banco de dados que devem ser verificado.</span><span class="sxs-lookup"><span data-stu-id="780d5-153">The account that the application is running under must have read permissions to the database and log files that are to be checked.</span></span>
  

