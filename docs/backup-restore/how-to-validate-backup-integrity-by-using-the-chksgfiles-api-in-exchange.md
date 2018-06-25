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
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a>Validar a integridade do backup, usando a API CHKSGFILES no Exchange 2013

Descubra como usar a API de CHKSGFILES para validar um backup do repositório do Exchange no Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013 
  
Durante operações de backup gerenciadas pelo serviço de cópia de sombra de Volume (VSS), o Exchange Server 2013 não é possível ler cada arquivo de banco de dados inteira e verificar sua integridade de soma de verificação. Portanto, talvez você queira que o seu aplicativo de backup para verificar a integridade do arquivo de log do banco de dados e transações. É recomendável que o seu aplicativo de backup verificar a consistência física do conjunto de cópia de sombra antes da informando que o autor do Exchange que o backup for concluído. Após um backup bem-sucedido, o Exchange store atualiza os cabeçalhos os bancos de dados de backup para refletir o último backup bem-sucedido vezes e remove os logs de transação do servidor não são mais necessários para adiar a partir do último backup bem-sucedido.
  
## <a name="prerequisites-for-validating-backup-integrity"></a>Pré-requisitos para a validação de integridade do backup.

Antes de seu aplicativo possa validar a integridade do backup, você deve ter acesso ao seguinte:
  
- Arquivos de seu backup de repositório do Exchange.
- Uma versão do Visual Studio, começando com o Visual Studio 2010.
- Os arquivos de cabeçalho e de biblioteca CHKSGFILES. Você pode baixar os arquivos de biblioteca e o cabeçalho do [Centro de Download da Microsoft](http://www.microsoft.com/en-us/download/details.aspx?id=36802).
    
## <a name="validate-backup-integrity"></a>Validar a integridade do backup.

O procedimento a seguir descreve como validar a integridade dos dados no seu backup e restaurar o aplicativo.
  
### <a name="to-validate-backup-integrity"></a>Para validar a integridade do backup.

1. Crie uma nova instância da classe **CChkSGFiles** . 
   
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

   As primeiras linhas de código cria um objeto error e defina seu valor inicial para o sucesso e criar um objeto que verifica a validade do banco de dados. Em seguida, a [função CChkSGFiles.New](cchksgfiles-new-function.md) cria uma nova instância da classe **CChkSGFiles** . Uma verificação rápida do novo objeto indica se qualquer problema ocorreu quando a nova instância foi criada. 
    
2. Inicialize o objeto **CChkSGFiles** . 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   Para obter mais informações sobre os parâmetros, consulte a [função de CChkSGFiles.ErrInit](cchksgfiles-errinit-function.md).
   
3. Use a [função CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md) para validar a integridade do banco de dados, verificando os cabeçalhos de banco de dados.
   
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
   
   Para obter mais informações sobre os parâmetros, consulte a [função de CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md).
   
4. Manipular erros e usar a [função CChkSGFiles.Delete](cchksgfiles-delete-function.md) para remover a classe de **CChkSGFiles** da memória. 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a>Confira também

- [Referência de classe CChkSGFiles](cchksgfiles-class-reference.md)
- [Criar um backup e restaurar aplicativos para o Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
- [Conceitos de backup e restauração do Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

