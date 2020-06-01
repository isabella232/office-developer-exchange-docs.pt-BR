---
title: Validar a integridade do backup usando a ferramenta Eseutil no Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0d325ba-4482-4ca2-9a69-c890f985b206
description: Descubra como usar a ferramenta de linha de comando Eseutil para validar um backup do repositório do Exchange.
ms.openlocfilehash: e8f1a46e2d94729ae5586861317312e277216d63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452794"
---
#  <a name="validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013"></a>Validar a integridade do backup usando a ferramenta Eseutil no Exchange 2013

Descubra como usar a ferramenta de linha de comando Eseutil para validar um backup do repositório do Exchange. 
  
**Aplica-se a:** Exchange Server 2013 
  
Como o serviço de cópias de sombra de volume (VSS) pode criar backups enquanto o Exchange continua a gravar no banco de dados, o servidor não toca em todas as páginas e realiza as verificações de consistência necessárias. Por esse motivo, qualquer aplicativo de backup e restauração que usa o VSS deve verificar a consistência do instantâneo. O Exchange Server 2013 suporta os dois métodos a seguir para verificar a consistência do instantâneo: 
  
- A API CHKSGFILES
    
- A ferramenta de linha de comando Eseutil
    
Recomendamos que você use a API CHKSGFILES, pois é mais fácil para o aplicativo de backup detectar, diagnosticar e relatar erros encontrados durante a verificação de consistência do CHKSGFILES. Para saber mais sobre como usar a API do CHKSGFILES, confira [validar integridade do backup usando a API do CHKSGFILES no Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md).
  
## <a name="running-the-eseutil-tool"></a>Executando a ferramenta Eseutil

Para verificar a consistência do instantâneo, execute o comando Eseutil em relação aos arquivos de log e banco de dados identificados na tabela a seguir. 
  
**Tabela 1. Comandos Eseutil. exe para cada tipo de backup**

|**Tipo de arquivo/tipo de backup**|**Backup completo**|**Copiar backup**|**Backup incremental**|**Backup diferencial**|
|:-----|:-----|:-----|:-----|:-----|
|. edb  <br/> |"Eseutil/k/i"  <br/> |"Eseutil/k/i"  <br/> |Não aplicável  <br/> |Não aplicável  <br/> |
|. log  <br/> |"Eseutil/k" (1)  <br/> |"Eseutil/k" (1)  <br/> |"Eseutil/k" (2)  <br/> |"Eseutil/k" (2)  <br/> |
   
> [!NOTE]
> Não é necessário executar o comando Eseutil em arquivos. stm e. chk. 
  
Todos os arquivos de log que têm um número de geração de arquivo de log igual ou maior que o número de geração do arquivo de log de ponto de verificação são necessários para recuperar um banco de dados de instantâneo. Se ele existir, o arquivo de log atual (Enn. log) também será necessário para a recuperação de banco de dados. Se algum dos arquivos de log necessários falhar na verificação de consistência, o solicitante deverá garantir que o status do componente de backup seja definido como FALSE antes de chamar o método [BackupComplete](https://msdn.microsoft.com/library/windows/desktop/aa382651%28v=vs.85%29.aspx) . Para identificar o arquivo de log de ponto de verificação, execute o Eseutil. exe em relação ao arquivo de verificação de instantâneo e analise a saída de "ponto de verificação:". O exemplo a seguir mostra como executar o Eseutil. exe em um arquivo de ponto de verificação. 
  
```cpp
c:\eseutil.exe /mk E01.chk
Checkpoint: (0x20, 9D, 187)
```

A segunda linha no exemplo é o valor de retorno, onde 0x20 é o número de geração de log hexadecimal do arquivo de log de ponto de verificação. Neste exemplo, qualquer arquivo de log, incluindo E01000020. log e superior, não deve estar corrompido para recuperar o banco de dados de instantâneo, mesmo que o banco de dados em si já tenha passado a verificação de consistência física.
  
Todos os arquivos de log em um conjunto de backup incremental ou diferencial são necessários para a recuperação do banco de dados. Você pode verificar a consistência de uma sequência de log executando o Eseutil. exe em relação ao prefixo do arquivo de log. O exemplo a seguir mostra como executar verificações de consistência em todos os arquivos do formato E01xxxxx. log em um determinado caminho.
  
```cpp
c:\eseutil /k E01
```

## <a name="checking-the-eseutilexe-output"></a>Verificação da saída de Eseutil. exe

O solicitante deve verificar se todos os valores de erro de Exit ERRORLEVEL retornados não são negativos. Para obter informações sobre valores ERRORLEVEL, confira [referência para erros comuns de Eseutil](https://technet.microsoft.com/library/aa996759%28v=exchg.80%29.aspx). Para ver o ERRORLEVEL na linha de comando, digite "Echo% ERRORLEVEL%" após o Eseutil. exe terminar a execução. Um ERRORLEVEL negativo indica que um ou mais arquivos estão corrompidos.
  
Antes de o solicitante chamar o método **BackupComplete** , ele deve garantir que o status do componente de backup reflita o resultado da verificação de consistência. Se alguma corrupção for encontrada, o status será FALSE; Se nenhuma corrupção for encontrada, o status será TRUE. 
  
## <a name="see-also"></a>Também consulte

- [Validar a integridade do backup usando a API CHKSGFILES no Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
- [Criar aplicativos de backup e restauração para o Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
- [Referência de classe função cchksgfiles](cchksgfiles-class-reference.md)
- [Conceitos de backup e restauração para o Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

