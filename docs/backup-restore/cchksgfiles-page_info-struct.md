---
title: CChkSGFiles.PAGE_INFO struct
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
description: 'Modificado pela última vez: 22 de fevereiro de 2013'
ms.openlocfilehash: fa66d253b4fc6bd5c29a39c5323f59bf323a906f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751569"
---
# <a name="cchksgfilespageinfo-struct"></a><span data-ttu-id="c23cf-103">CChkSGFiles.PAGE_INFO struct</span><span class="sxs-lookup"><span data-stu-id="c23cf-103">CChkSGFiles.PAGE_INFO struct</span></span>

<span data-ttu-id="c23cf-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="c23cf-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="c23cf-105">Contém informações para uma página de banco de dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c23cf-105">Holds information for an Exchange database page.</span></span> <span data-ttu-id="c23cf-106">Essa estrutura é usada com a função **ErrCheckDbPages** .</span><span class="sxs-lookup"><span data-stu-id="c23cf-106">This structure is used with the **ErrCheckDbPages** function.</span></span> 
  
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

## <a name="members"></a><span data-ttu-id="c23cf-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c23cf-107">Members</span></span>

### <a name="ulpgno"></a><span data-ttu-id="c23cf-108">ulPgNo</span><span class="sxs-lookup"><span data-stu-id="c23cf-108">ulPgNo</span></span>
  
<span data-ttu-id="c23cf-109">Unsigned Long.</span><span class="sxs-lookup"><span data-stu-id="c23cf-109">Unsigned Long.</span></span> <span data-ttu-id="c23cf-110">Número da página lógica da página banco de dados a ser verificado.</span><span class="sxs-lookup"><span data-stu-id="c23cf-110">Logical page number of the database page to be checked.</span></span> <span data-ttu-id="c23cf-111">Este valor deve ser definido antes de chamar **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="c23cf-111">This value must be set before calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="c23cf-112">Se o aplicativo está lendo o arquivo com base em arquivo deslocamentos e, portanto, deve ser mapeados esses deslocamentos de arquivo aos números de página lógicos, você encontrará o método **PgnoFromFileOffset** útil para determinar o valor para esse campo.</span><span class="sxs-lookup"><span data-stu-id="c23cf-112">If the application is reading the file based on file offsets, and must therefore map those file offsets to logical page numbers, you will find the **PgnoFromFileOffset** method useful to determine the value for this field.</span></span> <span data-ttu-id="c23cf-113">**ErrCheckDbPages** não modifique esse valor.</span><span class="sxs-lookup"><span data-stu-id="c23cf-113">**ErrCheckDbPages** does not modify this value.</span></span> 
    
### <a name="fpageisinitialized"></a><span data-ttu-id="c23cf-114">fPageIsInitialized</span><span class="sxs-lookup"><span data-stu-id="c23cf-114">fPageIsInitialized</span></span> 
  
<span data-ttu-id="c23cf-115">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c23cf-115">Boolean.</span></span> <span data-ttu-id="c23cf-116">Um valor TRUE indica que a página de banco de dados contém dados.</span><span class="sxs-lookup"><span data-stu-id="c23cf-116">A value of TRUE indicates that the database page contains data.</span></span> <span data-ttu-id="c23cf-117">Um valor FALSE indica que a página contém somente zeros.</span><span class="sxs-lookup"><span data-stu-id="c23cf-117">A value of FALSE indicates that the page contains only zeros.</span></span> <span data-ttu-id="c23cf-118">**ErrCheckDbPages** define esse valor.</span><span class="sxs-lookup"><span data-stu-id="c23cf-118">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="fcorrectableerror"></a><span data-ttu-id="c23cf-119">fCorrectableError</span><span class="sxs-lookup"><span data-stu-id="c23cf-119">fCorrectableError</span></span>
  
<span data-ttu-id="c23cf-120">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c23cf-120">Boolean.</span></span> <span data-ttu-id="c23cf-121">Um valor TRUE indica que houve uma incompatibilidade de soma de verificação detectada na página banco de dados, mas que é um erro pode ser corrigido.</span><span class="sxs-lookup"><span data-stu-id="c23cf-121">A value of TRUE indicates that there was a checksum mismatch detected in the database page, but that it is a correctable error.</span></span> <span data-ttu-id="c23cf-122">**ErrCheckDbPages** define esse valor.</span><span class="sxs-lookup"><span data-stu-id="c23cf-122">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="checksumactual"></a><span data-ttu-id="c23cf-123">checksumActual</span><span class="sxs-lookup"><span data-stu-id="c23cf-123">checksumActual</span></span>
  
<span data-ttu-id="c23cf-124">Inteiro não assinado de 64 bits.</span><span class="sxs-lookup"><span data-stu-id="c23cf-124">Unsigned 64-bit integer.</span></span> <span data-ttu-id="c23cf-125">Indica o valor de soma de verificação armazenado no banco de dados para esta página lógica.</span><span class="sxs-lookup"><span data-stu-id="c23cf-125">Indicates the checksum value stored in the database for this logical page.</span></span> <span data-ttu-id="c23cf-126">**ErrCheckDbPages** define esse valor.</span><span class="sxs-lookup"><span data-stu-id="c23cf-126">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="checksumexpected"></a><span data-ttu-id="c23cf-127">checksumExpected</span><span class="sxs-lookup"><span data-stu-id="c23cf-127">checksumExpected</span></span>
  
<span data-ttu-id="c23cf-128">Inteiro não assinado de 64 bits.</span><span class="sxs-lookup"><span data-stu-id="c23cf-128">Unsigned 64-bit integer.</span></span> <span data-ttu-id="c23cf-129">Esse é o valor de soma de verificação esperada é calculado para a página de banco de dados; ele é definido por **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="c23cf-129">This is the expected checksum value that is calculated for the database page; it is set by **ErrCheckDbPages**.</span></span> <span data-ttu-id="c23cf-130">Se esse valor é diferente daquele armazenadas na página banco de dados (ou seja, o valor retornado em **checksumActual**), **ErrCheckDbPages** indicará que um erro foi localizado nesta página de banco de dados.</span><span class="sxs-lookup"><span data-stu-id="c23cf-130">If this value is different from that stored on the database page (that is, the value returned in **checksumActual**), **ErrCheckDbPages** will indicate that an error was found on this database page.</span></span> 
    
### <a name="dbtime"></a><span data-ttu-id="c23cf-131">dbTime</span><span class="sxs-lookup"><span data-stu-id="c23cf-131">dbTime</span></span>
  
<span data-ttu-id="c23cf-132">Inteiro não assinado de 64 bits.</span><span class="sxs-lookup"><span data-stu-id="c23cf-132">Unsigned 64-bit integer.</span></span> <span data-ttu-id="c23cf-133">**ErrCheckDbPages** define este membro para o carimbo de hora na página banco de dados.</span><span class="sxs-lookup"><span data-stu-id="c23cf-133">**ErrCheckDbPages** sets this member to the timestamp on the database page.</span></span> 
    
### <a name="checksumpagestructure"></a><span data-ttu-id="c23cf-134">checksumPageStructure</span><span class="sxs-lookup"><span data-stu-id="c23cf-134">checksumPageStructure</span></span> 
  
<span data-ttu-id="c23cf-135">Inteiro não assinado de 64-bt.</span><span class="sxs-lookup"><span data-stu-id="c23cf-135">Unsigned 64-bt integer.</span></span> <span data-ttu-id="c23cf-136">**ErrCheckDbPages** define este membro para o valor calculado de soma de verificação do conteúdo da página excluindo dados que é desnecessários ao determinar a equivalência lógica de página.</span><span class="sxs-lookup"><span data-stu-id="c23cf-136">**ErrCheckDbPages** sets this member to the calculated checksum value of the contents of the page excluding data which is unnecessary when determining the logical page equivalence.</span></span> <span data-ttu-id="c23cf-137">Por exemplo, é desnecessário considerar os valores de dados no espaço de página do banco de dados não utilizados.</span><span class="sxs-lookup"><span data-stu-id="c23cf-137">For example, it is unnecessary to consider the data values in unused database page space.</span></span> <span data-ttu-id="c23cf-138">Este membro só será válido se os valores de **checksumActual** e **checksumExpected** são iguais uns aos outros.</span><span class="sxs-lookup"><span data-stu-id="c23cf-138">This member is only valid if the **checksumActual**  and  **checksumExpected**  values are equal to each other.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="c23cf-139">ulFlags</span><span class="sxs-lookup"><span data-stu-id="c23cf-139">ulFlags</span></span>
  
<span data-ttu-id="c23cf-140">Inteiro não assinado de 64 bits.</span><span class="sxs-lookup"><span data-stu-id="c23cf-140">Unsigned 64-bit integer.</span></span> <span data-ttu-id="c23cf-141">Reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="c23cf-141">Reserved for future use.</span></span> <span data-ttu-id="c23cf-142">O valor desse campo deve ser definido como 0 (zero) antes de chamar **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="c23cf-142">The value of this field must be set to 0 (zero) before calling **ErrCheckDbPages**.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="c23cf-143">Comentários</span><span class="sxs-lookup"><span data-stu-id="c23cf-143">Remarks</span></span>

<span data-ttu-id="c23cf-144">Ao chamar a função **ErrCheckDbPages** , o parâmetro **rgPageInfo** é uma matriz de **página\_INFO** estruturas.</span><span class="sxs-lookup"><span data-stu-id="c23cf-144">When calling the **ErrCheckDbPages** function, the **rgPageInfo**  parameter is an array of **PAGE\_INFO** structures.</span></span> <span data-ttu-id="c23cf-145">Deve haver um **página\_INFO** estrutura para cada página de banco de dados a ser verificado.</span><span class="sxs-lookup"><span data-stu-id="c23cf-145">There must be one **PAGE\_INFO** structure for each database page to be checked.</span></span> 
  
<span data-ttu-id="c23cf-146">O aplicativo deve definir o membro **ulPgno** com o valor apropriado e também deve definir o membro **ulFlags** como 0 (zero) antes de chamar **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="c23cf-146">The application must set the **ulPgno**  member to the proper value, and must also set the  **ulFlags**  member to 0 (zero) before calling **ErrCheckDbPages**.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="c23cf-147">Requisitos</span><span class="sxs-lookup"><span data-stu-id="c23cf-147">Requirements</span></span>

<span data-ttu-id="c23cf-148">Exchange Server 2013 apenas inclui uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="c23cf-148">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="c23cf-149">A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.</span><span class="sxs-lookup"><span data-stu-id="c23cf-149">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

