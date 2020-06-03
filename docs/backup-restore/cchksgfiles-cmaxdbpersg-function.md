---
title: Função função cchksgfiles. CMaxDbPerSG
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
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: b7c3517779eb07ef053c1dd4fa25544310fb3343
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455258"
---
# <a name="cchksgfilescmaxdbpersg-function"></a><span data-ttu-id="0552a-103">Função função cchksgfiles. CMaxDbPerSG</span><span class="sxs-lookup"><span data-stu-id="0552a-103">CChkSGFiles.CMaxDbPerSG function</span></span>

<span data-ttu-id="0552a-104">**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="0552a-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="0552a-105">Retorna o número máximo de bancos de dados permitidos em um único grupo de armazenamento do Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="0552a-105">Returns the maximum number of databases allowed in a single Exchange server storage group.</span></span>
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a><span data-ttu-id="0552a-106">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="0552a-106">Parameters</span></span>

<span data-ttu-id="0552a-107">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0552a-107">None.</span></span>
  
## <a name="return-value"></a><span data-ttu-id="0552a-108">Valor retornado</span><span class="sxs-lookup"><span data-stu-id="0552a-108">Return value</span></span>

<span data-ttu-id="0552a-109">O número máximo de bancos de dados que o servidor do Exchange especificado permite por grupo de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="0552a-109">The maximum number of databases that the specified Exchange server allows per storage group.</span></span> <span data-ttu-id="0552a-110">Como os grupos de armazenamento não fazem parte do Exchange 2013, essa função retorna 1.</span><span class="sxs-lookup"><span data-stu-id="0552a-110">Because storage groups are not part of Exchange 2013, this function returns 1.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0552a-111">Comentários</span><span class="sxs-lookup"><span data-stu-id="0552a-111">Remarks</span></span>

<span data-ttu-id="0552a-112">Você pode usar o objeto **CCheckSGFiles** para validar bancos de dados (e arquivos de log de transações) em apenas um grupo de armazenamento, portanto, o valor retornado pela função **CMaxDbPerSG** também representa o número máximo de bancos de dados que você pode verificar usando uma instância da classe **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="0552a-112">You can use the **CCheckSGFiles** object to validate databases (and transaction log files) in only one storage group, so the value returned by the **CMaxDbPerSG** function also represents the maximum number of databases that you can check by using an instance of the **CCheckSGFiles** class.</span></span> 
  
<span data-ttu-id="0552a-113">Observe que, por padrão, o Exchange Server 2003 e o Exchange Server 2007 permitem um máximo de cinco bancos de dados por grupo de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="0552a-113">Note that by default, Exchange Server 2003 and Exchange Server 2007 allow a maximum of five databases per storage group.</span></span>
  
## <a name="requirements"></a><span data-ttu-id="0552a-114">Requirements</span><span class="sxs-lookup"><span data-stu-id="0552a-114">Requirements</span></span>

<span data-ttu-id="0552a-115">O Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="0552a-115">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="0552a-116">A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.</span><span class="sxs-lookup"><span data-stu-id="0552a-116">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

