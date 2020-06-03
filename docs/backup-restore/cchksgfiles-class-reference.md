---
title: Referência de classe função cchksgfiles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9347d5f6-95bb-4045-9c86-0dc0ded24fe8
description: Encontre informações de referência para a API do CHKSGFILES no Exchange 2013.
ms.openlocfilehash: 38b1f2c900767c22594636f0c6ddf4855961aec4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526729"
---
# <a name="cchksgfiles-class-reference"></a><span data-ttu-id="b977a-103">Referência de classe função cchksgfiles</span><span class="sxs-lookup"><span data-stu-id="b977a-103">CChkSGFiles class reference</span></span>

<span data-ttu-id="b977a-104">Encontre informações de referência para a API do CHKSGFILES no Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="b977a-104">Find reference information for the CHKSGFILES API in Exchange 2013.</span></span>
  
<span data-ttu-id="b977a-105">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="b977a-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="b977a-106">A API CHKSGFILES permite que aplicativos de backup e restauração verifiquem a integridade dos arquivos de log de transações e bancos de dados do Exchange Server 2013 programaticamente.</span><span class="sxs-lookup"><span data-stu-id="b977a-106">The CHKSGFILES API enables backup and restore applications to verify the integrity of Exchange Server 2013 transaction log files and databases programmatically.</span></span> <span data-ttu-id="b977a-107">Você pode usar essa API em aplicativos de backup e restauração que usam o serviço de cópias de sombra de volume (VSS).</span><span class="sxs-lookup"><span data-stu-id="b977a-107">You can use this API in backup and restore applications that use the Volume Shadow Copy Service (VSS).</span></span>
  
> [!NOTE]
> <span data-ttu-id="b977a-108">Os grupos de armazenamento não estão disponíveis no Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="b977a-108">Storage groups are not available in Exchange 2013.</span></span> <span data-ttu-id="b977a-109">O suporte para grupos de armazenamento foi removido de versões do Exchange a partir do Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="b977a-109">Support for storage groups was removed from versions of Exchange starting with Exchange Server 2010.</span></span> <span data-ttu-id="b977a-110">Para compatibilidade com versões anteriores com bancos de dados e grupos de armazenamento em versões do Exchange anteriores ao Exchange 2010, a API CHKSGFILES permite que você especifique grupos de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="b977a-110">For backward compatibility with databases and storage groups in versions of Exchange earlier than Exchange 2010, the CHKSGFILES API enables you to specify storage groups.</span></span> <span data-ttu-id="b977a-111">Ao executar o CHKSGFILES em bancos de dados do Exchange 2013, você deve definir parâmetros que especificam um identificador de grupo de armazenamento para uma cadeia de caracteres vazia.</span><span class="sxs-lookup"><span data-stu-id="b977a-111">When you run CHKSGFILES against Exchange 2013 databases, you should set parameters that specify a storage group identifier to an empty string.</span></span> 
  
## <a name="file-location"></a><span data-ttu-id="b977a-112">Local do arquivo</span><span class="sxs-lookup"><span data-stu-id="b977a-112">File location</span></span>
<span data-ttu-id="b977a-113"><a name="bk_fileslocation"> </a></span><span class="sxs-lookup"><span data-stu-id="b977a-113"><a name="bk_fileslocation"> </a></span></span>

<span data-ttu-id="b977a-114">A API do CHKSGFILES é fornecida como parte do Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="b977a-114">The CHKSGFILES API ships as part of Exchange 2013.</span></span> <span data-ttu-id="b977a-115">Você pode usar essa API em um computador que tenha a função de servidor caixa de Correio instalada.</span><span class="sxs-lookup"><span data-stu-id="b977a-115">You can use this API on a computer that has the Mailbox server role installed.</span></span> 
  
<span data-ttu-id="b977a-116">Por padrão, a DLL CHKSGFILES é instalada no diretório C:\Arquivos de Files\Microsoft\Exchange\V15\Bin.</span><span class="sxs-lookup"><span data-stu-id="b977a-116">By default, the CHKSGFILES DLL is installed in the C:\Program Files\Microsoft\Exchange\V15\Bin directory.</span></span>
  
<span data-ttu-id="b977a-117">O Exchange 2013 inclui apenas uma versão de 64 bits (amd64) da API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="b977a-117">Exchange 2013 includes only a 64-bit (amd64) version of the CHKSGFILES API.</span></span> 
  
<span data-ttu-id="b977a-118">Você pode baixar um arquivo. zip que inclui a biblioteca CHKSGFILE. lib e os arquivos de cabeçalho CHKSGFILES. hXX para uso no seu aplicativo personalizado no [centro de download da Microsoft](https://www.microsoft.com/download/details.aspx?id=36802).</span><span class="sxs-lookup"><span data-stu-id="b977a-118">You can download a .zip file that includes the CHKSGFILE.lib library and CHKSGFILES.hxx header files for use in your custom application from the [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=36802).</span></span>
  
## <a name="development-languages"></a><span data-ttu-id="b977a-119">Linguagens de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="b977a-119">Development languages</span></span>
<span data-ttu-id="b977a-120"><a name="bk_developmentlanguages"> </a></span><span class="sxs-lookup"><span data-stu-id="b977a-120"><a name="bk_developmentlanguages"> </a></span></span>

<span data-ttu-id="b977a-121">A API CHKSGFILES deve ser usada com versões do Visual Studio que começam com o Visual Studio 2005 no C/C++ nativo.</span><span class="sxs-lookup"><span data-stu-id="b977a-121">The CHKSGFILES API is intended for use with versions of Visual Studio starting with Visual Studio 2005 in native C/C++.</span></span> <span data-ttu-id="b977a-122">A API CHKSGFILES não se destina ao uso em código gerenciado.</span><span class="sxs-lookup"><span data-stu-id="b977a-122">The CHKSGFILES API is not intended for use in managed code.</span></span> <span data-ttu-id="b977a-123">Embora você possa criar um assembly de interoperabilidade com com o CHKSGFILES, não enviamos um assembly de interoperabilidade COM com o Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="b977a-123">Although you can create a COM Interop assembly with CHKSGFILES, we do not ship a supported COM Interop assembly with Exchange 2013.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="b977a-124">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="b977a-124">In this section</span></span>
<span data-ttu-id="b977a-125"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="b977a-125"><a name="bk_inthissection"> </a></span></span>

- [<span data-ttu-id="b977a-126">Função função cchksgfiles. CMaxDbPerSG</span><span class="sxs-lookup"><span data-stu-id="b977a-126">CChkSGFiles.CMaxDbPerSG function</span></span>](cchksgfiles-cmaxdbpersg-function.md)
    
- [<span data-ttu-id="b977a-127">Função função cchksgfiles. Delete</span><span class="sxs-lookup"><span data-stu-id="b977a-127">CChkSGFiles.Delete function</span></span>](cchksgfiles-delete-function.md)
    
- [<span data-ttu-id="b977a-128">Enumeração função cchksgfiles. ERR</span><span class="sxs-lookup"><span data-stu-id="b977a-128">CChkSGFiles.ERR enumeration</span></span>](cchksgfiles-err-enumeration.md)
    
- [<span data-ttu-id="b977a-129">Função função cchksgfiles. ErrCheckDbHeaders</span><span class="sxs-lookup"><span data-stu-id="b977a-129">CChkSGFiles.ErrCheckDbHeaders function</span></span>](cchksgfiles-errcheckdbheaders-function.md)
    
- [<span data-ttu-id="b977a-130">Função função cchksgfiles. ErrCheckDbPages</span><span class="sxs-lookup"><span data-stu-id="b977a-130">CChkSGFiles.ErrCheckDbPages function</span></span>](cchksgfiles-errcheckdbpages-function.md)
    
- [<span data-ttu-id="b977a-131">Função função cchksgfiles. ErrCheckLogs</span><span class="sxs-lookup"><span data-stu-id="b977a-131">CChkSGFiles.ErrCheckLogs function</span></span>](cchksgfiles-errchecklogs-function.md)
    
- [<span data-ttu-id="b977a-132">Função função cchksgfiles. ErrGetHeader (reservado)</span><span class="sxs-lookup"><span data-stu-id="b977a-132">CChkSGFiles.ErrGetHeader function (reserved)</span></span>](cchksgfiles-errgetheader-function-reserved.md)
    
- [<span data-ttu-id="b977a-133">Função função cchksgfiles. ErrInit</span><span class="sxs-lookup"><span data-stu-id="b977a-133">CChkSGFiles.ErrInit function</span></span>](cchksgfiles-errinit-function.md)
    
- [<span data-ttu-id="b977a-134">Função função cchksgfiles. ErrTerm</span><span class="sxs-lookup"><span data-stu-id="b977a-134">CChkSGFiles.ErrTerm function</span></span>](cchksgfiles-errterm-function.md)
    
- [<span data-ttu-id="b977a-135">Enumeração função cchksgfiles. iDbInvalid</span><span class="sxs-lookup"><span data-stu-id="b977a-135">CChkSGFiles.iDbInvalid enumeration</span></span>](cchksgfiles-idbinvalid-enumeration.md)
    
- [<span data-ttu-id="b977a-136">Função função cchksgfiles. New</span><span class="sxs-lookup"><span data-stu-id="b977a-136">CChkSGFiles.New function</span></span>](cchksgfiles-new-function.md)
    
- [<span data-ttu-id="b977a-137">Enumeração função cchksgfiles. NO_FLAGS</span><span class="sxs-lookup"><span data-stu-id="b977a-137">CChkSGFiles.NO_FLAGS enumeration</span></span>](cchksgfiles-no_flags-enumeration.md)
    
- [<span data-ttu-id="b977a-138">Struct função cchksgfiles. PAGE_INFO</span><span class="sxs-lookup"><span data-stu-id="b977a-138">CChkSGFiles.PAGE_INFO struct</span></span>](cchksgfiles-page_info-struct.md)
    
- [<span data-ttu-id="b977a-139">Função função cchksgfiles. PgnoFromFileOffset</span><span class="sxs-lookup"><span data-stu-id="b977a-139">CChkSGFiles.PgnoFromFileOffset function</span></span>](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a><span data-ttu-id="b977a-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="b977a-140">See also</span></span>

- [<span data-ttu-id="b977a-141">Desenvolvimento do Exchange Online e do Exchange</span><span class="sxs-lookup"><span data-stu-id="b977a-141">Exchange Online and Exchange development</span></span>](../exchange-server-development.md)
- [<span data-ttu-id="b977a-142">Backup, restauração e recuperação de desastre</span><span class="sxs-lookup"><span data-stu-id="b977a-142">Backup, Restore, and Disaster Recovery</span></span>](https://technet.microsoft.com/library/dd876874)
    

