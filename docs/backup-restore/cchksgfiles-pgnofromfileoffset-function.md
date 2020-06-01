---
title: Função função cchksgfiles. PgnoFromFileOffset
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PgnoFromFileOffset
api_type:
- dllExport
ms.assetid: 3d69ca6d-5ed1-4038-859e-106e776eeec1
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: 3c8f749a03b4aa251bf9312eba5d7e2d46c91fae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452892"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a><span data-ttu-id="af571-103">Função função cchksgfiles. PgnoFromFileOffset</span><span class="sxs-lookup"><span data-stu-id="af571-103">CChkSGFiles.PgnoFromFileOffset function</span></span>

<span data-ttu-id="af571-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="af571-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="af571-105">Retorna o número de página do banco de dados lógico que corresponde ao índice de bytes especificado no arquivo de banco de dados físico.</span><span class="sxs-lookup"><span data-stu-id="af571-105">Returns the logical database page number that corresponds to the specified byte index in the physical database file.</span></span> <span data-ttu-id="af571-106">Se o deslocamento do arquivo for inválido, ou se a função **ErrCheckDbHeaders** não tiver sido chamada para os bancos de dados, essa função retornará 0 (zero).</span><span class="sxs-lookup"><span data-stu-id="af571-106">If the file offset is invalid, or if the **ErrCheckDbHeaders** function has not been called for the databases, this function returns 0 (zero).</span></span> 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a><span data-ttu-id="af571-107">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="af571-107">Parameters</span></span>

### <a name="ibfileoffset"></a><span data-ttu-id="af571-108">ibFileOffset</span><span class="sxs-lookup"><span data-stu-id="af571-108">ibFileOffset</span></span>
  
<span data-ttu-id="af571-109">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="af571-109">Input parameter.</span></span> <span data-ttu-id="af571-110">O deslocamento em um arquivo de banco de dados, em bytes.</span><span class="sxs-lookup"><span data-stu-id="af571-110">The offset into a database file, in bytes.</span></span>
    
## <a name="return-value"></a><span data-ttu-id="af571-111">Valor de retorno</span><span class="sxs-lookup"><span data-stu-id="af571-111">Return value</span></span>

<span data-ttu-id="af571-112">O número de página lógica do arquivo de banco de dados que inclui o deslocamento especificado.</span><span class="sxs-lookup"><span data-stu-id="af571-112">The database file's logical page number that includes the specified offset.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="af571-113">Comentários</span><span class="sxs-lookup"><span data-stu-id="af571-113">Remarks</span></span>

<span data-ttu-id="af571-114">Se o parâmetro **ibFileOffset** for inválido, a função **PgnoFromFileOffset** retornará 0 (zero).</span><span class="sxs-lookup"><span data-stu-id="af571-114">If the **ibFileOffset** parameter is invalid, the **PgnoFromFileOffset** function returns 0 (zero).</span></span> 
  
<span data-ttu-id="af571-115">**PgnoFromFileOffset** também retornará 0 (zero) se você não chamou a função **ErrCheckDbHeaders** na instância do **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="af571-115">**PgnoFromFileOffset** also returns 0 (zero) if you haven't called the **ErrCheckDbHeaders** function on the **CCheckSGFiles** instance.</span></span> <span data-ttu-id="af571-116">Você deve chamar **ErrCheckDbHeaders** para inicializar o tamanho da página do banco de dados e o número de páginas alocadas para cabeçalhos do banco de dados.</span><span class="sxs-lookup"><span data-stu-id="af571-116">You must call **ErrCheckDbHeaders** to initialize the database page size and number of pages allocated to database headers.</span></span> 
  
<span data-ttu-id="af571-117">Você deve usar **PgnoFromFileOffset** para preencher os elementos da estrutura de \*\* \_ informações da página\*\* em preparação para chamar **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="af571-117">You should use **PgnoFromFileOffset** to fill in the **PAGE\_INFO** structure elements in preparation for calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="af571-118">O parâmetro **rgPageInfo** para **ErrCheckDbPages** exige que cada elemento na matriz seja uma estrutura **PAGE_INFO** , com os valores de membro **ulPgno** inicializados corretamente.</span><span class="sxs-lookup"><span data-stu-id="af571-118">The **rgPageInfo** parameter to **ErrCheckDbPages** requires that each element in the array be a **PAGE_INFO** structure, with the **ulPgno** member values correctly initialized.</span></span> 
  
<span data-ttu-id="af571-119">Se você estiver usando o CHKSGFILES em um aplicativo multi-threaded, poderá chamar a função **PgnoFromFileOffset** na parte multithread do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="af571-119">If you're using CHKSGFILES in a multithreaded application, you can call the **PgnoFromFileOffset** function in the multithreaded portion of the application.</span></span> <span data-ttu-id="af571-120">Observe que você normalmente chamaria essa função várias vezes para cada banco de dados sendo verificado.</span><span class="sxs-lookup"><span data-stu-id="af571-120">Note that you would typically call this function multiple times for each database being checked.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="af571-121">Requirements</span><span class="sxs-lookup"><span data-stu-id="af571-121">Requirements</span></span>

<span data-ttu-id="af571-122">O Exchange Server 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="af571-122">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="af571-123">A conta sob a qual o aplicativo está sendo executado deve ter permissão de leitura para o banco de dados e arquivos de log que devem ser verificados.</span><span class="sxs-lookup"><span data-stu-id="af571-123">The account that the application is running under must have read permission to the database and log files that are to be checked.</span></span>
  

