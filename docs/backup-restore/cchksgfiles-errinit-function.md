---
title: Função CChkSGFiles.ErrInit
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrInit
api_type:
- dllExport
ms.assetid: 61bb3af1-8b51-4bae-8e25-90a4dc1226c5
description: 'Modificado pela última vez: 03 de março de 2013'
ms.openlocfilehash: d4b76933a747fe4bf084061cf080bc68264132ed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750628"
---
# <a name="cchksgfileserrinit-function"></a>Função CChkSGFiles.ErrInit
  
**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Inicializa o objeto **CChkSGFiles** especificando os bancos de dados a ser verificado e o caminho e nome de base dos arquivos de log de transação a ser verificado. Aplicativos devem chamar essa função imediatamente após chamar com êxito a função de **New** . 
  
```cs
Vitual ERRErrInit  
(
    Const WCHAR  * const rgwszDb[],
    Const ULONGcDB,
    __in_z const WCHAR  * const wszLogPath,
    __in_z const WCHAR  * const wszBaseName,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Par�metros

### <a name="rgwszdb"></a>[] de rgwszDb
  
Parâmetro de entrada. Uma matriz que especifica os bancos de dados a ser verificado. Cada elemento da matriz é uma cadeia de Unicode terminada em nulo que contém o nome de arquivo e o caminho de um banco de dados a ser verificado.
    
### <a name="cdb"></a>cDB
  
Parâmetro de entrada. O número de elementos na matriz **rgwszDb** do caminho de banco de dados válido. 
    
#### <a name="wszlogpath"></a>wszLogPath
  
Parâmetro de entrada. O caminho completo dos arquivos de log de transações a serem verificados, na forma de uma cadeia de caracteres Unicode terminada em nulo.
    
### <a name="wszbasename"></a>wszBaseName
  
Parâmetro de entrada. O nome de base três letras dos arquivos de log de transação do Exchange, na forma de uma cadeia de caracteres Unicode terminada em nulo.
    
### <a name="ulflags"></a>ulFlags
  
Parâmetro de entrada opcional. Esse valor é reservado para uso futuro. O valor passado por este parâmetro deve ser de 0 (zero).
    
## <a name="return-value"></a>Valor retornado

Um código de erro da enumeração [ERR](cchksgfiles-err-enumeration.md) . 
  
## <a name="remarks"></a>Comentários

A função **ErrInit** registra os bancos de dados e arquivos de log a serem verificados. Esta função deve ser chamada após a função **New** é chamada, mas antes de qualquer outro **ChkSGFiles** é chamada de função. 
  
Você deve fornecer o nome de base, o caminho do arquivo de log e todos os nomes de banco de dados como sequências de caracteres de Unicode terminada em nulo.
  
Você pode verificar somente os arquivos de banco de dados, somente os arquivos de log, ou os arquivos de log e de banco de dados. No entanto, ao chamar essa função, o aplicativo deve especificar pelo menos uma entidade a ser verificado. Passar 0 (zero) para **cDB** e NULL para **wszLogPath** retornará um erro. 
  
Se o valor da **cDB** for diferente de 0 (zero), passar NULL para **rgwszDb** resultará em erro. Para verificar se os arquivos de banco de dados, o aplicativo deve fornecer os nomes de banco de dados. 
  
Se NULL é passado para **wszBaseName** , mas **wszLogPath** não for nula, um erro será retornado. Um nome de arquivo de log base é sempre necessário ao verificar arquivos de log. 
  
Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você deve chamar a função **ErrInit** na parte com um único segmento do aplicativo e você poderá chamá-lo apenas uma vez para cada objeto **CCheckSGFiles** . 
  
## <a name="requirements"></a>Requisitos

Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.
  

