---
title: Validar a integridade do backup, usando a API CHKSGFILES no Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 607cbeb9-0a02-4079-8a4d-34bdeb560224
description: Descubra como usar a API de CHKSGFILES para validar um backup do repositório do Exchange no Exchange 2013.
ms.openlocfilehash: 968484cd5bb7439730685643683e1d850bec33ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750633"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a><span data-ttu-id="0dd70-103">Validar a integridade do backup, usando a API CHKSGFILES no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0dd70-103">Validate backup integrity by using the CHKSGFILES API in Exchange 2013</span></span>

<span data-ttu-id="0dd70-104">Descubra como usar a API de CHKSGFILES para validar um backup do repositório do Exchange no Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="0dd70-104">Find out how to use the CHKSGFILES API to validate a backup of the Exchange store in Exchange 2013.</span></span>
  
<span data-ttu-id="0dd70-105">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="0dd70-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="0dd70-106">Durante operações de backup gerenciadas pelo serviço de cópia de sombra de Volume (VSS), o Exchange Server 2013 não é possível ler cada arquivo de banco de dados inteira e verificar sua integridade de soma de verificação.</span><span class="sxs-lookup"><span data-stu-id="0dd70-106">During backup operations managed by the Volume Shadow Copy Service (VSS), Exchange Server 2013 cannot read each database file in its entirety and verify its checksum integrity.</span></span> <span data-ttu-id="0dd70-107">Portanto, talvez você queira que o seu aplicativo de backup para verificar a integridade do arquivo de log do banco de dados e transações.</span><span class="sxs-lookup"><span data-stu-id="0dd70-107">Therefore, you might want your backup application to verify database and transaction log file integrity.</span></span> <span data-ttu-id="0dd70-108">É recomendável que o seu aplicativo de backup verificar a consistência física do conjunto de cópia de sombra antes da informando que o autor do Exchange que o backup for concluído.</span><span class="sxs-lookup"><span data-stu-id="0dd70-108">We recommend that your backup application verify the physical consistency of the shadow copy set prior to informing the Exchange writer that the backup is complete.</span></span> <span data-ttu-id="0dd70-109">Após um backup bem-sucedido, o Exchange store atualiza os cabeçalhos os bancos de dados de backup para refletir o último backup bem-sucedido vezes e remove os logs de transação do servidor não são mais necessários para adiar a partir do último backup bem-sucedido.</span><span class="sxs-lookup"><span data-stu-id="0dd70-109">After a successful backup, the Exchange store updates the headers of the backed-up databases to reflect the last successful backup times and removes transaction logs from the server that are no longer required to roll forward from the last successful backup.</span></span>
  
## <a name="prerequisites-for-validating-backup-integrity"></a><span data-ttu-id="0dd70-110">Pré-requisitos para a validação de integridade do backup.</span><span class="sxs-lookup"><span data-stu-id="0dd70-110">Prerequisites for validating backup integrity</span></span>

<span data-ttu-id="0dd70-111">Antes de seu aplicativo possa validar a integridade do backup, você deve ter acesso ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="0dd70-111">Before your application can validate the integrity of your backup, you must have access to the following:</span></span>
  
- <span data-ttu-id="0dd70-112">Arquivos de seu backup de repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dd70-112">Files from your Exchange store backup.</span></span>
- <span data-ttu-id="0dd70-113">Uma versão do Visual Studio, começando com o Visual Studio 2010.</span><span class="sxs-lookup"><span data-stu-id="0dd70-113">A version of Visual Studio starting with Visual Studio 2010.</span></span>
- <span data-ttu-id="0dd70-114">Os arquivos de cabeçalho e de biblioteca CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="0dd70-114">The CHKSGFILES library and header files.</span></span> <span data-ttu-id="0dd70-115">Você pode baixar os arquivos de biblioteca e o cabeçalho do [Centro de Download da Microsoft](http://www.microsoft.com/en-us/download/details.aspx?id=36802).</span><span class="sxs-lookup"><span data-stu-id="0dd70-115">You can download the library and header files from the [Microsoft Download Center](http://www.microsoft.com/en-us/download/details.aspx?id=36802).</span></span>
    
## <a name="validate-backup-integrity"></a><span data-ttu-id="0dd70-116">Validar a integridade do backup.</span><span class="sxs-lookup"><span data-stu-id="0dd70-116">Validate backup integrity</span></span>

<span data-ttu-id="0dd70-117">O procedimento a seguir descreve como validar a integridade dos dados no seu backup e restaurar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0dd70-117">The following procedure describes how to validate data integrity in your backup and restore application.</span></span>
  
### <a name="to-validate-backup-integrity"></a><span data-ttu-id="0dd70-118">Para validar a integridade do backup.</span><span class="sxs-lookup"><span data-stu-id="0dd70-118">To validate backup integrity</span></span>

1. <span data-ttu-id="0dd70-119">Crie uma nova instância da classe **CChkSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="0dd70-119">Create a new instance of the **CChkSGFiles** class.</span></span> 
   
   ```cpp
   CCheckSGFiles::ERRerr = CCheckSGFiles::errSuccess;
   ULONGiDbError = (ULONG)CCheckSGFiles::iDbInvalid;
   CCheckSGFiles * const pcchecksgfiles = CCheckSGFiles::New();
   if ( NULL == pcchecksgfiles )
   {
     err = CCheckSGFiles::errOutOfMemory;
     printf( "ERROR: Could not allocate CCheckSGFiles object.\n" );
     goto HandleError;
   }
   ```

   <span data-ttu-id="0dd70-120">As primeiras linhas de código cria um objeto error e defina seu valor inicial para o sucesso e criar um objeto que verifica a validade do banco de dados.</span><span class="sxs-lookup"><span data-stu-id="0dd70-120">The first lines of code create an error object and set its initial value to success, and create an object that checks the validity of the database.</span></span> <span data-ttu-id="0dd70-121">Em seguida, a [função CChkSGFiles.New](cchksgfiles-new-function.md) cria uma nova instância da classe **CChkSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="0dd70-121">Then, the [CChkSGFiles.New function](cchksgfiles-new-function.md) creates a new instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="0dd70-122">Uma verificação rápida do novo objeto indica se qualquer problema ocorreu quando a nova instância foi criada.</span><span class="sxs-lookup"><span data-stu-id="0dd70-122">A quick check of the new object indicates whether any issues occurred when the new instance was created.</span></span> 
    
2. <span data-ttu-id="0dd70-123">Inicialize o objeto **CChkSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="0dd70-123">Initialize the **CChkSGFiles** object.</span></span> 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   <span data-ttu-id="0dd70-124">Para obter mais informações sobre os parâmetros, consulte a [função de CChkSGFiles.ErrInit](cchksgfiles-errinit-function.md).</span><span class="sxs-lookup"><span data-stu-id="0dd70-124">For more information about the parameters, see [CChkSGFiles.ErrInit function](cchksgfiles-errinit-function.md).</span></span>
   
3. <span data-ttu-id="0dd70-125">Use a [função CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md) para validar a integridade do banco de dados, verificando os cabeçalhos de banco de dados.</span><span class="sxs-lookup"><span data-stu-id="0dd70-125">Use the [CChkSGFiles.ErrCheckDbHeaders function](cchksgfiles-errcheckdbheaders-function.md) to validate database integrity by checking the database headers.</span></span>
   
   ```cpp
   err = pcchecksgfiles->ErrCheckDbHeaders(
   &amp;cbDbPageSize,
   &amp;cDbHeaderPages,
   &amp;iDbError );
   if ( CCheckSGFiles::errSuccess != err )
   {
   if ( CCheckSGFiles::iDbInvalid != iDbError )
   {
   printf(
   "ERROR: Database header validation for '%S' failed with error %d (0x%x)\n",
   rgwszDb[ iDbError ],
   err,
   err );
   }
   goto HandleError;
   }
   ```
   
   <span data-ttu-id="0dd70-126">Para obter mais informações sobre os parâmetros, consulte a [função de CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md).</span><span class="sxs-lookup"><span data-stu-id="0dd70-126">For more information about the parameters, see [CChkSGFiles.ErrCheckDbHeaders function](cchksgfiles-errcheckdbheaders-function.md).</span></span>
   
4. <span data-ttu-id="0dd70-127">Manipular erros e usar a [função CChkSGFiles.Delete](cchksgfiles-delete-function.md) para remover a classe de **CChkSGFiles** da memória.</span><span class="sxs-lookup"><span data-stu-id="0dd70-127">Handle errors, and use the [CChkSGFiles.Delete function](cchksgfiles-delete-function.md) to remove the **CChkSGFiles** class from memory.</span></span> 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a><span data-ttu-id="0dd70-128">Confira também</span><span class="sxs-lookup"><span data-stu-id="0dd70-128">See also</span></span>

- [<span data-ttu-id="0dd70-129">Referência de classe CChkSGFiles</span><span class="sxs-lookup"><span data-stu-id="0dd70-129">CChkSGFiles class reference</span></span>](cchksgfiles-class-reference.md)
- [<span data-ttu-id="0dd70-130">Criar um backup e restaurar aplicativos para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0dd70-130">Build backup and restore applications for Exchange 2013</span></span>](build-backup-and-restore-applications-for-exchange-2013.md)
- [<span data-ttu-id="0dd70-131">Conceitos de backup e restauração do Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0dd70-131">Backup and restore concepts for Exchange 2013</span></span>](backup-and-restore-concepts-for-exchange-2013.md)
    

