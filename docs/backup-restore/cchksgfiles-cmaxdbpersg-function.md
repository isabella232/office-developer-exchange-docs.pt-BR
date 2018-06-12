---
title: Função CChkSGFiles.CMaxDbPerSG
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CMaxDbPerSG
api_type:
- dllExport
ms.assetid: 5871988b-a5d7-42cc-9b83-8fededb5072f
description: 'Modificado pela última vez: 22 de fevereiro de 2013'
ms.openlocfilehash: bf09074bab6dee13e97e8a59a22ae1b19522a5e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751592"
---
# <a name="cchksgfilescmaxdbpersg-function"></a><span data-ttu-id="4b122-103">Função CChkSGFiles.CMaxDbPerSG</span><span class="sxs-lookup"><span data-stu-id="4b122-103">CChkSGFiles.CMaxDbPerSG function</span></span>

<span data-ttu-id="4b122-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="4b122-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="4b122-105">Retorna o número máximo de bancos de dados permitidos em um único grupo de armazenamento do Exchange server.</span><span class="sxs-lookup"><span data-stu-id="4b122-105">Returns the maximum number of databases allowed in a single Exchange server storage group.</span></span>
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a><span data-ttu-id="4b122-106">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="4b122-106">Parameters</span></span>

<span data-ttu-id="4b122-107">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4b122-107">None.</span></span>
  
## <a name="return-value"></a><span data-ttu-id="4b122-108">Valor retornado</span><span class="sxs-lookup"><span data-stu-id="4b122-108">Return value</span></span>

<span data-ttu-id="4b122-109">O número máximo de bancos de dados que permite que o servidor Exchange especificado por grupo de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="4b122-109">The maximum number of databases that the specified Exchange server allows per storage group.</span></span> <span data-ttu-id="4b122-110">Como os grupos de armazenamento não fazem parte do Exchange 2013, essa função retornará 1.</span><span class="sxs-lookup"><span data-stu-id="4b122-110">Because storage groups are not part of Exchange 2013, this function returns 1.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4b122-111">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="4b122-111">Remarks</span></span>

<span data-ttu-id="4b122-112">Você pode usar o objeto **CCheckSGFiles** para validar os bancos de dados (e os arquivos de log de transação) em apenas um grupo de armazenamento e, portanto, o valor retornado pela função **CMaxDbPerSG** também representa o número máximo de bancos de dados que você pode verificar usando um instância da classe **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="4b122-112">You can use the **CCheckSGFiles** object to validate databases (and transaction log files) in only one storage group, so the value returned by the **CMaxDbPerSG** function also represents the maximum number of databases that you can check by using an instance of the **CCheckSGFiles** class.</span></span> 
  
<span data-ttu-id="4b122-113">Observe que por padrão, o Exchange Server 2003 e Exchange Server 2007 permite que um máximo de cinco bancos de dados por grupo de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="4b122-113">Note that by default, Exchange Server 2003 and Exchange Server 2007 allow a maximum of five databases per storage group.</span></span>
  
## <a name="requirements"></a><span data-ttu-id="4b122-114">Requisitos</span><span class="sxs-lookup"><span data-stu-id="4b122-114">Requirements</span></span>

<span data-ttu-id="4b122-115">Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="4b122-115">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="4b122-116">A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.</span><span class="sxs-lookup"><span data-stu-id="4b122-116">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

