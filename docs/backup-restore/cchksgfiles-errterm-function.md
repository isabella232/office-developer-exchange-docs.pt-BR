---
title: Função CChkSGFiles.ErrTerm
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
ms.openlocfilehash: 099ec33663baa2414a0c28b90364523b6191c697
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750634"
---
# <a name="cchksgfileserrterm-function"></a><span data-ttu-id="1f7cb-103">Função CChkSGFiles.ErrTerm</span><span class="sxs-lookup"><span data-stu-id="1f7cb-103">CChkSGFiles.ErrTerm function</span></span>
  
<span data-ttu-id="1f7cb-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="1f7cb-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="1f7cb-105">Fornece um status geral da verificação de banco de dados e log, que indica se todas as páginas de banco de dados e logs foram verificados com êxito.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-105">Provides an overall status of the database and log verification, which indicates whether all the database pages and logs were successfully verified.</span></span>
  
> [!IMPORTANT]
> <span data-ttu-id="1f7cb-106">Grupos de armazenamento não estão disponíveis no Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-106">Storage groups are not available in Exchange 2013.</span></span> <span data-ttu-id="1f7cb-107">Para manter a compatibilidade com bancos de dados e os grupos de armazenamento nas versões do Exchange anteriores ao Exchange Server 2010, a API CHKSGFILES permite especificar grupos de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-107">For backward compatibility with databases and storage groups in versions of Exchange earlier than Exchange Server 2010, the CHKSGFILES API enables you to specify storage groups.</span></span> <span data-ttu-id="1f7cb-108">Quando você executa CHKSGFILES em bancos de dados do Exchange 2013, você deve definir parâmetros que especificam um identificador de grupo de armazenamento como uma sequência vazia.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-108">When you run CHKSGFILES against Exchange 2013 databases, you should set parameters that specify a storage group identifier to an empty string.</span></span> 
  
```cs
Vitual ERRErrTerm 
(
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="1f7cb-109">Par�metros</span><span class="sxs-lookup"><span data-stu-id="1f7cb-109">Parameters</span></span>

### <a name="ulflags"></a><span data-ttu-id="1f7cb-110">ulFlags</span><span class="sxs-lookup"><span data-stu-id="1f7cb-110">ulFlags</span></span>
  
<span data-ttu-id="1f7cb-111">Parâmetro de entrada opcional.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-111">Optional input parameter.</span></span> <span data-ttu-id="1f7cb-112">Esse valor é reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-112">This value is reserved for future use.</span></span> <span data-ttu-id="1f7cb-113">O valor passado por este parâmetro deve ser de 0 (zero).</span><span class="sxs-lookup"><span data-stu-id="1f7cb-113">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="1f7cb-114">Valor retornado</span><span class="sxs-lookup"><span data-stu-id="1f7cb-114">Return value</span></span>

<span data-ttu-id="1f7cb-115">Um código de erro da enumeração [ERR](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="1f7cb-115">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1f7cb-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="1f7cb-116">Remarks</span></span>

<span data-ttu-id="1f7cb-117">O objeto **CChkSGFiles** determina se todos os bancos de dados registrados com a função **ErrInit** realmente marcados.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-117">The **CChkSGFiles** object determines whether all the databases registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="1f7cb-118">Este objeto usa a função **ErrCheckDbPages** para verificar se o mesmo número de páginas identificadas pela função **ErrCheckDbHeaders** realmente foram verificadas de banco de dados.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-118">This object uses the **ErrCheckDbPages** function to verify that the same number of database pages identified by the **ErrCheckDbHeaders** function were actually verified.</span></span> <span data-ttu-id="1f7cb-119">Se o número correto das páginas em cada banco de dados não forem verificado com êxito, a função de **ErrTerm** retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-119">If the correct number of pages in each database are not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="1f7cb-120">Se o número de páginas de banco de dados verificado com **ErrCheckDbPages** for menor do que indicado pelo **ErrCheckDbHeaders**, essa função cria um erro no log de eventos do Windows e **ErrTerm** retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-120">If the number of database pages checked with **ErrCheckDbPages** is less than that indicated by **ErrCheckDbHeaders**, this function creates an error in the Windows Event log, and **ErrTerm** returns an error.</span></span> 
  
<span data-ttu-id="1f7cb-121">Se o número de páginas de banco de dados verificado com **ErrCheckDbPages** for maior do que o indicado pelo **ErrCheckDbHeaders**, essa função cria um aviso no log de eventos do Windows para indicar que o aplicativo pode ser desnecessariamente verificando alguns páginas de banco de dados mais de uma vez.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-121">If the number of database pages checked with **ErrCheckDbPages** is greater than that indicated by **ErrCheckDbHeaders**, this function creates a warning in the Windows Event log to indicate that the application might be unnecessarily checking some database pages more than once.</span></span> <span data-ttu-id="1f7cb-122">Nesse caso, entretanto, a função **ErrTerm** for bem-sucedido.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-122">In this case, however, the **ErrTerm** function succeeds.</span></span> 
  
<span data-ttu-id="1f7cb-123">O objeto **CChkSGFiles** também determina se os arquivos de log registrados com **ErrInit** realmente marcados.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-123">The **CChkSGFiles** object also determines whether the log files registered with **ErrInit** were actually checked.</span></span> <span data-ttu-id="1f7cb-124">Se não todos os logs foram verificadas com êxito, a função **ErrTerm** retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-124">If not all the logs were successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="1f7cb-125">Quando **ErrTerm** retornará um erro, será o primeiro erro encontrar, mesmo que ele verifica o status de verificação para todos os bancos de dados registrados com **ErrInit**.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-125">When **ErrTerm** returns an error, it will be the first error it finds, even though it checks the verification status for all databases registered with **ErrInit**.</span></span>
  
<span data-ttu-id="1f7cb-126">Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você deve chamar a função **ErrTerm** na parte com um único segmento do aplicativo e você poderá chamá-lo sem com mais de uma vez para cada objeto **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="1f7cb-126">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrTerm** function in the single-threaded portion of the application, and you can call it no more than once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="1f7cb-127">Requisitos</span><span class="sxs-lookup"><span data-stu-id="1f7cb-127">Requirements</span></span>

<span data-ttu-id="1f7cb-128">Exchange 2013 inclui apenas uma versão de 64 bits do CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-128">Exchange 2013 only includes a 64-bit version of CHKSGFILES.</span></span>
  
<span data-ttu-id="1f7cb-129">A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.</span><span class="sxs-lookup"><span data-stu-id="1f7cb-129">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

