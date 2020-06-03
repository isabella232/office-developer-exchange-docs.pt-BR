---
title: Função função cchksgfiles. ErrCheckLogs
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckLogs
api_type:
- dllExport
ms.assetid: cec0df4b-4679-4682-bacf-69b4f4aef343
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: 71e21bb3a748a532f9e3167e0b36898acde71b02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526715"
---
# <a name="cchksgfileserrchecklogs-function"></a>Função função cchksgfiles. ErrCheckLogs

**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Valida os arquivos de log de todos os arquivos de banco de dados que foram especificados na função **ErrInit** . Os logs validados são aqueles que existem no caminho e que têm o nome do arquivo de log base de três letras passado para **ErrInit**.
  
```cs
Vitual ERRErrCheckLogs 
(
        BOOL  * const pfOnlyUnnecessaryLogsCorrup,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Parâmetros

### <a name="pfonlyunnecessarylogscorrupt"></a>pfOnlyUnnecessaryLogsCorrupt 
  
Parâmetro de saída. Quando **true**, este parâmetro indica que foram encontrados erros nos arquivos de log de transações, mas esses erros foram encontrados nos arquivos de log que não são necessários para trazer o banco de dados para um estado de desligamento normal sem perda de dados. Um valor **true** retornado nesse parâmetro é válido somente quando **ErrCheckLogs** retorna **errSuccess**. 
    
### <a name="ulflags"></a>ulFlags
  
Parâmetro de entrada opcional. Esse valor é reservado para uso futuro. O valor passado por esse parâmetro deve ser 0 (zero).
    
## <a name="return-value"></a>Valor de retorno

Um código de erro da enumeração [Err](cchksgfiles-err-enumeration.md) . 
  
É importante lembrar que essa função pode retornar **errSuccess** mesmo quando são encontrados erros nos arquivos de log. Portanto, quando **ErrCheckLogs** retornar **errSuccess**, o aplicativo também deverá verificar o parâmetro de retorno **pfOnlyUnnecessaryLogsCorrupt** . Se **pfOnlyUnnecessaryLogsCorrupts** for **true** quando **ErrCheckLogs** retornar **errSuccess**, isso indica que um ou mais erros foram encontrados, mas apenas em arquivos de log não são necessários para atualizar o banco de dados.
  
## <a name="remarks"></a>Comentários

A função **ErrCheckDbHeaders** deve ser chamada para que a função **ErrCheckLogs** possa ser chamada. 
  
Quando os arquivos de log de transações do banco de dados do Exchange estiverem sendo verificados, alguns dos arquivos de log serão necessários para colocar os bancos de dados no grupo de armazenamento em um estado de desligamento normal sem perda de dados, enquanto outros arquivos de log podem não ser necessários. A função **ErrCheckLogs** determina tanto os arquivos de log mais antigos quanto os mais recentes necessários para atualizar os bancos de dados. 
  
A função **ErrCheckLogs** verifica todos os arquivos de log nos caminhos especificados que também têm o nome de arquivo base de três letras especificado, conforme passado para a função **ErrInit** . 
  
Se nenhum erro for encontrado nos arquivos de log, **ErrCheckLogs** retornará **errSuccess**. 
  
Se qualquer um dos arquivos de log necessários estiver corrompido, **ErrCheckLogs** retornará um erro. 
  
Se forem encontrados erros somente nos arquivos de log que sejam mais antigos do que o mais antigo necessário, a função retornará **errSuccess** e definirá o parâmetro de retorno **pfOnlyUnnecessaryLogCorrupt** como **true**. O aplicativo deve reconhecer que há erros em alguns desses arquivos de log antigos e, em caso afirmativo, ele possivelmente alertará o usuário. Em qualquer caso, esses erros não devem afetar a integridade geral do banco de dados ou afetam se a execução do envio dos logs será bem-sucedida.
  
Se forem encontrados erros em qualquer arquivo de log criado depois que o primeiro log que **ErrCheckLogs** determina for necessário, a função retornará um erro. O erro será retornado mesmo se o erro do arquivo de log foi encontrado em um arquivo de log que foi gerado mais tarde do que o necessário para atualizar o banco de dados. Embora seja possível trazer os bancos de dados para um estado de desligamento normal usando os arquivos de log identificados, as transações especificadas nos arquivos de log corrompidos posteriormente não seriam aplicadas, resultando em perda de dados quando o banco de dados é restaurado. 
  
O objeto **função cchksgfiles** determina se todos os arquivos de log registrados na função **ErrInit** foram realmente verificados. Se nem todos os logs não foram verificados com êxito, a função **ErrTerm** retornará um erro. 
  
Se você estiver usando o CHKSGFILES em um aplicativo multi-threaded, poderá chamar a função **ErrCheckLogs** na parte multithread do aplicativo, mas poderá chamá-la apenas uma vez para cada objeto **CCheckSGFiles** . 
  
## <a name="requirements"></a>Requirements

O Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

