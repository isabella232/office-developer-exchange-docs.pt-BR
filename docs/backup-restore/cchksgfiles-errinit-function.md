---
title: Função função cchksgfiles. ErrInit
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
description: 'Última modificação: 03 de março de 2013'
ms.openlocfilehash: c881691e7c1ba83a396e659f6aac0328625e49a5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457008"
---
# <a name="cchksgfileserrinit-function"></a>Função função cchksgfiles. ErrInit
  
**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Inicializa o objeto **função cchksgfiles** especificando os bancos de dados a serem verificados e o caminho e o nome base dos arquivos de log de transações a serem verificados. Os aplicativos devem chamar essa função imediatamente após chamarem com êxito a **nova** função. 
  
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

## <a name="parameters"></a>Parâmetros

### <a name="rgwszdb"></a>rgwszDb[]
  
Parâmetro de entrada. Uma matriz que especifica os bancos de dados a serem verificados. Cada elemento da matriz é uma cadeia de caracteres Unicode terminada em nulo que contém o caminho e o nome de arquivo de um banco de dados a ser verificado.
    
### <a name="cdb"></a>cDB
  
Parâmetro de entrada. O número de elementos de caminho de banco de dados válidos na matriz **rgwszDb** . 
    
#### <a name="wszlogpath"></a>wszLogPath
  
Parâmetro de entrada. O caminho completo dos arquivos de log de transações a serem verificados, na forma de uma cadeia de caracteres Unicode terminada em nulo.
    
### <a name="wszbasename"></a>wszBaseName
  
Parâmetro de entrada. O nome base de três letras dos arquivos de log de transações do Exchange, na forma de uma cadeia de caracteres Unicode terminada em nulo.
    
### <a name="ulflags"></a>ulFlags
  
Parâmetro de entrada opcional. Esse valor é reservado para uso futuro. O valor passado por esse parâmetro deve ser 0 (zero).
    
## <a name="return-value"></a>Valor de retorno

Um código de erro da enumeração [Err](cchksgfiles-err-enumeration.md) . 
  
## <a name="remarks"></a>Comentários

A função **ErrInit** registra os bancos de dados e arquivos de log que devem ser verificados. Essa função deve ser chamada depois que a **nova** função é chamada, mas antes de qualquer outra função de **ChkSGFiles** ser chamada. 
  
Você deve fornecer todos os nomes de banco de dados, o caminho do arquivo de log e o nome base como cadeias de caracteres Unicode terminadas por caractere nulo.
  
Você pode verificar somente os arquivos de banco de dados, somente os arquivos de log ou os arquivos de log e de banco de dados. No entanto, ao chamar essa função, o aplicativo deve especificar pelo menos uma entidade a ser verificada. Passar 0 (zero) para **cDB** e NULL para **wszLogPath** retornará um erro. 
  
Se o valor de **cDB** for diferente de 0 (zero), passar NULL para **rgwszDb** resultará em um erro. Para verificar os arquivos do banco de dados, o aplicativo deve fornecer os nomes do banco de dados. 
  
Se NULL for passado para **wszBaseName** mas **WSZLOGPATH** não for nulo, um erro será retornado. Um nome base de arquivo de log sempre é necessário ao verificar arquivos de log. 
  
Se você estiver usando o CHKSGFILES em um aplicativo multi-threaded, deverá chamar a função **ErrInit** na parte de thread único do aplicativo, e poderá chamá-la somente uma vez para cada objeto **CCheckSGFiles** . 
  
## <a name="requirements"></a>Requirements

O Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

