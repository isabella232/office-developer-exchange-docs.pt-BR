---
title: Função CChkSGFiles.ErrCheckLogs
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
description: 'Modificado pela última vez: 22 de fevereiro de 2013'
ms.openlocfilehash: 5b1070de73bc23ae09ddb7835bd72c8e8a71a95f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750632"
---
# <a name="cchksgfileserrchecklogs-function"></a>Função CChkSGFiles.ErrCheckLogs

**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Valida os arquivos de log de todos os arquivos de banco de dados que foram especificados na função **ErrInit** . Os logs validados são aqueles que existir no caminho e que possuírem o nome do arquivo de log de base de três letras passado para **ErrInit**.
  
```cs
Vitual ERRErrCheckLogs 
(
        BOOL  * const pfOnlyUnnecessaryLogsCorrup,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Par�metros

### <a name="pfonlyunnecessarylogscorrupt"></a>pfOnlyUnnecessaryLogsCorrupt 
  
Parâmetro de saída. Quando **true**, esse parâmetro indica que foram encontrados erros em arquivos de log de transações, mas esses erros foram todas encontradas nos arquivos de log que não são necessários para colocar o banco de dados para um estado de desligamento sem perda de dados. Um valor **true** retornado neste parâmetro é válido somente quando **ErrCheckLogs** retorna **errSuccess**. 
    
### <a name="ulflags"></a>ulFlags
  
Parâmetro de entrada opcional. Esse valor é reservado para uso futuro. O valor passado por este parâmetro deve ser de 0 (zero).
    
## <a name="return-value"></a>Valor retornado

Um código de erro da enumeração [ERR](cchksgfiles-err-enumeration.md) . 
  
É importante lembrar-se de que esta função pode retornar **errSuccess** , mesmo quando são encontrados erros nos arquivos de log. Portanto, quando **ErrCheckLogs** retorna **errSuccess**, o aplicativo deve também verificar o parâmetro de retorno de **pfOnlyUnnecessaryLogsCorrupt** . Se **pfOnlyUnnecessaryLogsCorrupts** for **true** quando **ErrCheckLogs** retorna **errSuccess**, isto indica que foram encontrados erros de um ou mais, mas apenas nos arquivos de log que não é necessários colocar o banco de dados atualizado.
  
## <a name="remarks"></a>Coment�rios

A função **ErrCheckDbHeaders** deve ser chamada antes que a função **ErrCheckLogs** pode ser chamada. 
  
Quando os arquivos de log de transações de banco de dados do Exchange estão sendo verificados, alguns dos arquivos de log será necessário colocar os bancos de dados no grupo de armazenamento em um estado de desligamento sem perda de dados, enquanto outros arquivos de log não podem ser necessários. A função **ErrCheckLogs** determina antigos e os arquivos de log mais recentes que são necessárias para tornar os bancos de dados atualizados. 
  
A função **ErrCheckLogs** verifica todos os arquivos de log nos caminhos especificados que também tenham o nome de arquivo especificado de base de três letras, como passados para a função **ErrInit** . 
  
Se nenhum erro for encontrado nos arquivos de log, **ErrCheckLogs** retorna **errSuccess**. 
  
Se qualquer um dos arquivos de log exigidos forem encontradas corrompido, **ErrCheckLogs** retornará um erro. 
  
Se houver erros apenas nos arquivos de log mais antigas que a primeira aqueles necessários, a função retorna **errSuccess** e define o parâmetro de retorno **pfOnlyUnnecessaryLogCorrupt** como **true**. O aplicativo deve reconhecer que há erros em alguns desses arquivos de log antigo e, em caso afirmativo, ele irá alertá possivelmente o usuário. Em qualquer caso, esses erros não devem afetar a integridade geral do banco de dados ou afetam se reproduzir os logs de encaminhar terá êxito.
  
Se houver erros em qualquer arquivo de log criado após a primeira log **ErrCheckLogs** determina é necessária, a função retornará um erro. O erro será retornado até mesmo se o erro de arquivo de log foi encontrado em um arquivo de log gerado mais recente do que o que é precisava colocar o banco de dados atualizado. Embora seria possível trazer os bancos de dados para um estado de desligamento usando os arquivos de log identificados, especificadas nos arquivos de posteriormente corrompidos log de transações não seriam aplicadas, resultando em perda de dados quando o banco de dados for restaurado. 
  
O objeto **CChkSGFiles** determina se todos os arquivos de log registrados com a função **ErrInit** realmente marcados. Se não todos os logs não foram verificada com êxito, a função **ErrTerm** retornará um erro. 
  
Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você pode chamar a função **ErrCheckLogs** na parte multithread do aplicativo, mas você poderá chamá-lo apenas uma vez para cada objeto **CCheckSGFiles** . 
  
## <a name="requirements"></a>Requisitos

Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.
  

