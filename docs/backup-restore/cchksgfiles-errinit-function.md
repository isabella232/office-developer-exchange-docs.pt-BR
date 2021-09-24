---
title: Função CChkSGFiles.ErrInit
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ErrInit
api_type:
- dllExport
ms.assetid: 61bb3af1-8b51-4bae-8e25-90a4dc1226c5
description: 'Última modificação: 03 de março de 2013'
ms.openlocfilehash: ccb5293e35f20328181c4cf1cb5f0eddbb42e03f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516290"
---
# <a name="cchksgfileserrinit-function"></a>Função CChkSGFiles.ErrInit
  
**Aplica-se a: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Inicializa o objeto **CChkSGFiles** especificando os bancos de dados a serem verificados e o caminho e o nome base dos arquivos de log de transação a serem verificados. Os aplicativos devem chamar essa função imediatamente após chamar com êxito a **função** New. 
  
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
  
Parâmetro de entrada. Uma matriz que especifica os bancos de dados a serem verificados. Cada elemento de matriz é uma cadeia de caracteres Unicode terminada em nulo que contém o caminho e o nome do arquivo de um banco de dados a ser verificado.
    
### <a name="cdb"></a>cDB
  
Parâmetro de entrada. O número de elementos de caminho de banco de dados válidos na **matriz rgwszDb.** 
    
#### <a name="wszlogpath"></a>wszLogPath
  
Parâmetro de entrada. O caminho completo dos arquivos de log de transação a serem verificados, na forma de uma cadeia de caracteres Unicode terminada em nulo.
    
### <a name="wszbasename"></a>wszBaseName
  
Parâmetro de entrada. O nome base de três letras dos arquivos Exchange de log de transação, na forma de uma cadeia de caracteres Unicode terminada em nulo.
    
### <a name="ulflags"></a>ulFlags
  
Parâmetro de entrada opcional. Esse valor é reservado para uso futuro. O valor passado por esse parâmetro deve ser 0 (zero).
    
## <a name="return-value"></a>Valor de retorno

Um código de erro da [enumeração ERR.](cchksgfiles-err-enumeration.md) 
  
## <a name="remarks"></a>Comentários

A **função ErrInit** registra os bancos de dados e os arquivos de log que devem ser verificados. Essa função deve ser chamada depois que **a função New** for chamada, mas antes que qualquer outra função **ChkSGFiles** seja chamada. 
  
Você deve fornecer todos os nomes de banco de dados, o caminho do arquivo de log e o nome base como cadeias de caracteres Unicode terminadas por nulo.
  
Você pode verificar apenas os arquivos de banco de dados, somente os arquivos de log ou o banco de dados e os arquivos de log. No entanto, ao chamar essa função, o aplicativo deve especificar pelo menos uma entidade a ser verificada. Passar 0 (zero) para  **cDB**  e NULL para  **wszLogPath**  retornará um erro. 
  
Se o valor de  **cDB**  for diferente de 0 (zero), passar NULL para  **rgwszDb**  resultará em um erro. Para verificar os arquivos de banco de dados, o aplicativo deve fornecer os nomes do banco de dados. 
  
Se NULL for passado para  **wszBaseName,**  mas  **wszLogPath**  não for NULL, um erro será retornado. Um nome de base de arquivo de log é sempre necessário ao verificar arquivos de log. 
  
Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você deve chamar a função **ErrInit** na parte de thread único do aplicativo e pode chamá-la apenas uma vez para cada **objeto CCheckSGFiles.** 
  
## <a name="requirements"></a>Requisitos

Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta em que o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

