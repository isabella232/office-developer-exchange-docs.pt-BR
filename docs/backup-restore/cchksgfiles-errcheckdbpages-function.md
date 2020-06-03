---
title: Função função cchksgfiles. ErrCheckDbPages
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
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: 78d2dbee6253096d597b4ec2de3878f40ee1b6d7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526722"
---
# <a name="cchksgfileserrcheckdbpages-function"></a><span data-ttu-id="487b6-103">Função função cchksgfiles. ErrCheckDbPages</span><span class="sxs-lookup"><span data-stu-id="487b6-103">CChkSGFiles.ErrCheckDbPages function</span></span>

<span data-ttu-id="487b6-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="487b6-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="487b6-105">Valida um intervalo de páginas em um banco de dados especificado.</span><span class="sxs-lookup"><span data-stu-id="487b6-105">Validates a range of pages in a specified database.</span></span> 
  
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

## <a name="parameters"></a><span data-ttu-id="487b6-106">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="487b6-106">Parameters</span></span>

### <a name="idb"></a><span data-ttu-id="487b6-107">iDb</span><span class="sxs-lookup"><span data-stu-id="487b6-107">iDb</span></span>
  
<span data-ttu-id="487b6-108">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="487b6-108">Input parameter.</span></span> <span data-ttu-id="487b6-109">Um índice na matriz de bancos de dados especificado no parâmetro **rgwszDb []** para a função **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="487b6-109">An index into the array of databases specified in the **rgwszDb[]** parameter to the **ErrInit** function.</span></span> <span data-ttu-id="487b6-110">O banco de dados indexado por esse parâmetro será verificado.</span><span class="sxs-lookup"><span data-stu-id="487b6-110">The database indexed by this parameter will be checked.</span></span> 
    
### <a name="pvpagebuffer"></a><span data-ttu-id="487b6-111">pvPageBuffer</span><span class="sxs-lookup"><span data-stu-id="487b6-111">pvPageBuffer</span></span> 
  
<span data-ttu-id="487b6-112">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="487b6-112">Input parameter.</span></span> <span data-ttu-id="487b6-113">Um ponteiro para um buffer contendo uma ou mais páginas de banco de dados a serem verificadas.</span><span class="sxs-lookup"><span data-stu-id="487b6-113">A pointer to a buffer containing one or more database pages to be checked.</span></span> <span data-ttu-id="487b6-114">O tamanho do buffer deve ser um múltiplo do tamanho da página do banco de dados, conforme retornado no parâmetro **pcbDbPageSize** pela função **ErrCheckDbHeaders** .</span><span class="sxs-lookup"><span data-stu-id="487b6-114">The size of the buffer must be a multiple of the database page size, as returned in the **pcbDbPageSize** parameter by the **ErrCheckDbHeaders** function.</span></span> <span data-ttu-id="487b6-115">O aplicativo de chamada deve preencher o buffer com o conteúdo da página do banco de dados antes de chamar **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="487b6-115">The calling application must fill the buffer with the database page contents before calling **ErrCheckDbPages**.</span></span>
    
### <a name="cbpagebuffer"></a><span data-ttu-id="487b6-116">cbPageBuffer</span><span class="sxs-lookup"><span data-stu-id="487b6-116">cbPageBuffer</span></span>
  
<span data-ttu-id="487b6-117">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="487b6-117">Input parameter.</span></span> <span data-ttu-id="487b6-118">O tamanho do parâmetro **pvPageBuffer** , em bytes.</span><span class="sxs-lookup"><span data-stu-id="487b6-118">The size of the **pvPageBuffer** parameter, in bytes.</span></span> <span data-ttu-id="487b6-119">Esse valor deve ser um múltiplo do tamanho da página do banco de dados, conforme retornado no parâmetro **pcbDbPageSize** pela função **ErrCheckDbHeaders** .</span><span class="sxs-lookup"><span data-stu-id="487b6-119">This value must be a multiple of the database page size, as returned in the **pcbDbPageSize** parameter by the **ErrCheckDbHeaders** function.</span></span> 
    
### <a name="rgpageinfo"></a><span data-ttu-id="487b6-120">rgPageInfo[]</span><span class="sxs-lookup"><span data-stu-id="487b6-120">rgPageInfo[]</span></span> 
  
<span data-ttu-id="487b6-121">Parâmetro de entrada/saída.</span><span class="sxs-lookup"><span data-stu-id="487b6-121">Input/output parameter.</span></span> <span data-ttu-id="487b6-122">Uma matriz de estruturas de \*\* \_ informações de página\*\* que **ErrCheckDbPages** preenche com resultados detalhados de cada página de banco de dados verificada.</span><span class="sxs-lookup"><span data-stu-id="487b6-122">An array of **PAGE\_INFO** structures that **ErrCheckDbPages** fills with detailed results of each database page that is checked.</span></span> <span data-ttu-id="487b6-123">A matriz deve ter um elemento para cada página de banco de dados aprovada no parâmetro **pvPageBuffer** , e o campo **ulPgno** em cada estrutura de \*\* \_ informações de página\*\* deve ser definido como o número de página lógica que corresponde à página do banco de dados.</span><span class="sxs-lookup"><span data-stu-id="487b6-123">The array must have one element for each database page passed in the **pvPageBuffer** parameter, and the **ulPgno** field in each **PAGE\_INFO** structure must be set to the logical page number that corresponds to the database page.</span></span> <span data-ttu-id="487b6-124">Para obter mais informações, consulte "Comentários", mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="487b6-124">For more information, see "Remarks" later in this topic.</span></span> 
    
### <a name="cpageinfo"></a><span data-ttu-id="487b6-125">cPageInfo</span><span class="sxs-lookup"><span data-stu-id="487b6-125">cPageInfo</span></span>
  
<span data-ttu-id="487b6-126">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="487b6-126">Input parameter.</span></span> <span data-ttu-id="487b6-127">O número de entradas na matriz **rgPageInfo []** .</span><span class="sxs-lookup"><span data-stu-id="487b6-127">The number of entries in the **rgPageInfo[]** array.</span></span> <span data-ttu-id="487b6-128">Esse valor deve ser igual ao número de páginas de banco de dados passadas no parâmetro **pvPageBuffer** .</span><span class="sxs-lookup"><span data-stu-id="487b6-128">This value must be equal to the number of database pages passed in the **pvPageBuffer** parameter.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="487b6-129">ulFlags</span><span class="sxs-lookup"><span data-stu-id="487b6-129">ulFlags</span></span> 
  
<span data-ttu-id="487b6-130">Parâmetro de entrada opcional.</span><span class="sxs-lookup"><span data-stu-id="487b6-130">Optional input parameter.</span></span> <span data-ttu-id="487b6-131">Esse valor é reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="487b6-131">This value is reserved for future use.</span></span> <span data-ttu-id="487b6-132">O valor passado nesse parâmetro deve ser 0 (zero).</span><span class="sxs-lookup"><span data-stu-id="487b6-132">The value passed in this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="487b6-133">Valor de retorno</span><span class="sxs-lookup"><span data-stu-id="487b6-133">Return value</span></span>

<span data-ttu-id="487b6-134">Um código de erro da enumeração [Err](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="487b6-134">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="487b6-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="487b6-135">Remarks</span></span>

<span data-ttu-id="487b6-136">Observe que você precisa ter especificado o banco de dados na matriz de bancos de dados passada para a função **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="487b6-136">Note that you need to have specified the database in the array of databases passed to the **ErrInit** function.</span></span> <span data-ttu-id="487b6-137">Além disso, **ErrCheckDbHeaders** deve ser chamado antes de **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="487b6-137">Also, **ErrCheckDbHeaders** must be called before **ErrCheckDbPages**.</span></span>
  
<span data-ttu-id="487b6-138">O aplicativo de chamada deve alocar um buffer de memória grande o suficiente para armazenar as páginas do banco de dados a serem verificadas.</span><span class="sxs-lookup"><span data-stu-id="487b6-138">The calling application must allocate a memory buffer that is large enough to hold the database pages to be checked.</span></span> <span data-ttu-id="487b6-139">O aplicativo é responsável por preencher o buffer com o conteúdo de uma ou mais dessas páginas de banco de dados.</span><span class="sxs-lookup"><span data-stu-id="487b6-139">The application is responsible for filling the buffer with the contents of one or more such database pages.</span></span> 
  
<span data-ttu-id="487b6-140">O aplicativo de chamada deve chamar **ErrCheckDbHeaders** antes de chamar **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="487b6-140">The calling application must call **ErrCheckDbHeaders** before calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="487b6-141">Essa função pode ser chamada quantas vezes forem necessárias para abranger todas as páginas em todos os arquivos de banco de dados que devem ser verificados.</span><span class="sxs-lookup"><span data-stu-id="487b6-141">This function can be called as many times as necessary to cover all the pages in all database files that are to be checked.</span></span>
  
<span data-ttu-id="487b6-142">No parâmetro **rgPageInfo []** , cada elemento retornado contém informações sobre a página do banco de dados em uma estrutura de \*\* \_ informações da página\*\* .</span><span class="sxs-lookup"><span data-stu-id="487b6-142">In the **rgPageInfo[]** parameter, each element returned contains information about the database page in a **PAGE\_INFO** structure.</span></span> <span data-ttu-id="487b6-143">Se a função **ErrCheckDbPages** retornar um erro, o aplicativo deve verificar cada estrutura de \*\* \_ informações da página\*\* para determinar em qual página o erro foi encontrado.</span><span class="sxs-lookup"><span data-stu-id="487b6-143">If the **ErrCheckDbPages** function returns an error, the application should check each **PAGE\_INFO** structure to determine on which page the error was found.</span></span> <span data-ttu-id="487b6-144">Por exemplo, comparar os valores **checksumActual** e **checksumExpected** indicará se um erro de checksum foi detectado na página do banco de dados.</span><span class="sxs-lookup"><span data-stu-id="487b6-144">For example, comparing the **checksumActual** and **checksumExpected** values will indicate whether a checksum error was detected on that database page.</span></span> 
  
<span data-ttu-id="487b6-145">Se o **ErrCheckDbPages** detectar qualquer erro no conteúdo do banco de dados, ele criará uma entrada do log de eventos de erro do Windows.</span><span class="sxs-lookup"><span data-stu-id="487b6-145">If **ErrCheckDbPages** detects any errors in the database content, it will create a Windows Error event log entry.</span></span> 
  
<span data-ttu-id="487b6-146">O objeto **função cchksgfiles** determina se todos os bancos de dados registrados com a função **ErrInit** foram realmente verificados.</span><span class="sxs-lookup"><span data-stu-id="487b6-146">The **CChkSGFiles** object determines whether all the databases registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="487b6-147">Especificamente, **função cchksgfiles** usa a função **ErrCheckDbPages** para determinar se o mesmo número de páginas de banco de dados indicadas por **ErrCheckDbHeaders** foram realmente verificadas.</span><span class="sxs-lookup"><span data-stu-id="487b6-147">Specifically, **CChkSGFiles** uses the **ErrCheckDbPages** function to determine whether the same number of database pages indicated by **ErrCheckDbHeaders** were actually verified.</span></span> <span data-ttu-id="487b6-148">Se o número correto de páginas em cada banco de dados não foi verificado com êxito, a função **ErrTerm** retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="487b6-148">If the correct number of pages in each database were not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="487b6-149">Se você estiver usando o CHKSGFILES em um aplicativo multi-threaded, poderá chamar a função **ErrCheckDbPages** na parte multithread do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="487b6-149">If you're using CHKSGFILES in a multithreaded application, you can call the **ErrCheckDbPages** function in the multithreaded portion of the application.</span></span> <span data-ttu-id="487b6-150">Observe que **ErrCheckDbPages** normalmente é chamado várias vezes para cada banco de dados selecionado.</span><span class="sxs-lookup"><span data-stu-id="487b6-150">Note that **ErrCheckDbPages** is typically called multiple times for each database that is checked.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="487b6-151">Requirements</span><span class="sxs-lookup"><span data-stu-id="487b6-151">Requirements</span></span>

<span data-ttu-id="487b6-152">O Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="487b6-152">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="487b6-153">A conta sob a qual o aplicativo está sendo executado deve ter permissões de leitura para o banco de dados e arquivos de log que devem ser verificados.</span><span class="sxs-lookup"><span data-stu-id="487b6-153">The account that the application is running under must have read permissions to the database and log files that are to be checked.</span></span>
  

