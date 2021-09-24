---
title: Função CChkSGFiles.ErrCheckLogs
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ErrCheckLogs
api_type:
- dllExport
ms.assetid: cec0df4b-4679-4682-bacf-69b4f4aef343
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: 64484b32fdc566d6fee8631f80d078aca82b11d1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516381"
---
# <a name="cchksgfileserrchecklogs-function"></a>Função CChkSGFiles.ErrCheckLogs

**Aplica-se a: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Valida os arquivos de log de todos os arquivos de banco de dados especificados na **função ErrInit.** Os logs validados são aqueles que existem no caminho e que têm o nome do arquivo de log base de três letras passado para **ErrInit**.
  
```cs
Vitual ERRErrCheckLogs 
(
        BOOL  * const pfOnlyUnnecessaryLogsCorrup,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Parâmetros

### <a name="pfonlyunnecessarylogscorrupt"></a>pfOnlyUnnecessaryLogsCorrupt 
  
Parâmetro de saída. Quando **true**, esse parâmetro indica que erros foram encontrados nos arquivos de log de transações, mas todos esses erros foram encontrados em arquivos de log que não são necessários para levar o banco de dados a um estado de desligamento limpo sem perda de dados. Um **valor** verdadeiro retornado neste parâmetro é válido somente quando **ErrCheckLogs** retorna **errSuccess**. 
    
### <a name="ulflags"></a>ulFlags
  
Parâmetro de entrada opcional. Esse valor é reservado para uso futuro. O valor passado por esse parâmetro deve ser 0 (zero).
    
## <a name="return-value"></a>Valor de retorno

Um código de erro da [enumeração ERR.](cchksgfiles-err-enumeration.md) 
  
É importante lembrar que essa função pode retornar **errSuccess** mesmo quando erros são encontrados nos arquivos de log. Portanto, quando **ErrCheckLogs** retorna **errSuccess**, o aplicativo também deve verificar o parâmetro de retorno **pfOnlyUnnecessaryLogsCorrupt.** Se **pfOnlyUnnecessaryLogsCorrupts** for **true** quando **ErrCheckLogs** retornar **errSuccess**, isso indica que um ou mais erros foram encontrados, mas somente em arquivos de log não necessários para tornar o banco de dados atualizado.
  
## <a name="remarks"></a>Comentários

A **função ErrCheckDbHeaders** deve ser chamada antes que a **função ErrCheckLogs** possa ser chamada. 
  
Quando Exchange arquivos de log de transações de banco de dados estão sendo verificados, alguns dos arquivos de log serão necessários para colocar os bancos de dados no grupo de armazenamento em um estado de desligamento limpo sem perda de dados, enquanto outros arquivos de log podem não ser necessários. A **função ErrCheckLogs** determina os arquivos de log mais antigos e os mais novos necessários para manter os bancos de dados atualizados. 
  
A **função ErrCheckLogs** verifica todos os arquivos de log nos caminhos especificados que também têm o nome de arquivo base de três letras especificado, conforme passado para a **função ErrInit.** 
  
Se nenhum erro for encontrado nos arquivos de log, **ErrCheckLogs** **retornará errSuccess**. 
  
Se algum dos arquivos de log necessários for considerado corrompido, **ErrCheckLogs** retornará um erro. 
  
Se erros são encontrados apenas em arquivos de log mais antigos do que os primeiros necessários, a função retornará **errSuccess** e define o parâmetro de retorno **pfOnlyUnnecessaryLogCorrupt** como **true**. O aplicativo deve reconhecer que há erros em alguns desses arquivos de log antigos e, se for o caso, ele possivelmente alertará o usuário. Em qualquer caso, esses erros não devem afetar a integridade geral do banco de dados ou afetar se a reprodução dos logs será bem-sucedida.
  
Se erros são encontrados em qualquer arquivo de log criado após o log mais antigo que **ErrCheckLogs** determina ser necessário, a função retornará um erro. O erro será retornado mesmo que o erro do arquivo de log foi encontrado em um arquivo de log gerado posteriormente ao necessário para manter o banco de dados atualizado. Embora seja possível colocar os bancos de dados em um estado de desligamento limpo usando os arquivos de log identificados, as transações especificadas nos arquivos de log corrompidos posteriormente não serão aplicadas, resultando em perda de dados quando o banco de dados for restaurado. 
  
O **objeto CChkSGFiles** determina se todos os arquivos de log registrados com a **função ErrInit** foram realmente verificados. Se nem todos os logs não foram verificados com êxito, a **função ErrTerm** retornará um erro. 
  
Se você estiver usando CHKSGFILES em um aplicativo multithreaded, poderá chamar a função **ErrCheckLogs** na parte multithreaded do aplicativo, mas você pode chamá-la apenas uma vez para cada **objeto CCheckSGFiles.** 
  
## <a name="requirements"></a>Requisitos

Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta em que o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

