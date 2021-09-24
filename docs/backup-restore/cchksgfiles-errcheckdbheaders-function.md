---
title: Função CChkSGFiles.ErrCheckDbHeaders
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ErrCheckDbHeaders
api_type:
- dllExport
ms.assetid: 75289cd2-35b1-4f75-a651-dce01f1ddda1
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: 215a0d1126fce48b7e3800016619b0c52915312b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510467"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a>Função CChkSGFiles.ErrCheckDbHeaders

**Aplica-se a: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 
  
Valida os headers dos arquivos de banco de dados especificados pela **função ErrInit.** Essa função também retorna o tamanho da página e o número de páginas em cada um dos bancos de dados especificados. 
  
```cs
Vitual ERRErrCheckDbHeaders  
(
        ULONG  * const pcbDbPageSize,
        ULONG  * const pcHeaderPagesPerDb,
        ULONG   const piDbErrorEncountered,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Parâmetros

### <a name="pcbdbpagesize"></a>pcbDbPageSize 
  
Parâmetro de saída. O tamanho da página de cada um dos bancos de dados especificados, em bytes.
    
### <a name="pcheaderpagesperdb"></a>pcHeaderPagesPerDb 
  
Parâmetro de saída. O número de páginas no início de cada banco de dados especificado reservado pelo mecanismo de banco de dados para uso interno. Observe que você *não deve passar* páginas de header para a função **ErrCheckDbPages** para validação. 
    
### <a name="pidberrorencountered"></a>piDbErrorEncountered
  
Parâmetro de saída. Se o valor de retorno da função indicar um erro, esse parâmetro será um índice para a matriz **rgwszDb[]** passada para a **função ErrInit.** O elemento de matriz indexada representa o banco de dados no qual o erro foi encontrado. Se a função não retornar um valor de erro, esse valor de parâmetro será inválido. 
    
### <a name="ulflags"></a>ulFlags 
  
Parâmetro de entrada opcional. Esse valor é reservado para uso futuro. O valor passado deve ser 0 (zero).
    
## <a name="return-value"></a>Valor de retorno

Esta função retorna um código de erro da [enumeração CChkSGFiles.ERR](cchksgfiles-err-enumeration.md).
  
## <a name="remarks"></a>Comentários

**ErrCheckDbHeaders** verifica se todos os bancos de dados registrados com **ErrInit** têm a mesma assinatura de log e o tamanho da página do banco de dados. Você também pode usar o valor do parâmetro **genMin** mais baixo e o valor de parâmetro **genMax** mais alto para determinar o conjunto de arquivos de log necessários para levar todos os bancos de dados registrados para um estado de desligamento limpo. 
  
O **parâmetro piDbErrorEncountered** é definido somente quando um erro é detectado, conforme indicado por um valor de retorno **errCheckDbHeaders** não zero. 
  
Quando ocorrer um erro nessa função, um evento de erro será adicionado ao log de eventos Windows Erro.
  
Você pode chamar **ErrCheckDbHeaders** somente depois de chamar **ErrInit**, e você deve chamá-lo antes de **chamar ErrCheckDbPages** e **ErrCheckLogs**.
  
Se você estiver usando CHKSGFILES em um aplicativo multithreaded, deverá chamar a **função ErrCheckDbHeaders** na parte de thread único e poderá chamá-la apenas uma vez para cada **objeto CCheckSGFiles.** 
  
## <a name="requirements"></a>Requisitos

Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta em que o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

