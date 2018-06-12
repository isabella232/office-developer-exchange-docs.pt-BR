---
title: Referência de classe CChkSGFiles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9347d5f6-95bb-4045-9c86-0dc0ded24fe8
description: Encontre informações de referência para a API CHKSGFILES no Exchange 2013.
ms.openlocfilehash: 583ac5e16ab60d119c3028bf81123e9f60a58ff4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750631"
---
# <a name="cchksgfiles-class-reference"></a><span data-ttu-id="642ee-103">Referência de classe CChkSGFiles</span><span class="sxs-lookup"><span data-stu-id="642ee-103">CChkSGFiles class reference</span></span>

<span data-ttu-id="642ee-104">Encontre informações de referência para a API CHKSGFILES no Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="642ee-104">Find reference information for the CHKSGFILES API in Exchange 2013.</span></span>
  
<span data-ttu-id="642ee-105">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="642ee-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="642ee-106">A API CHKSGFILES permite que os aplicativos de backup e restauração verificar a integridade dos arquivos de log de transações do Exchange Server 2013 e bancos de dados programaticamente.</span><span class="sxs-lookup"><span data-stu-id="642ee-106">The CHKSGFILES API enables backup and restore applications to verify the integrity of Exchange Server 2013 transaction log files and databases programmatically.</span></span> <span data-ttu-id="642ee-107">Você pode usar essa API no backup e restaurar aplicativos que usam o serviço de cópia de sombra de Volume (VSS).</span><span class="sxs-lookup"><span data-stu-id="642ee-107">You can use this API in backup and restore applications that use the Volume Shadow Copy Service (VSS).</span></span>
  
> [!NOTE]
> <span data-ttu-id="642ee-108">Grupos de armazenamento não estão disponíveis no Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="642ee-108">Storage groups are not available in Exchange 2013.</span></span> <span data-ttu-id="642ee-109">Suporte para grupos de armazenamento foi removido de versões do Exchange, começando com o Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="642ee-109">Support for storage groups was removed from versions of Exchange starting with Exchange Server 2010.</span></span> <span data-ttu-id="642ee-110">Para manter a compatibilidade com bancos de dados e os grupos de armazenamento nas versões do Exchange anteriores ao Exchange 2010, a API CHKSGFILES permite especificar grupos de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="642ee-110">For backward compatibility with databases and storage groups in versions of Exchange earlier than Exchange 2010, the CHKSGFILES API enables you to specify storage groups.</span></span> <span data-ttu-id="642ee-111">Quando você executa CHKSGFILES em bancos de dados do Exchange 2013, você deve definir parâmetros que especificam um identificador de grupo de armazenamento como uma sequência vazia.</span><span class="sxs-lookup"><span data-stu-id="642ee-111">When you run CHKSGFILES against Exchange 2013 databases, you should set parameters that specify a storage group identifier to an empty string.</span></span> 
  
## <a name="file-location"></a><span data-ttu-id="642ee-112">Local do arquivo</span><span class="sxs-lookup"><span data-stu-id="642ee-112">File location</span></span>
<span data-ttu-id="642ee-113"><a name="bk_fileslocation"> </a></span><span class="sxs-lookup"><span data-stu-id="642ee-113"></span></span>

<span data-ttu-id="642ee-114">A API CHKSGFILES é fornecido como parte do Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="642ee-114">The CHKSGFILES API ships as part of Exchange 2013.</span></span> <span data-ttu-id="642ee-115">Você pode usar essa API em um computador que possui a função de servidor de caixa de correio instalada.</span><span class="sxs-lookup"><span data-stu-id="642ee-115">You can use this API on a computer that has the Mailbox server role installed.</span></span> 
  
<span data-ttu-id="642ee-116">Por padrão, a DLL CHKSGFILES é instalada no diretório C:\Program Files\Microsoft\Exchange\V15\Bin.</span><span class="sxs-lookup"><span data-stu-id="642ee-116">By default, the CHKSGFILES DLL is installed in the C:\Program Files\Microsoft\Exchange\V15\Bin directory.</span></span>
  
<span data-ttu-id="642ee-117">Exchange 2013 inclui somente uma versão de 64 bits (amd64) da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="642ee-117">Exchange 2013 includes only a 64-bit (amd64) version of the CHKSGFILES API.</span></span> 
  
<span data-ttu-id="642ee-118">Você pode baixar um arquivo. zip que inclui a biblioteca CHKSGFILE.lib e arquivos de cabeçalho CHKSGFILES.hxx para uso em seu aplicativo personalizado a partir do [Centro de Download da Microsoft](http://www.microsoft.com/en-us/download/details.aspx?id=36802).</span><span class="sxs-lookup"><span data-stu-id="642ee-118">You can download a .zip file that includes the CHKSGFILE.lib library and CHKSGFILES.hxx header files for use in your custom application from the [Microsoft Download Center](http://www.microsoft.com/en-us/download/details.aspx?id=36802).</span></span>
  
## <a name="development-languages"></a><span data-ttu-id="642ee-119">Idiomas de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="642ee-119">Development languages</span></span>
<span data-ttu-id="642ee-120"><a name="bk_developmentlanguages"> </a></span><span class="sxs-lookup"><span data-stu-id="642ee-120"></span></span>

<span data-ttu-id="642ee-121">A API CHKSGFILES destina-se a uso com versões do Visual Studio, começando com o Visual Studio 2005 em C/C++ nativo.</span><span class="sxs-lookup"><span data-stu-id="642ee-121">The CHKSGFILES API is intended for use with versions of Visual Studio starting with Visual Studio 2005 in native C/C++.</span></span> <span data-ttu-id="642ee-122">A API CHKSGFILES não é destinada para uso em código gerenciado.</span><span class="sxs-lookup"><span data-stu-id="642ee-122">The CHKSGFILES API is not intended for use in managed code.</span></span> <span data-ttu-id="642ee-123">Embora você possa criar um assembly de interoperabilidade COM CHKSGFILES, podemos não são fornecidos um assembly de interoperabilidade COM compatíveis com o Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="642ee-123">Although you can create a COM Interop assembly with CHKSGFILES, we do not ship a supported COM Interop assembly with Exchange 2013.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="642ee-124">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="642ee-124">In this section</span></span>
<span data-ttu-id="642ee-125"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="642ee-125"></span></span>

- [<span data-ttu-id="642ee-126">Função CChkSGFiles.CMaxDbPerSG</span><span class="sxs-lookup"><span data-stu-id="642ee-126">CChkSGFiles.CMaxDbPerSG function</span></span>](cchksgfiles-cmaxdbpersg-function.md)
    
- [<span data-ttu-id="642ee-127">Função CChkSGFiles.Delete</span><span class="sxs-lookup"><span data-stu-id="642ee-127">CChkSGFiles.Delete function</span></span>](cchksgfiles-delete-function.md)
    
- [<span data-ttu-id="642ee-128">Enumeração CChkSGFiles.ERR</span><span class="sxs-lookup"><span data-stu-id="642ee-128">CChkSGFiles.ERR enumeration</span></span>](cchksgfiles-err-enumeration.md)
    
- [<span data-ttu-id="642ee-129">Função CChkSGFiles.ErrCheckDbHeaders</span><span class="sxs-lookup"><span data-stu-id="642ee-129">CChkSGFiles.ErrCheckDbHeaders function</span></span>](cchksgfiles-errcheckdbheaders-function.md)
    
- [<span data-ttu-id="642ee-130">Função CChkSGFiles.ErrCheckDbPages</span><span class="sxs-lookup"><span data-stu-id="642ee-130">CChkSGFiles.ErrCheckDbPages function</span></span>](cchksgfiles-errcheckdbpages-function.md)
    
- [<span data-ttu-id="642ee-131">Função CChkSGFiles.ErrCheckLogs</span><span class="sxs-lookup"><span data-stu-id="642ee-131">CChkSGFiles.ErrCheckLogs function</span></span>](cchksgfiles-errchecklogs-function.md)
    
- [<span data-ttu-id="642ee-132">Função de CChkSGFiles.ErrGetHeader (reservada)</span><span class="sxs-lookup"><span data-stu-id="642ee-132">CChkSGFiles.ErrGetHeader function (reserved)</span></span>](cchksgfiles-errgetheader-function-reserved.md)
    
- [<span data-ttu-id="642ee-133">Função CChkSGFiles.ErrInit</span><span class="sxs-lookup"><span data-stu-id="642ee-133">CChkSGFiles.ErrInit function</span></span>](cchksgfiles-errinit-function.md)
    
- [<span data-ttu-id="642ee-134">Função CChkSGFiles.ErrTerm</span><span class="sxs-lookup"><span data-stu-id="642ee-134">CChkSGFiles.ErrTerm function</span></span>](cchksgfiles-errterm-function.md)
    
- [<span data-ttu-id="642ee-135">Enumeração CChkSGFiles.iDbInvalid</span><span class="sxs-lookup"><span data-stu-id="642ee-135">CChkSGFiles.iDbInvalid enumeration</span></span>](cchksgfiles-idbinvalid-enumeration.md)
    
- [<span data-ttu-id="642ee-136">Função CChkSGFiles.New</span><span class="sxs-lookup"><span data-stu-id="642ee-136">CChkSGFiles.New function</span></span>](cchksgfiles-new-function.md)
    
- [<span data-ttu-id="642ee-137">Enumeração CChkSGFiles.NO_FLAGS</span><span class="sxs-lookup"><span data-stu-id="642ee-137">CChkSGFiles.NO_FLAGS enumeration</span></span>](cchksgfiles-no_flags-enumeration.md)
    
- [<span data-ttu-id="642ee-138">CChkSGFiles.PAGE_INFO struct</span><span class="sxs-lookup"><span data-stu-id="642ee-138">CChkSGFiles.PAGE_INFO struct</span></span>](cchksgfiles-page_info-struct.md)
    
- [<span data-ttu-id="642ee-139">Função CChkSGFiles.PgnoFromFileOffset</span><span class="sxs-lookup"><span data-stu-id="642ee-139">CChkSGFiles.PgnoFromFileOffset function</span></span>](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a><span data-ttu-id="642ee-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="642ee-140">See also</span></span>

- [<span data-ttu-id="642ee-141">Exchange Online e o desenvolvimento do Exchange</span><span class="sxs-lookup"><span data-stu-id="642ee-141">Exchange Online and Exchange development</span></span>](../exchange-server-development.md)
- [<span data-ttu-id="642ee-142">Backup, restauração e recuperação de desastres</span><span class="sxs-lookup"><span data-stu-id="642ee-142">Backup, Restore, and Disaster Recovery</span></span>](http://technet.microsoft.com/en-us/library/dd876874)
    

