---
title: Função CChkSGFiles.Delete
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
description: 'Modificado pela última vez: 22 de fevereiro de 2013'
ms.openlocfilehash: 5c41007a797e5a256692b2c4bdcb3cfae82c12ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750630"
---
# <a name="cchksgfilesdelete-function"></a><span data-ttu-id="00efe-103">Função CChkSGFiles.Delete</span><span class="sxs-lookup"><span data-stu-id="00efe-103">CChkSGFiles.Delete function</span></span>

<span data-ttu-id="00efe-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="00efe-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="00efe-105">Destruir uma instância existente da classe **CChkSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="00efe-105">Destroys an existing instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="00efe-106">Você deve chamar essa função depois que o aplicativo tiver terminado de trabalhar com o objeto especificado.</span><span class="sxs-lookup"><span data-stu-id="00efe-106">You must call this function after the application has finished working with the specified object.</span></span> 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a><span data-ttu-id="00efe-107">Par�metros</span><span class="sxs-lookup"><span data-stu-id="00efe-107">Parameters</span></span>

### <a name="pcchecksgfiles"></a><span data-ttu-id="00efe-108">pcchecksgfiles</span><span class="sxs-lookup"><span data-stu-id="00efe-108">pcchecksgfiles</span></span> 
  
<span data-ttu-id="00efe-109">Parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="00efe-109">Input parameter.</span></span> <span data-ttu-id="00efe-110">Um ponteiro para um objeto **CCheckSGFiles** existente.</span><span class="sxs-lookup"><span data-stu-id="00efe-110">A pointer to an existing **CCheckSGFiles** object.</span></span> <span data-ttu-id="00efe-111">A memória associada ao objeto, em seguida, será liberada.</span><span class="sxs-lookup"><span data-stu-id="00efe-111">The memory associated with the object will then be freed.</span></span> 
    
## <a name="return-value"></a><span data-ttu-id="00efe-112">Valor retornado</span><span class="sxs-lookup"><span data-stu-id="00efe-112">Return value</span></span>

<span data-ttu-id="00efe-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="00efe-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="00efe-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="00efe-114">Remarks</span></span>

<span data-ttu-id="00efe-115">A função **Excluir** libera a memória associada ao objeto **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="00efe-115">The **Delete** function frees the memory associated with the **CCheckSGFiles** object.</span></span> <span data-ttu-id="00efe-116">Depois de chamar **Excluir**, o ponteiro transmitido no parâmetro *pcchecksgfiles* será inválido e nenhuma outra operação pode ser executada em desse objeto.</span><span class="sxs-lookup"><span data-stu-id="00efe-116">After you call **Delete**, the pointer passed in the  *pcchecksgfiles*  parameter will be invalid and no other operations can be performed on that object.</span></span> 
  
<span data-ttu-id="00efe-117">Se o aplicativo usa a função **ErrCheckDbPages** , o aplicativo deve liberar o buffer de memória manualmente; a função **Excluir** não serão liberá-la.</span><span class="sxs-lookup"><span data-stu-id="00efe-117">If the application uses the **ErrCheckDbPages** function, the application must free the memory buffer manually; the **Delete** function will not free it.</span></span> 
  
<span data-ttu-id="00efe-118">Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você deve chamar a função **Excluir** na parte com um único segmento do aplicativo e você poderá chamá-lo apenas uma vez para cada objeto **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="00efe-118">If you're using CHKSGFILES in a multithreaded application, you must call the **Delete** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="00efe-119">Requisitos</span><span class="sxs-lookup"><span data-stu-id="00efe-119">Requirements</span></span>

<span data-ttu-id="00efe-120">Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="00efe-120">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="00efe-121">A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.</span><span class="sxs-lookup"><span data-stu-id="00efe-121">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

