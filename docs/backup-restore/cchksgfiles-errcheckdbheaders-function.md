---
title: Função CChkSGFiles.ErrCheckDbHeaders
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckDbHeaders
api_type:
- dllExport
ms.assetid: 75289cd2-35b1-4f75-a651-dce01f1ddda1
description: 'Modificado pela última vez: 22 de fevereiro de 2013'
ms.openlocfilehash: a407019063b34970e883a00ca4f4d730935d7cba
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750636"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a><span data-ttu-id="d6a3d-103">Função CChkSGFiles.ErrCheckDbHeaders</span><span class="sxs-lookup"><span data-stu-id="d6a3d-103">CChkSGFiles.ErrCheckDbHeaders function</span></span>

<span data-ttu-id="d6a3d-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="d6a3d-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span> 
  
<span data-ttu-id="d6a3d-105">Valida os cabeçalhos dos arquivos de banco de dados que foram especificados pela função **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="d6a3d-105">Validates the headers of the database files that were specified by the **ErrInit** function.</span></span> <span data-ttu-id="d6a3d-106">Essa função também retornará o tamanho de página e o número de páginas em cada um dos bancos de dados especificados.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-106">This function also returns the page size and number of pages in each of the specified databases.</span></span> 
  
```cs
Vitual ERRErrCheckDbHeaders  
(
        ULONG  * const pcbDbPageSize,
        ULONG  * const pcHeaderPagesPerDb,
        ULONG   const piDbErrorEncountered,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="d6a3d-107">Par�metros</span><span class="sxs-lookup"><span data-stu-id="d6a3d-107">Parameters</span></span>

### <a name="pcbdbpagesize"></a><span data-ttu-id="d6a3d-108">pcbDbPageSize</span><span class="sxs-lookup"><span data-stu-id="d6a3d-108">pcbDbPageSize</span></span> 
  
<span data-ttu-id="d6a3d-109">Parâmetro de saída.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-109">Output parameter.</span></span> <span data-ttu-id="d6a3d-110">O tamanho de página de cada banco de dados especificados, em bytes.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-110">The page size of each of the specified databases, in bytes.</span></span>
    
### <a name="pcheaderpagesperdb"></a><span data-ttu-id="d6a3d-111">pcHeaderPagesPerDb</span><span class="sxs-lookup"><span data-stu-id="d6a3d-111">pcHeaderPagesPerDb</span></span> 
  
<span data-ttu-id="d6a3d-112">Parâmetro de saída.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-112">Output parameter.</span></span> <span data-ttu-id="d6a3d-113">O número de páginas no início de cada especificado banco de dados que são reservados pelo mecanismo de banco de dados para uso interno.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-113">The number of pages at the beginning of each specified database that are reserved by the database engine for internal use.</span></span> <span data-ttu-id="d6a3d-114">Observe que você deve *secreta páginas de cabeçalho para a função **ErrCheckDbPages** para validação* .</span><span class="sxs-lookup"><span data-stu-id="d6a3d-114">Note that you should *not* pass header pages to the **ErrCheckDbPages** function for validation.</span></span> 
    
### <a name="pidberrorencountered"></a><span data-ttu-id="d6a3d-115">piDbErrorEncountered</span><span class="sxs-lookup"><span data-stu-id="d6a3d-115">piDbErrorEncountered</span></span>
  
<span data-ttu-id="d6a3d-116">Parâmetro de saída.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-116">Output parameter.</span></span> <span data-ttu-id="d6a3d-117">Se o valor de retorno da função indica um erro, esse parâmetro será um índice na matriz **[] de rgwszDb** passado para a função **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="d6a3d-117">If the return value of the function indicates an error, this parameter will be an index into the **rgwszDb[]** array passed to the **ErrInit** function.</span></span> <span data-ttu-id="d6a3d-118">O elemento de matriz indexada representa o banco de dados no qual o erro foi encontrado.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-118">The indexed array element represents the database in which the error was encountered.</span></span> <span data-ttu-id="d6a3d-119">Se a função não retorna um valor de erro, o valor do parâmetro é inválido.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-119">If the function does not return an error value, this parameter value is invalid.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="d6a3d-120">ulFlags</span><span class="sxs-lookup"><span data-stu-id="d6a3d-120">ulFlags</span></span> 
  
<span data-ttu-id="d6a3d-121">Parâmetro de entrada opcional.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-121">Optional input parameter.</span></span> <span data-ttu-id="d6a3d-122">Esse valor é reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-122">This value is reserved for future use.</span></span> <span data-ttu-id="d6a3d-123">O valor passado deve ser de 0 (zero).</span><span class="sxs-lookup"><span data-stu-id="d6a3d-123">The value passed should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="d6a3d-124">Valor retornado</span><span class="sxs-lookup"><span data-stu-id="d6a3d-124">Return value</span></span>

<span data-ttu-id="d6a3d-125">Essa função retornará um código de erro da [enumeração CChkSGFiles.ERR](cchksgfiles-err-enumeration.md).</span><span class="sxs-lookup"><span data-stu-id="d6a3d-125">This function returns an error code from the [CChkSGFiles.ERR enumeration](cchksgfiles-err-enumeration.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d6a3d-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="d6a3d-126">Remarks</span></span>

<span data-ttu-id="d6a3d-127">**ErrCheckDbHeaders** certifica-se de que todos os bancos de dados registrados com **ErrInit** tenham o mesmo log assinatura e do banco de dados do tamanho da página.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-127">**ErrCheckDbHeaders** verifies that all databases registered with **ErrInit** have the same log signature and database page size.</span></span> <span data-ttu-id="d6a3d-128">Você também pode usar o menor valor de parâmetro de **genMin** e o maior valor do parâmetro **genMax** para determinar o conjunto de arquivos de log que são necessárias para colocar todos os bancos de dados registrados em um estado de desligamento.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-128">You can also use the lowest **genMin** parameter value and the highest **genMax** parameter value to determine the set of log files that are necessary to bring all of the registered databases to a clean-shutdown state.</span></span> 
  
<span data-ttu-id="d6a3d-129">O parâmetro **piDbErrorEncountered** é definido somente quando for detectado um erro, conforme indicado por uma diferente de zero **ErrCheckDbHeaders** o valor de retorno.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-129">The **piDbErrorEncountered** parameter is set only when an error is detected, as indicated by a non-zero **ErrCheckDbHeaders** return value.</span></span> 
  
<span data-ttu-id="d6a3d-130">Quando ocorre um erro nessa função, será adicionado um evento de erro no log de eventos de erro do Windows.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-130">When an error occurs in this function, an error event will be added to the Windows Error event log.</span></span>
  
<span data-ttu-id="d6a3d-131">Você pode chamar **ErrCheckDbHeaders** somente depois de chamar **ErrInit**e você deverá chamá-la antes de chamar **ErrCheckDbPages** e **ErrCheckLogs**.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-131">You can call **ErrCheckDbHeaders** only after calling **ErrInit**, and you must call it before calling **ErrCheckDbPages** and **ErrCheckLogs**.</span></span>
  
<span data-ttu-id="d6a3d-132">Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você deve chamar a função **ErrCheckDbHeaders** na parte com um único segmento e você poderá chamá-lo apenas uma vez para cada objeto **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="d6a3d-132">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrCheckDbHeaders** function in the single-threaded portion, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="d6a3d-133">Requisitos</span><span class="sxs-lookup"><span data-stu-id="d6a3d-133">Requirements</span></span>

<span data-ttu-id="d6a3d-134">Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-134">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="d6a3d-135">A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.</span><span class="sxs-lookup"><span data-stu-id="d6a3d-135">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

