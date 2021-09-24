---
title: Validar a integridade do backup usando a API CHKSGFILES no Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 607cbeb9-0a02-4079-8a4d-34bdeb560224
description: Saiba como usar a API CHKSGFILES para validar um backup do Exchange store no Exchange 2013.
ms.openlocfilehash: 7a12a0a8f66128970a782da50ba59f41767c60d3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516227"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a>Validar a integridade do backup usando a API CHKSGFILES no Exchange 2013

Saiba como usar a API CHKSGFILES para validar um backup do Exchange store no Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013 
  
Durante operações de backup gerenciadas pelo Serviço de Cópia de Sombra de Volume (VSS), o Exchange Server 2013 não pode ler cada arquivo de banco de dados em sua totalidade e verificar sua integridade de verificação. Portanto, talvez você queira que seu aplicativo de backup verifique a integridade do arquivo de log de transações e do banco de dados. Recomendamos que seu aplicativo de backup verifique a consistência física do conjunto de cópias de sombra antes de informar ao Exchange que o backup está concluído. Após um backup bem-sucedido, o Exchange atualiza os headers dos bancos de dados de backup para refletir os últimos tempos de backup bem-sucedidos e remove os logs de transação do servidor que não são mais necessários para avançar do último backup bem-sucedido.
  
## <a name="prerequisites-for-validating-backup-integrity"></a>Pré-requisitos para validar a integridade do backup

Para que seu aplicativo possa validar a integridade do backup, você deve ter acesso ao seguinte:
  
- Arquivos do seu Exchange armazenam backup.
- Uma versão do Visual Studio começando com Visual Studio 2010.
- A biblioteca CHKSGFILES e os arquivos de header. Você pode baixar os arquivos de biblioteca e de header do [Centro de Download da Microsoft.](https://www.microsoft.com/download/details.aspx?id=36802)
    
## <a name="validate-backup-integrity"></a>Validar a integridade do backup

O procedimento a seguir descreve como validar a integridade de dados em seu aplicativo de backup e restauração.
  
### <a name="to-validate-backup-integrity"></a>Para validar a integridade do backup

1. Crie uma nova instância da **classe CChkSGFiles.** 
   
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

   As primeiras linhas de código criam um objeto de erro e configuram seu valor inicial como sucesso e criam um objeto que verifica a validade do banco de dados. Em seguida, a [função CChkSGFiles.New](cchksgfiles-new-function.md) cria uma nova instância da **classe CChkSGFiles.** Uma verificação rápida do novo objeto indica se ocorreu algum problema quando a nova instância foi criada. 
    
2. Inicializar o **objeto CChkSGFiles.** 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   Para obter mais informações sobre os parâmetros, consulte [A função CChkSGFiles.ErrInit](cchksgfiles-errinit-function.md).
   
3. Use a [função CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md) para validar a integridade do banco de dados verificando os headers do banco de dados.
   
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
   
   Para obter mais informações sobre os parâmetros, consulte [A função CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md).
   
4. Manipular erros e usar a [função CChkSGFiles.Delete](cchksgfiles-delete-function.md) para remover a **classe CChkSGFiles** da memória. 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a>Confira também

- [Referência da classe CChkSGFiles](cchksgfiles-class-reference.md)
- [Criar aplicativos de backup e restauração para Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
- [Conceitos de backup e restauração para Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

