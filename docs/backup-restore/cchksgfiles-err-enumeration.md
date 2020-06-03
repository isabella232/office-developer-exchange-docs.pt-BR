---
title: Enumeração função cchksgfiles. ERR
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ERR
api_type:
- dllExport
ms.assetid: f0efe195-91c3-4f3a-8c7d-e5dba336465a
description: 'Última modificação: 9 de março de 2015'
ms.openlocfilehash: dbc76601a808f79ce3ed5b5dc9fbe4cf92efb015
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455251"
---
# <a name="cchksgfileserr-enumeration"></a>Enumeração função cchksgfiles. ERR 
  
**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Indica os resultados da função chamada. Essa enumeração é retornada por muitas funções da classe **CCheckSGFiles** . 
  
```cs
Enum ERR  
{
        errSuccess = 0,
        errTaskDropped = -106,
        errRequiredLogFilesMissing = -543,
        errInvalidParameter = -1003,
        errOutOfMemory = -1011,
        errReadVerifyFailure = -1018,
        errTooManyActiveUsers = -1059,
        errDatabaseCorrupted = -1206
}

```

## <a name="values"></a>Values

|**Nome do membro**|**Valor**|**Descrição**|
|:-----|:-----|:-----|
|errSuccess  <br/> |,0  <br/> |A função foi concluída sem erros.  <br/> |
|errTaskDropped  <br/> |-106  <br/> |Retornado pela função **ErrTerm** para indicar que nem todas as páginas do banco de dados e os arquivos de log de transações foram verificados ou que foram encontrados erros durante a verificação.  <br/> |
|errRequiredLogFilesMissing  <br/> |-543  <br/> |Um ou mais arquivos de log necessários para colocar o banco de dados em um estado de desligamento normal não foram encontrados no caminho do arquivo de log ou não tinham o nome da base de três letras especificado.  <br/> |
|errInvalidParameter  <br/> |-1003  <br/> |Um ou mais parâmetros que foram passados para a função eram inválidos.  <br/> |
|errOutOfMemory  <br/> |-1011  <br/> |Memória insuficiente disponível para concluir a operação solicitada.  <br/> |
|errReadVerifyFailure  <br/> |-1018  <br/> |O checksum armazenado em uma página de banco de dados não corresponde à soma de verificação esperada.  <br/> |
|errTooManyActiveUsers  <br/> |-1059  <br/> |A função **ErrTerm** foi chamada enquanto o objeto ainda estava sendo usado. Isso pode ocorrer se **ErrTerm** for chamado antes de **ErrCheckDbPages** ou **ErrCheckLogFiles** ter retornado.  <br/> |
   
## <a name="requirements"></a>Requirements

O Exchange Server 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

