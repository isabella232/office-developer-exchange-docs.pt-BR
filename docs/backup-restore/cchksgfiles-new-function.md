---
title: Função função cchksgfiles. New
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
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: d18d3ef20890012a1d8c193ec87bdca10a1ed451
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455230"
---
# <a name="cchksgfilesnew-function"></a><span data-ttu-id="45954-103">Função função cchksgfiles. New</span><span class="sxs-lookup"><span data-stu-id="45954-103">CChkSGFiles.New function</span></span>

<span data-ttu-id="45954-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="45954-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="45954-105">Cria uma nova instância da classe **função cchksgfiles** .</span><span class="sxs-lookup"><span data-stu-id="45954-105">Creates a new instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="45954-106">Você deve chamar essa função antes de poder especificar o grupo de armazenamento e os bancos de dados a serem verificados.</span><span class="sxs-lookup"><span data-stu-id="45954-106">You must call this function before you can specify the storage group and databases to be checked.</span></span> 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a><span data-ttu-id="45954-107">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="45954-107">Parameters</span></span>

<span data-ttu-id="45954-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="45954-108">None.</span></span>
  
## <a name="return-value"></a><span data-ttu-id="45954-109">Valor retornado</span><span class="sxs-lookup"><span data-stu-id="45954-109">Return value</span></span>

<span data-ttu-id="45954-110">Uma referência (ponteiro) para o objeto recém-criado.</span><span class="sxs-lookup"><span data-stu-id="45954-110">A reference (pointer) to the newly created object.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="45954-111">Comentários</span><span class="sxs-lookup"><span data-stu-id="45954-111">Remarks</span></span>

<span data-ttu-id="45954-112">A **nova** função cria um objeto **CCheckSGFiles** e retorna ao chamador uma referência (ponteiro) para esse objeto.</span><span class="sxs-lookup"><span data-stu-id="45954-112">The **New** function creates a **CCheckSGFiles** object and returns to the caller a reference (pointer) to that object.</span></span> <span data-ttu-id="45954-113">Você deve chamar essa função antes de chamar qualquer uma das outras funções na classe **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="45954-113">You must call this function before it calls any of the other functions in the **CCheckSGFiles** class.</span></span> 
  
<span data-ttu-id="45954-114">Se você estiver usando o CHKSGFILES em um aplicativo multi-threaded, deverá chamar a **nova** função na parte de thread único do aplicativo, e poderá chamá-la somente uma vez para cada objeto **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="45954-114">If you're using CHKSGFILES in a multithreaded application, you must call the **New** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="45954-115">Requirements</span><span class="sxs-lookup"><span data-stu-id="45954-115">Requirements</span></span>

<span data-ttu-id="45954-116">O Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="45954-116">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="45954-117">A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.</span><span class="sxs-lookup"><span data-stu-id="45954-117">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

