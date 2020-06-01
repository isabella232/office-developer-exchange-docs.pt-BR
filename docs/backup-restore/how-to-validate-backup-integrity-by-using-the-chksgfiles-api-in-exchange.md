---
title: Validar a integridade do backup usando a API CHKSGFILES no Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 607cbeb9-0a02-4079-8a4d-34bdeb560224
description: Descubra como usar a API CHKSGFILES para validar um backup do repositório do Exchange no Exchange 2013.
ms.openlocfilehash: c101413793cf3b952d3db3e0f792c8bcf2dd9fc9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452857"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a><span data-ttu-id="4ece4-103">Validar a integridade do backup usando a API CHKSGFILES no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="4ece4-103">Validate backup integrity by using the CHKSGFILES API in Exchange 2013</span></span>

<span data-ttu-id="4ece4-104">Descubra como usar a API CHKSGFILES para validar um backup do repositório do Exchange no Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="4ece4-104">Find out how to use the CHKSGFILES API to validate a backup of the Exchange store in Exchange 2013.</span></span>
  
<span data-ttu-id="4ece4-105">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="4ece4-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="4ece4-106">Durante operações de backup gerenciadas pelo serviço de cópias de sombra de volume (VSS), o Exchange Server 2013 não pode ler cada arquivo de banco de dados em sua totalidade e verificar a integridade da soma de verificação.</span><span class="sxs-lookup"><span data-stu-id="4ece4-106">During backup operations managed by the Volume Shadow Copy Service (VSS), Exchange Server 2013 cannot read each database file in its entirety and verify its checksum integrity.</span></span> <span data-ttu-id="4ece4-107">Portanto, você pode querer que seu aplicativo de backup Verifique a integridade do banco de dados e do arquivo de log de transações.</span><span class="sxs-lookup"><span data-stu-id="4ece4-107">Therefore, you might want your backup application to verify database and transaction log file integrity.</span></span> <span data-ttu-id="4ece4-108">Recomendamos que o aplicativo de backup Verifique a consistência física do conjunto de cópia de sombra antes de informar o gravador do Exchange de que o backup foi concluído.</span><span class="sxs-lookup"><span data-stu-id="4ece4-108">We recommend that your backup application verify the physical consistency of the shadow copy set prior to informing the Exchange writer that the backup is complete.</span></span> <span data-ttu-id="4ece4-109">Após um backup bem-sucedido, o repositório do Exchange atualiza os cabeçalhos dos bancos de dados de backup para refletir os últimos tempos de backup com êxito e remove logs de transações do servidor que não são mais necessários para rolar para frente a partir do último backup bem-sucedido.</span><span class="sxs-lookup"><span data-stu-id="4ece4-109">After a successful backup, the Exchange store updates the headers of the backed-up databases to reflect the last successful backup times and removes transaction logs from the server that are no longer required to roll forward from the last successful backup.</span></span>
  
## <a name="prerequisites-for-validating-backup-integrity"></a><span data-ttu-id="4ece4-110">Pré-requisitos para validar a integridade do backup</span><span class="sxs-lookup"><span data-stu-id="4ece4-110">Prerequisites for validating backup integrity</span></span>

<span data-ttu-id="4ece4-111">Para que o aplicativo possa validar a integridade do backup, você deve ter acesso ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="4ece4-111">Before your application can validate the integrity of your backup, you must have access to the following:</span></span>
  
- <span data-ttu-id="4ece4-112">Arquivos do backup do armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ece4-112">Files from your Exchange store backup.</span></span>
- <span data-ttu-id="4ece4-113">Uma versão do Visual Studio que começa com o Visual Studio 2010.</span><span class="sxs-lookup"><span data-stu-id="4ece4-113">A version of Visual Studio starting with Visual Studio 2010.</span></span>
- <span data-ttu-id="4ece4-114">A biblioteca CHKSGFILES e os arquivos de cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="4ece4-114">The CHKSGFILES library and header files.</span></span> <span data-ttu-id="4ece4-115">Você pode baixar os arquivos de biblioteca e de cabeçalho no [centro de download da Microsoft](https://www.microsoft.com/download/details.aspx?id=36802).</span><span class="sxs-lookup"><span data-stu-id="4ece4-115">You can download the library and header files from the [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=36802).</span></span>
    
## <a name="validate-backup-integrity"></a><span data-ttu-id="4ece4-116">Validar a integridade do backup</span><span class="sxs-lookup"><span data-stu-id="4ece4-116">Validate backup integrity</span></span>

<span data-ttu-id="4ece4-117">O procedimento a seguir descreve como validar a integridade dos dados no aplicativo de backup e restauração.</span><span class="sxs-lookup"><span data-stu-id="4ece4-117">The following procedure describes how to validate data integrity in your backup and restore application.</span></span>
  
### <a name="to-validate-backup-integrity"></a><span data-ttu-id="4ece4-118">Para validar a integridade do backup</span><span class="sxs-lookup"><span data-stu-id="4ece4-118">To validate backup integrity</span></span>

1. <span data-ttu-id="4ece4-119">Crie uma nova instância da classe **função cchksgfiles** .</span><span class="sxs-lookup"><span data-stu-id="4ece4-119">Create a new instance of the **CChkSGFiles** class.</span></span> 
   
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

   <span data-ttu-id="4ece4-120">As primeiras linhas de código criam um objeto Error e definem seu valor inicial como Success e criam um objeto que verifica a validade do banco de dados.</span><span class="sxs-lookup"><span data-stu-id="4ece4-120">The first lines of code create an error object and set its initial value to success, and create an object that checks the validity of the database.</span></span> <span data-ttu-id="4ece4-121">Em seguida, a [função função cchksgfiles. New](cchksgfiles-new-function.md) cria uma nova instância da classe **função cchksgfiles** .</span><span class="sxs-lookup"><span data-stu-id="4ece4-121">Then, the [CChkSGFiles.New function](cchksgfiles-new-function.md) creates a new instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="4ece4-122">Uma verificação rápida do novo objeto indica se ocorreram problemas quando a nova instância foi criada.</span><span class="sxs-lookup"><span data-stu-id="4ece4-122">A quick check of the new object indicates whether any issues occurred when the new instance was created.</span></span> 
    
2. <span data-ttu-id="4ece4-123">Inicialize o objeto **função cchksgfiles** .</span><span class="sxs-lookup"><span data-stu-id="4ece4-123">Initialize the **CChkSGFiles** object.</span></span> 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   <span data-ttu-id="4ece4-124">Para obter mais informações sobre os parâmetros, consulte a [função função cchksgfiles. ErrInit](cchksgfiles-errinit-function.md).</span><span class="sxs-lookup"><span data-stu-id="4ece4-124">For more information about the parameters, see [CChkSGFiles.ErrInit function](cchksgfiles-errinit-function.md).</span></span>
   
3. <span data-ttu-id="4ece4-125">Use a [função função cchksgfiles. ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md) para validar a integridade do banco de dados verificando os cabeçalhos do banco de dados.</span><span class="sxs-lookup"><span data-stu-id="4ece4-125">Use the [CChkSGFiles.ErrCheckDbHeaders function](cchksgfiles-errcheckdbheaders-function.md) to validate database integrity by checking the database headers.</span></span>
   
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
   
   <span data-ttu-id="4ece4-126">Para obter mais informações sobre os parâmetros, consulte a [função função cchksgfiles. ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md).</span><span class="sxs-lookup"><span data-stu-id="4ece4-126">For more information about the parameters, see [CChkSGFiles.ErrCheckDbHeaders function](cchksgfiles-errcheckdbheaders-function.md).</span></span>
   
4. <span data-ttu-id="4ece4-127">Manipule erros e use a [função função cchksgfiles. Delete](cchksgfiles-delete-function.md) para remover a classe **função cchksgfiles** da memória.</span><span class="sxs-lookup"><span data-stu-id="4ece4-127">Handle errors, and use the [CChkSGFiles.Delete function](cchksgfiles-delete-function.md) to remove the **CChkSGFiles** class from memory.</span></span> 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a><span data-ttu-id="4ece4-128">Também consulte</span><span class="sxs-lookup"><span data-stu-id="4ece4-128">See also</span></span>

- [<span data-ttu-id="4ece4-129">Referência de classe função cchksgfiles</span><span class="sxs-lookup"><span data-stu-id="4ece4-129">CChkSGFiles class reference</span></span>](cchksgfiles-class-reference.md)
- [<span data-ttu-id="4ece4-130">Criar aplicativos de backup e restauração para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="4ece4-130">Build backup and restore applications for Exchange 2013</span></span>](build-backup-and-restore-applications-for-exchange-2013.md)
- [<span data-ttu-id="4ece4-131">Conceitos de backup e restauração para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="4ece4-131">Backup and restore concepts for Exchange 2013</span></span>](backup-and-restore-concepts-for-exchange-2013.md)
    

