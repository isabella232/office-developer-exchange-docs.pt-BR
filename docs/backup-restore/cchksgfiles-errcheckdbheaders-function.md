---
title: Função função cchksgfiles. ErrCheckDbHeaders
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
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: a62c5940322d3d7a71f2db93214f1e970fc6859b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455244"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a><span data-ttu-id="6ccd1-103">Função função cchksgfiles. ErrCheckDbHeaders</span><span class="sxs-lookup"><span data-stu-id="6ccd1-103">CChkSGFiles.ErrCheckDbHeaders function</span></span>

<span data-ttu-id="6ccd1-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="6ccd1-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span> 
  
<span data-ttu-id="6ccd1-105">Valida os cabeçalhos dos arquivos de banco de dados que foram especificados pela função **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="6ccd1-105">Validates the headers of the database files that were specified by the **ErrInit** function.</span></span> <span data-ttu-id="6ccd1-106">Essa função também retorna o tamanho da página e o número de páginas em cada um dos bancos de dados especificados.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-106">This function also returns the page size and number of pages in each of the specified databases.</span></span> 
  
```cs
Vitual ERRErrCheckDbHeaders  
(
        ULONG  * const pcbDbPageSize,
        ULONG  * const pcHeaderPagesPerDb,
        ULONG   const piDbErrorEncountered,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="6ccd1-107">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="6ccd1-107">Parameters</span></span>

### <a name="pcbdbpagesize"></a><span data-ttu-id="6ccd1-108">pcbDbPageSize</span><span class="sxs-lookup"><span data-stu-id="6ccd1-108">pcbDbPageSize</span></span> 
  
<span data-ttu-id="6ccd1-109">Parâmetro de saída.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-109">Output parameter.</span></span> <span data-ttu-id="6ccd1-110">O tamanho de página de cada um dos bancos de dados especificados, em bytes.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-110">The page size of each of the specified databases, in bytes.</span></span>
    
### <a name="pcheaderpagesperdb"></a><span data-ttu-id="6ccd1-111">pcHeaderPagesPerDb</span><span class="sxs-lookup"><span data-stu-id="6ccd1-111">pcHeaderPagesPerDb</span></span> 
  
<span data-ttu-id="6ccd1-112">Parâmetro de saída.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-112">Output parameter.</span></span> <span data-ttu-id="6ccd1-113">O número de páginas no início de cada banco de dados especificado que são reservados pelo mecanismo de banco de dados para uso interno.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-113">The number of pages at the beginning of each specified database that are reserved by the database engine for internal use.</span></span> <span data-ttu-id="6ccd1-114">Observe que você *não* deve passar páginas de cabeçalho para a função **ErrCheckDbPages** para validação.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-114">Note that you should *not* pass header pages to the **ErrCheckDbPages** function for validation.</span></span> 
    
### <a name="pidberrorencountered"></a><span data-ttu-id="6ccd1-115">piDbErrorEncountered</span><span class="sxs-lookup"><span data-stu-id="6ccd1-115">piDbErrorEncountered</span></span>
  
<span data-ttu-id="6ccd1-116">Parâmetro de saída.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-116">Output parameter.</span></span> <span data-ttu-id="6ccd1-117">Se o valor de retorno da função indicar um erro, esse parâmetro será um índice na matriz **rgwszDb []** passada para a função **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="6ccd1-117">If the return value of the function indicates an error, this parameter will be an index into the **rgwszDb[]** array passed to the **ErrInit** function.</span></span> <span data-ttu-id="6ccd1-118">O elemento de matriz indexada representa o banco de dados no qual o erro foi encontrado.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-118">The indexed array element represents the database in which the error was encountered.</span></span> <span data-ttu-id="6ccd1-119">Se a função não retornar um valor de erro, esse valor de parâmetro é inválido.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-119">If the function does not return an error value, this parameter value is invalid.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="6ccd1-120">ulFlags</span><span class="sxs-lookup"><span data-stu-id="6ccd1-120">ulFlags</span></span> 
  
<span data-ttu-id="6ccd1-121">Parâmetro de entrada opcional.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-121">Optional input parameter.</span></span> <span data-ttu-id="6ccd1-122">Esse valor é reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-122">This value is reserved for future use.</span></span> <span data-ttu-id="6ccd1-123">O valor passado deve ser 0 (zero).</span><span class="sxs-lookup"><span data-stu-id="6ccd1-123">The value passed should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="6ccd1-124">Valor de retorno</span><span class="sxs-lookup"><span data-stu-id="6ccd1-124">Return value</span></span>

<span data-ttu-id="6ccd1-125">Essa função retorna um código de erro da [Enumeração função cchksgfiles. err](cchksgfiles-err-enumeration.md).</span><span class="sxs-lookup"><span data-stu-id="6ccd1-125">This function returns an error code from the [CChkSGFiles.ERR enumeration](cchksgfiles-err-enumeration.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6ccd1-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="6ccd1-126">Remarks</span></span>

<span data-ttu-id="6ccd1-127">**ErrCheckDbHeaders** verifica se todos os bancos de dados registrados com **ErrInit** têm a mesma assinatura de log e o tamanho da página do banco de dados.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-127">**ErrCheckDbHeaders** verifies that all databases registered with **ErrInit** have the same log signature and database page size.</span></span> <span data-ttu-id="6ccd1-128">Você também pode usar o menor valor de parâmetro **genMin** e o valor de parâmetro de **genMax** mais alto para determinar o conjunto de arquivos de log que são necessários para colocar todos os bancos de dados registrados em um estado de desligamento normal.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-128">You can also use the lowest **genMin** parameter value and the highest **genMax** parameter value to determine the set of log files that are necessary to bring all of the registered databases to a clean-shutdown state.</span></span> 
  
<span data-ttu-id="6ccd1-129">O parâmetro **piDbErrorEncountered** é definido somente quando um erro é detectado, conforme indicado por um valor de retorno diferente de zero **ErrCheckDbHeaders** .</span><span class="sxs-lookup"><span data-stu-id="6ccd1-129">The **piDbErrorEncountered** parameter is set only when an error is detected, as indicated by a non-zero **ErrCheckDbHeaders** return value.</span></span> 
  
<span data-ttu-id="6ccd1-130">Quando ocorrer um erro nesta função, um evento de erro será adicionado ao log de eventos de erro do Windows.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-130">When an error occurs in this function, an error event will be added to the Windows Error event log.</span></span>
  
<span data-ttu-id="6ccd1-131">Você pode chamar **ErrCheckDbHeaders** somente depois de chamar **ErrInit**e deve chamá-lo antes de chamar **ErrCheckDbPages** e **ErrCheckLogs**.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-131">You can call **ErrCheckDbHeaders** only after calling **ErrInit**, and you must call it before calling **ErrCheckDbPages** and **ErrCheckLogs**.</span></span>
  
<span data-ttu-id="6ccd1-132">Se você estiver usando o CHKSGFILES em um aplicativo multi-threaded, deverá chamar a função **ErrCheckDbHeaders** na parte de thread único e você poderá chamá-la apenas uma vez para cada objeto **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="6ccd1-132">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrCheckDbHeaders** function in the single-threaded portion, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="6ccd1-133">Requirements</span><span class="sxs-lookup"><span data-stu-id="6ccd1-133">Requirements</span></span>

<span data-ttu-id="6ccd1-134">O Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-134">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="6ccd1-135">A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.</span><span class="sxs-lookup"><span data-stu-id="6ccd1-135">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

