---
title: Validar a integridade do backup, usando a ferramenta Eseutil no Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0d325ba-4482-4ca2-9a69-c890f985b206
description: Descubra como usar a ferramenta de linha de comando Eseutil para validar um backup do repositório do Exchange.
ms.openlocfilehash: 03c4c23d433418911240bbe7c337308a989f3739
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750625"
---
#  <a name="validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013"></a>Validar a integridade do backup, usando a ferramenta Eseutil no Exchange 2013

Descubra como usar a ferramenta de linha de comando Eseutil para validar um backup do repositório do Exchange. 
  
**Aplica-se a:** Exchange Server 2013 
  
Como o serviço de cópia de sombra de Volume (VSS) pode criar backups, enquanto continua do Exchange gravar no banco de dados, o servidor não todas as páginas de toque e executar as verificações de consistência necessárias. Por esse motivo, qualquer aplicativo de backup e restauração que usa VSS deve verificar a consistência do instantâneo. Exchange Server 2013 suporta dois métodos a seguir para verificar a consistência do instantâneo: 
  
- A API CHKSGFILES
    
- A ferramenta de linha de comando Eseutil
    
Recomendamos que você use a API CHKSGFILES porque é mais fácil para o aplicativo de backup detectar, diagnosticar e relatar erros encontrados durante a consistência CHKSGFILES verificar. Para obter informações sobre como usar a API CHKSGFILES, consulte [Validar integridade do backup, usando a API CHKSGFILES no Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md).
  
## <a name="running-the-eseutil-tool"></a>Executando a ferramenta Eseutil

Para verificar a consistência de instantâneo, execute o comando eseutil contra os arquivos de log e de banco de dados que são identificados na tabela a seguir. 
  
**Tabela 1. Comandos de Eseutil.exe para cada tipo de backup**

|**Tipo de backup do tipo de arquivo**|**Backup completo**|**Cópia de backup**|**Backup incremental**|**Backup diferencial**|
|:-----|:-----|:-----|:-----|:-----|
|. edb  <br/> |"eseutil /k /i"  <br/> |"eseutil /k /i"  <br/> |Não aplicável  <br/> |Não aplicável  <br/> |
|. log  <br/> |"eseutil /k" (1)  <br/> |"eseutil /k" (1)  <br/> |"eseutil /k" (2)  <br/> |"eseutil /k" (2)  <br/> |
   
> [!NOTE]
> Você não precisará executar o comando eseutil contra arquivos. stm e. chk. 
  
Todos os arquivos de log que têm a geração de um arquivo de log de número que é igual ou maior do que a geração de número do arquivo de log de ponto de verificação são obrigatórias para recuperar um banco de dados do instantâneo. Se ele existir, o arquivo de log atual (Enn.) também é necessário para recuperação de banco de dados. Se algum dos arquivos de log necessários falhar a verificação de consistência, o solicitante deve se certificar que o status de backup do componente está definido como FALSE, antes de chamar o método [BackupComplete](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382651%28v=vs.85%29.aspx) . Para identificar o arquivo de log de verificação, execute Eseutil.exe contra o arquivo de verificação de instantâneo e analisar a saída para "ponto de verificação:." O exemplo a seguir mostra como executar Eseutil.exe em um arquivo de ponto de verificação. 
  
```cpp
c:\eseutil.exe /mk E01.chk
Checkpoint: (0x20, 9D, 187)
```

A segunda linha do exemplo é o valor de retorno, onde o 0x20 é o número de geração de log hexadecimal do arquivo de log de ponto de verificação. Neste exemplo, quaisquer arquivos de log, incluindo E01000020.log e posterior, deve não estar corrompidos para recuperar o banco de dados do instantâneo, mesmo se o próprio banco de dados já tiver passado para a verificação de consistência física.
  
Todos os arquivos de log em um conjunto de backup incremental ou diferencial são necessários para a recuperação do banco de dados. Você pode verificar a consistência de uma sequência de log executando Eseutil.exe contra o prefixo de arquivo de log. O exemplo a seguir mostra como executar verificações de consistência em relação a todos os arquivos do formulário E01xxxxx.log em um determinado caminho.
  
```cpp
c:\eseutil /k E01
```

## <a name="checking-the-eseutilexe-output"></a>Verificando a saída Eseutil.exe

O solicitante deve verifique se todos os valores de erro ERRORLEVEL de saída que são retornados não negativos. Para obter informações sobre valores ERRORLEVEL, consulte [Reference para erros comuns de Eseutil](http://technet.microsoft.com/en-us/library/aa996759%28v=exchg.80%29.aspx). Para ver o ERRORLEVEL na linha de comando, digite "echo % errorlevel %" após a conclusão da Eseutil.exe. Um negativo ERRORLEVEL indica que um ou mais arquivos está corrompido.
  
Antes do solicitante chama o método **BackupComplete** , ele deve se certificar que o status de backup do componente reflete o resultado da verificação de consistência. Se nenhuma corrupção for encontrada, o status será FALSE; Se nenhuma corrupção for encontrada, o status será TRUE. 
  
## <a name="see-also"></a>Confira também

- [Validar a integridade do backup, usando a API CHKSGFILES no Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
- [Criar um backup e restaurar aplicativos para o Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
- [Referência de classe CChkSGFiles](cchksgfiles-class-reference.md)
- [Conceitos de backup e restauração do Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

