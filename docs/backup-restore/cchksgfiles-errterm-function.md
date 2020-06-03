---
title: Função função cchksgfiles. ErrTerm
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrTerm
api_type:
- dllExport
ms.assetid: eea20a55-4a2a-4209-ae79-dc1ee1cd631b
description: 'Última modificação: 25 de fevereiro de 2013'
ms.openlocfilehash: 12b07fba69054d327c7250bbf83e4c77016e8b3f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466196"
---
# <a name="cchksgfileserrterm-function"></a><span data-ttu-id="ee998-103">Função função cchksgfiles. ErrTerm</span><span class="sxs-lookup"><span data-stu-id="ee998-103">CChkSGFiles.ErrTerm function</span></span>
  
<span data-ttu-id="ee998-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="ee998-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="ee998-105">Fornece um status geral do banco de dados e verificação de log, que indica se todas as páginas de banco de dados e logs foram verificadas com êxito.</span><span class="sxs-lookup"><span data-stu-id="ee998-105">Provides an overall status of the database and log verification, which indicates whether all the database pages and logs were successfully verified.</span></span>
  
> [!IMPORTANT]
> <span data-ttu-id="ee998-106">Os grupos de armazenamento não estão disponíveis no Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="ee998-106">Storage groups are not available in Exchange 2013.</span></span> <span data-ttu-id="ee998-107">Para compatibilidade com versões anteriores com bancos de dados e grupos de armazenamento em versões do Exchange anteriores ao Exchange Server 2010, a API CHKSGFILES permite que você especifique grupos de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="ee998-107">For backward compatibility with databases and storage groups in versions of Exchange earlier than Exchange Server 2010, the CHKSGFILES API enables you to specify storage groups.</span></span> <span data-ttu-id="ee998-108">Ao executar o CHKSGFILES em bancos de dados do Exchange 2013, você deve definir parâmetros que especificam um identificador de grupo de armazenamento para uma cadeia de caracteres vazia.</span><span class="sxs-lookup"><span data-stu-id="ee998-108">When you run CHKSGFILES against Exchange 2013 databases, you should set parameters that specify a storage group identifier to an empty string.</span></span> 
  
```cs
Vitual ERRErrTerm 
(
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="ee998-109">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="ee998-109">Parameters</span></span>

### <a name="ulflags"></a><span data-ttu-id="ee998-110">ulFlags</span><span class="sxs-lookup"><span data-stu-id="ee998-110">ulFlags</span></span>
  
<span data-ttu-id="ee998-111">Parâmetro de entrada opcional.</span><span class="sxs-lookup"><span data-stu-id="ee998-111">Optional input parameter.</span></span> <span data-ttu-id="ee998-112">Esse valor é reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="ee998-112">This value is reserved for future use.</span></span> <span data-ttu-id="ee998-113">O valor passado por esse parâmetro deve ser 0 (zero).</span><span class="sxs-lookup"><span data-stu-id="ee998-113">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="ee998-114">Valor de retorno</span><span class="sxs-lookup"><span data-stu-id="ee998-114">Return value</span></span>

<span data-ttu-id="ee998-115">Um código de erro da enumeração [Err](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="ee998-115">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ee998-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="ee998-116">Remarks</span></span>

<span data-ttu-id="ee998-117">O objeto **função cchksgfiles** determina se todos os bancos de dados registrados com a função **ErrInit** foram realmente verificados.</span><span class="sxs-lookup"><span data-stu-id="ee998-117">The **CChkSGFiles** object determines whether all the databases registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="ee998-118">Este objeto usa a função **ErrCheckDbPages** para verificar se o mesmo número de páginas de banco de dados identificadas pela função **ErrCheckDbHeaders** foram realmente verificados.</span><span class="sxs-lookup"><span data-stu-id="ee998-118">This object uses the **ErrCheckDbPages** function to verify that the same number of database pages identified by the **ErrCheckDbHeaders** function were actually verified.</span></span> <span data-ttu-id="ee998-119">Se o número correto de páginas em cada banco de dados não for verificado com êxito, a função **ErrTerm** retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="ee998-119">If the correct number of pages in each database are not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="ee998-120">Se o número de páginas de banco de dados verificadas com **ErrCheckDbPages** for menor que o indicado por **ErrCheckDbHeaders**, essa função cria um erro no log de eventos do Windows e **ErrTerm** retorna um erro.</span><span class="sxs-lookup"><span data-stu-id="ee998-120">If the number of database pages checked with **ErrCheckDbPages** is less than that indicated by **ErrCheckDbHeaders**, this function creates an error in the Windows Event log, and **ErrTerm** returns an error.</span></span> 
  
<span data-ttu-id="ee998-121">Se o número de páginas de banco de dados verificadas com **ErrCheckDbPages** for maior que o indicado por **ErrCheckDbHeaders**, essa função cria um aviso no log de eventos do Windows para indicar que o aplicativo pode estar desnecessariamente verificando algumas páginas de banco de dados mais de uma vez.</span><span class="sxs-lookup"><span data-stu-id="ee998-121">If the number of database pages checked with **ErrCheckDbPages** is greater than that indicated by **ErrCheckDbHeaders**, this function creates a warning in the Windows Event log to indicate that the application might be unnecessarily checking some database pages more than once.</span></span> <span data-ttu-id="ee998-122">Nesse caso, no entanto, a função **ErrTerm** é bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="ee998-122">In this case, however, the **ErrTerm** function succeeds.</span></span> 
  
<span data-ttu-id="ee998-123">O objeto **função cchksgfiles** também determina se os arquivos de log registrados no **ErrInit** foram realmente verificados.</span><span class="sxs-lookup"><span data-stu-id="ee998-123">The **CChkSGFiles** object also determines whether the log files registered with **ErrInit** were actually checked.</span></span> <span data-ttu-id="ee998-124">Se nem todos os logs foram verificados com êxito, a função **ErrTerm** retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="ee998-124">If not all the logs were successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="ee998-125">Quando **ErrTerm** retornar um erro, ele será o primeiro erro encontrado, mesmo que verifique o status de verificação de todos os bancos de dados registrados no **ErrInit**.</span><span class="sxs-lookup"><span data-stu-id="ee998-125">When **ErrTerm** returns an error, it will be the first error it finds, even though it checks the verification status for all databases registered with **ErrInit**.</span></span>
  
<span data-ttu-id="ee998-126">Se você estiver usando o CHKSGFILES em um aplicativo multi-threaded, deverá chamar a função **ErrTerm** na parte de thread único do aplicativo, e poderá chamá-la não mais do que uma vez para cada objeto **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="ee998-126">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrTerm** function in the single-threaded portion of the application, and you can call it no more than once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="ee998-127">Requirements</span><span class="sxs-lookup"><span data-stu-id="ee998-127">Requirements</span></span>

<span data-ttu-id="ee998-128">O Exchange 2013 inclui apenas uma versão de 64 bits do CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="ee998-128">Exchange 2013 only includes a 64-bit version of CHKSGFILES.</span></span>
  
<span data-ttu-id="ee998-129">A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.</span><span class="sxs-lookup"><span data-stu-id="ee998-129">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

