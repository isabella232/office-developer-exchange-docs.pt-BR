---
title: Struct função cchksgfiles. PAGE_INFO
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PAGE_INFO
api_type:
- dllExport
ms.assetid: 408335e1-6977-441f-bfad-ede791d1630c
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: 5ec9f4303b26ea95b125adac6943945ae1276439
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456336"
---
# <a name="cchksgfilespage_info-struct"></a><span data-ttu-id="58797-103">Struct função cchksgfiles. PAGE_INFO</span><span class="sxs-lookup"><span data-stu-id="58797-103">CChkSGFiles.PAGE_INFO struct</span></span>

<span data-ttu-id="58797-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="58797-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="58797-105">Armazena informações de uma página de banco de dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="58797-105">Holds information for an Exchange database page.</span></span> <span data-ttu-id="58797-106">Essa estrutura é usada com a função **ErrCheckDbPages** .</span><span class="sxs-lookup"><span data-stu-id="58797-106">This structure is used with the **ErrCheckDbPages** function.</span></span> 
  
```cs
Struct PAGE_INFO  
{
        ULONGulPgno;
        BOOLfPageIsInitialized : 1;
        BOOLfCorrectableError : 1;
        ULONGLONGchecksumActual;
        ULONGLONGchecksumExpected;
        ULONGLONGdbTime;
        ULONGLONGchecksumPageStructure;
        ULONGLONGulFlags;
}

```

## <a name="members"></a><span data-ttu-id="58797-107">Members</span><span class="sxs-lookup"><span data-stu-id="58797-107">Members</span></span>

### <a name="ulpgno"></a><span data-ttu-id="58797-108">ulPgNo</span><span class="sxs-lookup"><span data-stu-id="58797-108">ulPgNo</span></span>
  
<span data-ttu-id="58797-109">Longo não assinado.</span><span class="sxs-lookup"><span data-stu-id="58797-109">Unsigned Long.</span></span> <span data-ttu-id="58797-110">Número de página lógica da página do banco de dados a ser verificado.</span><span class="sxs-lookup"><span data-stu-id="58797-110">Logical page number of the database page to be checked.</span></span> <span data-ttu-id="58797-111">Esse valor deve ser definido antes de chamar **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="58797-111">This value must be set before calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="58797-112">Se o aplicativo estiver lendo o arquivo com base nos deslocamentos de arquivo e, portanto, mapear esses deslocamentos de arquivo para números de página lógicos, você encontrará o método **PgnoFromFileOffset** útil para determinar o valor desse campo.</span><span class="sxs-lookup"><span data-stu-id="58797-112">If the application is reading the file based on file offsets, and must therefore map those file offsets to logical page numbers, you will find the **PgnoFromFileOffset** method useful to determine the value for this field.</span></span> <span data-ttu-id="58797-113">**ErrCheckDbPages** não modifica esse valor.</span><span class="sxs-lookup"><span data-stu-id="58797-113">**ErrCheckDbPages** does not modify this value.</span></span> 
    
### <a name="fpageisinitialized"></a><span data-ttu-id="58797-114">fPageIsInitialized</span><span class="sxs-lookup"><span data-stu-id="58797-114">fPageIsInitialized</span></span> 
  
<span data-ttu-id="58797-115">Valor.</span><span class="sxs-lookup"><span data-stu-id="58797-115">Boolean.</span></span> <span data-ttu-id="58797-116">Um valor TRUE indica que a página do banco de dados contém dados.</span><span class="sxs-lookup"><span data-stu-id="58797-116">A value of TRUE indicates that the database page contains data.</span></span> <span data-ttu-id="58797-117">Um valor FALSE indica que a página contém apenas zeros.</span><span class="sxs-lookup"><span data-stu-id="58797-117">A value of FALSE indicates that the page contains only zeros.</span></span> <span data-ttu-id="58797-118">**ErrCheckDbPages** define este valor.</span><span class="sxs-lookup"><span data-stu-id="58797-118">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="fcorrectableerror"></a><span data-ttu-id="58797-119">fCorrectableError</span><span class="sxs-lookup"><span data-stu-id="58797-119">fCorrectableError</span></span>
  
<span data-ttu-id="58797-120">Valor.</span><span class="sxs-lookup"><span data-stu-id="58797-120">Boolean.</span></span> <span data-ttu-id="58797-121">Um valor TRUE indica que houve uma incompatibilidade de checksum detectada na página do banco de dados, mas é um erro corrigível.</span><span class="sxs-lookup"><span data-stu-id="58797-121">A value of TRUE indicates that there was a checksum mismatch detected in the database page, but that it is a correctable error.</span></span> <span data-ttu-id="58797-122">**ErrCheckDbPages** define este valor.</span><span class="sxs-lookup"><span data-stu-id="58797-122">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="checksumactual"></a><span data-ttu-id="58797-123">checksumActual</span><span class="sxs-lookup"><span data-stu-id="58797-123">checksumActual</span></span>
  
<span data-ttu-id="58797-124">Inteiro de 64 bits não assinado.</span><span class="sxs-lookup"><span data-stu-id="58797-124">Unsigned 64-bit integer.</span></span> <span data-ttu-id="58797-125">Indica o valor de checksum armazenado no banco de dados para essa página lógica.</span><span class="sxs-lookup"><span data-stu-id="58797-125">Indicates the checksum value stored in the database for this logical page.</span></span> <span data-ttu-id="58797-126">**ErrCheckDbPages** define este valor.</span><span class="sxs-lookup"><span data-stu-id="58797-126">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="checksumexpected"></a><span data-ttu-id="58797-127">checksumExpected</span><span class="sxs-lookup"><span data-stu-id="58797-127">checksumExpected</span></span>
  
<span data-ttu-id="58797-128">Inteiro de 64 bits não assinado.</span><span class="sxs-lookup"><span data-stu-id="58797-128">Unsigned 64-bit integer.</span></span> <span data-ttu-id="58797-129">Este é o valor de soma de verificação esperado que é calculado para a página do banco de dados; é definido pelo **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="58797-129">This is the expected checksum value that is calculated for the database page; it is set by **ErrCheckDbPages**.</span></span> <span data-ttu-id="58797-130">Se esse valor for diferente daquele armazenado na página de banco de dados (ou seja, o valor retornado em **checksumActual**), **ErrCheckDbPages** indicará que um erro foi encontrado nesta página de banco de dados.</span><span class="sxs-lookup"><span data-stu-id="58797-130">If this value is different from that stored on the database page (that is, the value returned in **checksumActual**), **ErrCheckDbPages** will indicate that an error was found on this database page.</span></span> 
    
### <a name="dbtime"></a><span data-ttu-id="58797-131">dbTime</span><span class="sxs-lookup"><span data-stu-id="58797-131">dbTime</span></span>
  
<span data-ttu-id="58797-132">Inteiro de 64 bits não assinado.</span><span class="sxs-lookup"><span data-stu-id="58797-132">Unsigned 64-bit integer.</span></span> <span data-ttu-id="58797-133">**ErrCheckDbPages** define este membro para o carimbo de data/hora na página do banco de dados.</span><span class="sxs-lookup"><span data-stu-id="58797-133">**ErrCheckDbPages** sets this member to the timestamp on the database page.</span></span> 
    
### <a name="checksumpagestructure"></a><span data-ttu-id="58797-134">checksumPageStructure</span><span class="sxs-lookup"><span data-stu-id="58797-134">checksumPageStructure</span></span> 
  
<span data-ttu-id="58797-135">Inteiro de 64-BT não assinado.</span><span class="sxs-lookup"><span data-stu-id="58797-135">Unsigned 64-bt integer.</span></span> <span data-ttu-id="58797-136">**ErrCheckDbPages** define este membro como o valor de soma de verificação calculado do conteúdo da página, excluindo dados desnecessários ao determinar a equivalência de página lógica.</span><span class="sxs-lookup"><span data-stu-id="58797-136">**ErrCheckDbPages** sets this member to the calculated checksum value of the contents of the page excluding data which is unnecessary when determining the logical page equivalence.</span></span> <span data-ttu-id="58797-137">Por exemplo, não é necessário considerar os valores de dados no espaço de página de banco de dados não usado.</span><span class="sxs-lookup"><span data-stu-id="58797-137">For example, it is unnecessary to consider the data values in unused database page space.</span></span> <span data-ttu-id="58797-138">Este membro só será válido se os valores **checksumActual** e **checksumExpected** forem iguais.</span><span class="sxs-lookup"><span data-stu-id="58797-138">This member is only valid if the **checksumActual**  and  **checksumExpected**  values are equal to each other.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="58797-139">ulFlags</span><span class="sxs-lookup"><span data-stu-id="58797-139">ulFlags</span></span>
  
<span data-ttu-id="58797-140">Inteiro de 64 bits não assinado.</span><span class="sxs-lookup"><span data-stu-id="58797-140">Unsigned 64-bit integer.</span></span> <span data-ttu-id="58797-141">Reserved for future use.</span><span class="sxs-lookup"><span data-stu-id="58797-141">Reserved for future use.</span></span> <span data-ttu-id="58797-142">O valor deste campo deve ser definido como 0 (zero) antes de chamar **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="58797-142">The value of this field must be set to 0 (zero) before calling **ErrCheckDbPages**.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="58797-143">Comentários</span><span class="sxs-lookup"><span data-stu-id="58797-143">Remarks</span></span>

<span data-ttu-id="58797-144">Ao chamar a função **ErrCheckDbPages** , o parâmetro **rgPageInfo** é uma matriz de estruturas de \*\* \_ informações da página\*\* .</span><span class="sxs-lookup"><span data-stu-id="58797-144">When calling the **ErrCheckDbPages** function, the **rgPageInfo**  parameter is an array of **PAGE\_INFO** structures.</span></span> <span data-ttu-id="58797-145">Deve haver uma estrutura **de \_ informações da página** para cada página de banco de dados a ser verificada.</span><span class="sxs-lookup"><span data-stu-id="58797-145">There must be one **PAGE\_INFO** structure for each database page to be checked.</span></span> 
  
<span data-ttu-id="58797-146">O aplicativo deve definir o membro **ulPgno** para o valor apropriado e também deve definir o membro **parâmetroulflags** como 0 (zero) antes de chamar **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="58797-146">The application must set the **ulPgno**  member to the proper value, and must also set the  **ulFlags**  member to 0 (zero) before calling **ErrCheckDbPages**.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="58797-147">Requirements</span><span class="sxs-lookup"><span data-stu-id="58797-147">Requirements</span></span>

<span data-ttu-id="58797-148">O Exchange Server 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="58797-148">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="58797-149">A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.</span><span class="sxs-lookup"><span data-stu-id="58797-149">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

