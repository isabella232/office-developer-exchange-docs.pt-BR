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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452857"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a>Validar a integridade do backup usando a API CHKSGFILES no Exchange 2013

Descubra como usar a API CHKSGFILES para validar um backup do repositório do Exchange no Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013 
  
Durante operações de backup gerenciadas pelo serviço de cópias de sombra de volume (VSS), o Exchange Server 2013 não pode ler cada arquivo de banco de dados em sua totalidade e verificar a integridade da soma de verificação. Portanto, você pode querer que seu aplicativo de backup Verifique a integridade do banco de dados e do arquivo de log de transações. Recomendamos que o aplicativo de backup Verifique a consistência física do conjunto de cópia de sombra antes de informar o gravador do Exchange de que o backup foi concluído. Após um backup bem-sucedido, o repositório do Exchange atualiza os cabeçalhos dos bancos de dados de backup para refletir os últimos tempos de backup com êxito e remove logs de transações do servidor que não são mais necessários para rolar para frente a partir do último backup bem-sucedido.
  
## <a name="prerequisites-for-validating-backup-integrity"></a>Pré-requisitos para validar a integridade do backup

Para que o aplicativo possa validar a integridade do backup, você deve ter acesso ao seguinte:
  
- Arquivos do backup do armazenamento do Exchange.
- Uma versão do Visual Studio que começa com o Visual Studio 2010.
- A biblioteca CHKSGFILES e os arquivos de cabeçalho. Você pode baixar os arquivos de biblioteca e de cabeçalho no [centro de download da Microsoft](https://www.microsoft.com/download/details.aspx?id=36802).
    
## <a name="validate-backup-integrity"></a>Validar a integridade do backup

O procedimento a seguir descreve como validar a integridade dos dados no aplicativo de backup e restauração.
  
### <a name="to-validate-backup-integrity"></a>Para validar a integridade do backup

1. Crie uma nova instância da classe **função cchksgfiles** . 
   
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

   As primeiras linhas de código criam um objeto Error e definem seu valor inicial como Success e criam um objeto que verifica a validade do banco de dados. Em seguida, a [função função cchksgfiles. New](cchksgfiles-new-function.md) cria uma nova instância da classe **função cchksgfiles** . Uma verificação rápida do novo objeto indica se ocorreram problemas quando a nova instância foi criada. 
    
2. Inicialize o objeto **função cchksgfiles** . 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   Para obter mais informações sobre os parâmetros, consulte a [função função cchksgfiles. ErrInit](cchksgfiles-errinit-function.md).
   
3. Use a [função função cchksgfiles. ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md) para validar a integridade do banco de dados verificando os cabeçalhos do banco de dados.
   
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
   
   Para obter mais informações sobre os parâmetros, consulte a [função função cchksgfiles. ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md).
   
4. Manipule erros e use a [função função cchksgfiles. Delete](cchksgfiles-delete-function.md) para remover a classe **função cchksgfiles** da memória. 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a>Confira também

- [Referência de classe função cchksgfiles](cchksgfiles-class-reference.md)
- [Criar aplicativos de backup e restauração para o Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
- [Conceitos de backup e restauração para o Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

