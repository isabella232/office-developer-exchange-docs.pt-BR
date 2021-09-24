---
title: Validar a integridade do backup usando a ferramenta Eseutil no Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b0d325ba-4482-4ca2-9a69-c890f985b206
description: Saiba como usar a ferramenta de linha de comando Eseutil para validar um backup do Exchange store.
ms.openlocfilehash: 0ac994201d1f6c711e5d4d0a3d5835f9bac6e041
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516220"
---
#  <a name="validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013"></a>Validar a integridade do backup usando a ferramenta Eseutil no Exchange 2013

Saiba como usar a ferramenta de linha de comando Eseutil para validar um backup do Exchange store. 
  
**Aplica-se a:** Exchange Server 2013 
  
Como o Serviço de Cópia de Sombra de Volume (VSS) pode criar backups enquanto o Exchange continua a gravar no banco de dados, o servidor não toca em todas as páginas e executa as verificações de consistência necessárias. Por esse motivo, qualquer aplicativo de backup e restauração que use VSS deve verificar a consistência do instantâneo. Exchange Server 2013 oferece suporte aos dois métodos a seguir para verificar a consistência do instantâneo: 
  
- A API CHKSGFILES
    
- A ferramenta de linha de comando Eseutil
    
Recomendamos que você use a API CHKSGFILES porque é mais fácil para o aplicativo de backup detectar, diagnosticar e relatar erros encontrados durante a verificação de consistência CHKSGFILES. Para obter informações sobre como usar a API CHKSGFILES, consulte Validate backup integrity by using the [CHKSGFILES API in Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md).
  
## <a name="running-the-eseutil-tool"></a>Executando a ferramenta Eseutil

Para verificar a consistência do instantâneo, execute o comando eseutil no banco de dados e nos arquivos de log identificados na tabela a seguir. 
  
**Tabela 1. Eseutil.exe comandos para cada tipo de backup**

|**Tipo de arquivo/tipo de backup**|**Backup completo**|**Copiar backup**|**Backup incremental**|**Backup diferencial**|
|:-----|:-----|:-----|:-----|:-----|
|.edb  <br/> |"eseutil /k /i"  <br/> |"eseutil /k /i"  <br/> |Não aplicável  <br/> |Não aplicável  <br/> |
|.log  <br/> |"eseutil /k" (1)  <br/> |"eseutil /k" (1)  <br/> |"eseutil /k" (2)  <br/> |"eseutil /k" (2)  <br/> |
   
> [!NOTE]
> Você não precisa executar o comando eseutil em arquivos .stm e .chk. 
  
Todos os arquivos de log que têm um número de geração de arquivo de log igual ou maior que o número de geração do arquivo de log de ponto de verificação são necessários para recuperar um banco de dados de instantâneo. Se existir, o arquivo de log atual (Enn.log) também será necessário para a recuperação do banco de dados. Se algum dos arquivos de log necessários falhar na verificação de consistência, o solicitante deverá verificar se o status do componente de backup está definido como FALSE antes de chamar o [método BackupComplete.](https://msdn.microsoft.com/library/windows/desktop/aa382651%28v=vs.85%29.aspx) Para identificar o arquivo de log de ponto de verificação, execute Eseutil.exe o arquivo de ponto de verificação do instantâneo e analisar a saída de "Checkpoint:". O exemplo a seguir mostra como executar Eseutil.exe em um arquivo de ponto de verificação. 
  
```cpp
c:\eseutil.exe /mk E01.chk
Checkpoint: (0x20, 9D, 187)
```

A segunda linha no exemplo é o valor de retorno, onde 0x20 é o número de geração de log hexadecimal do arquivo de log de ponto de verificação. Neste exemplo, todos os arquivos de log, incluindo E010000020.log e mais, não devem estar corrompidos para recuperar o banco de dados de instantâneo, mesmo que o banco de dados em si já tenha passado a verificação de consistência física.
  
Todos os arquivos de log em um conjunto de backup incremental ou diferencial são necessários para recuperação de banco de dados. Você pode verificar a consistência de uma sequência de log executando Eseutil.exe o prefixo de arquivo de log. O exemplo a seguir mostra como executar verificações de consistência em todos os arquivos do formulário E01xxxxx.log em um determinado caminho.
  
```cpp
c:\eseutil /k E01
```

## <a name="checking-the-eseutilexe-output"></a>Verificando a Eseutil.exe saída

O solicitante deve verificar se todos os valores de erro ERRORLEVEL de saída retornados não sãonnegative. Para obter informações sobre valores ERRORLEVEL, consulte [Reference for Common Eseutil Errors](https://technet.microsoft.com/library/aa996759%28v=exchg.80%29.aspx). Para ver ERRORLEVEL na linha de comando, digite "eco %errorlevel%" após Eseutil.exe terminar de executar. Um ERRORLEVEL negativo indica que um ou mais arquivos estão corrompidos.
  
Antes de chamar o método **BackupComplete,** o solicitante deve garantir que o status do componente de backup reflita o resultado da verificação de consistência. Se qualquer corrupção for encontrada, o status será FALSE; se nenhuma corrupção for encontrada, o status será VERDADEIRO. 
  
## <a name="see-also"></a>Confira também

- [Validar a integridade do backup usando a API CHKSGFILES no Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
- [Criar aplicativos de backup e restauração para Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
- [Referência da classe CChkSGFiles](cchksgfiles-class-reference.md)
- [Conceitos de backup e restauração para Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

