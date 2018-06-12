---
title: Função CChkSGFiles.New
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- New
api_type:
- dllExport
ms.assetid: 588d8c74-c9ce-4d5e-8a79-a2a68676e858
description: 'Modificado pela última vez: 22 de fevereiro de 2013'
ms.openlocfilehash: b40f8b1a95477715b29defb4addabfb333e92d04
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750624"
---
# <a name="cchksgfilesnew-function"></a><span data-ttu-id="d5ed4-103">Função CChkSGFiles.New</span><span class="sxs-lookup"><span data-stu-id="d5ed4-103">CChkSGFiles.New function</span></span>

<span data-ttu-id="d5ed4-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="d5ed4-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="d5ed4-105">Cria uma nova instância da classe **CChkSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="d5ed4-105">Creates a new instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="d5ed4-106">Você deve chamar essa função antes de especificar o grupo de armazenamento e bancos de dados a ser verificado.</span><span class="sxs-lookup"><span data-stu-id="d5ed4-106">You must call this function before you can specify the storage group and databases to be checked.</span></span> 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a><span data-ttu-id="d5ed4-107">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="d5ed4-107">Parameters</span></span>

<span data-ttu-id="d5ed4-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d5ed4-108">None.</span></span>
  
## <a name="return-value"></a><span data-ttu-id="d5ed4-109">Valor retornado</span><span class="sxs-lookup"><span data-stu-id="d5ed4-109">Return value</span></span>

<span data-ttu-id="d5ed4-110">Uma referência (ponteiro) para o objeto recém-criado.</span><span class="sxs-lookup"><span data-stu-id="d5ed4-110">A reference (pointer) to the newly created object.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d5ed4-111">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="d5ed4-111">Remarks</span></span>

<span data-ttu-id="d5ed4-112">A função **New** cria um objeto **CCheckSGFiles** e retorna ao chamador uma referência (ponteiro) para esse objeto.</span><span class="sxs-lookup"><span data-stu-id="d5ed4-112">The **New** function creates a **CCheckSGFiles** object and returns to the caller a reference (pointer) to that object.</span></span> <span data-ttu-id="d5ed4-113">Antes de chamar qualquer uma das outras funções na classe **CCheckSGFiles** , você deve chamar essa função.</span><span class="sxs-lookup"><span data-stu-id="d5ed4-113">You must call this function before it calls any of the other functions in the **CCheckSGFiles** class.</span></span> 
  
<span data-ttu-id="d5ed4-114">Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você deve chamar a função **New** na parte com um único segmento do aplicativo e você poderá chamá-lo apenas uma vez para cada objeto **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="d5ed4-114">If you're using CHKSGFILES in a multithreaded application, you must call the **New** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="d5ed4-115">Requisitos</span><span class="sxs-lookup"><span data-stu-id="d5ed4-115">Requirements</span></span>

<span data-ttu-id="d5ed4-116">Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="d5ed4-116">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="d5ed4-117">A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.</span><span class="sxs-lookup"><span data-stu-id="d5ed4-117">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

