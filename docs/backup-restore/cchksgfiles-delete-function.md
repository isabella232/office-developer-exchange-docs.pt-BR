---
title: Função função cchksgfiles. Delete
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- dllExport
ms.assetid: 869e927f-7df2-4247-88ef-b8b05b29a700
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: 38cb72b42727855f652de607bb2a02ecdeaae16e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44447047"
---
# <a name="cchksgfilesdelete-function"></a><span data-ttu-id="68ac8-103">Função função cchksgfiles. Delete</span><span class="sxs-lookup"><span data-stu-id="68ac8-103">CChkSGFiles.Delete function</span></span>

<span data-ttu-id="68ac8-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="68ac8-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="68ac8-105">Destrói uma instância existente da classe **função cchksgfiles** .</span><span class="sxs-lookup"><span data-stu-id="68ac8-105">Destroys an existing instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="68ac8-106">Você deve chamar essa função depois que o aplicativo tiver concluído o trabalho com o objeto especificado.</span><span class="sxs-lookup"><span data-stu-id="68ac8-106">You must call this function after the application has finished working with the specified object.</span></span> 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a><span data-ttu-id="68ac8-107">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="68ac8-107">Parameters</span></span>

### <a name="pcchecksgfiles"></a><span data-ttu-id="68ac8-108">pcchecksgfiles</span><span class="sxs-lookup"><span data-stu-id="68ac8-108">pcchecksgfiles</span></span> 
  
<span data-ttu-id="68ac8-109">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="68ac8-109">Input parameter.</span></span> <span data-ttu-id="68ac8-110">Um ponteiro para um objeto **CCheckSGFiles** existente.</span><span class="sxs-lookup"><span data-stu-id="68ac8-110">A pointer to an existing **CCheckSGFiles** object.</span></span> <span data-ttu-id="68ac8-111">A memória associada ao objeto será liberada.</span><span class="sxs-lookup"><span data-stu-id="68ac8-111">The memory associated with the object will then be freed.</span></span> 
    
## <a name="return-value"></a><span data-ttu-id="68ac8-112">Valor retornado</span><span class="sxs-lookup"><span data-stu-id="68ac8-112">Return value</span></span>

<span data-ttu-id="68ac8-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="68ac8-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="68ac8-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="68ac8-114">Remarks</span></span>

<span data-ttu-id="68ac8-115">A função **delete** libera a memória associada ao objeto **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="68ac8-115">The **Delete** function frees the memory associated with the **CCheckSGFiles** object.</span></span> <span data-ttu-id="68ac8-116">Depois de chamar **delete**, o ponteiro passado no parâmetro *pcchecksgfiles* será inválido e nenhuma outra operação poderá ser executada nesse objeto.</span><span class="sxs-lookup"><span data-stu-id="68ac8-116">After you call **Delete**, the pointer passed in the  *pcchecksgfiles*  parameter will be invalid and no other operations can be performed on that object.</span></span> 
  
<span data-ttu-id="68ac8-117">Se o aplicativo usar a função **ErrCheckDbPages** , o aplicativo deverá liberar o buffer de memória manualmente; a função **excluir** não a liberará.</span><span class="sxs-lookup"><span data-stu-id="68ac8-117">If the application uses the **ErrCheckDbPages** function, the application must free the memory buffer manually; the **Delete** function will not free it.</span></span> 
  
<span data-ttu-id="68ac8-118">Se você estiver usando o CHKSGFILES em um aplicativo multi-threaded, deverá chamar a função **excluir** na parte de thread único do aplicativo e poderá chamá-la somente uma vez para cada objeto **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="68ac8-118">If you're using CHKSGFILES in a multithreaded application, you must call the **Delete** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="68ac8-119">Requirements</span><span class="sxs-lookup"><span data-stu-id="68ac8-119">Requirements</span></span>

<span data-ttu-id="68ac8-120">O Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="68ac8-120">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="68ac8-121">A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.</span><span class="sxs-lookup"><span data-stu-id="68ac8-121">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

