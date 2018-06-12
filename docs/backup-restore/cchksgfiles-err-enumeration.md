---
title: Enumeração CChkSGFiles.ERR
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
description: '�ltima altera��o: segunda-feira, 9 de mar�o de 2015'
ms.openlocfilehash: 20f10c43e3b92604bb51e1aa5f896a8bd7c4b335
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751575"
---
# <a name="cchksgfileserr-enumeration"></a>Enumeração CChkSGFiles.ERR 
  
**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Indica os resultados da função chamada. Esta enumeração é retornada por muitas funções da classe **CCheckSGFiles** . 
  
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

## <a name="values"></a>Valores

|**Nome do membro**|**Valor**|**Descrição**|
|:-----|:-----|:-----|
|errSuccess  <br/> |0  <br/> |A função concluída sem erros.  <br/> |
|errTaskDropped  <br/> |-106  <br/> |Retornado pela função **ErrTerm** para indicar que nem todas as páginas do banco de dados e arquivos de log de transações marcados ou que foram encontrados erros durante a verificação.  <br/> |
|errRequiredLogFilesMissing  <br/> |-543  <br/> |Um ou mais arquivos de log que são necessários para que o banco de dados para um estado de desligamento não foi encontrado no caminho do arquivo de log ou não tinha o nome de base de três letras especificado.  <br/> |
|errInvalidParameter  <br/> |-1003  <br/> |Um ou mais parâmetros que foram passados para a função eram inválidos.  <br/> |
|errOutOfMemory  <br/> |-1011  <br/> |Memória insuficiente estava disponível para concluir a operação solicitada.  <br/> |
|errReadVerifyFailure  <br/> |-1018  <br/> |A soma de verificação que é armazenada em uma página de banco de dados não coincide com sua soma de verificação esperada.  <br/> |
|errTooManyActiveUsers  <br/> |-1059  <br/> |A função **ErrTerm** foi chamada enquanto o objeto ainda estava sendo usado. Isso pode ocorrer se **ErrTerm** é chamado antes **ErrCheckDbPages** ou **ErrCheckLogFiles** ter retornado.  <br/> |
   
## <a name="requirements"></a>Requisitos

Exchange Server 2013 apenas inclui uma versão de 64 bits da API CHKSGFILES.
  
A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.
  

