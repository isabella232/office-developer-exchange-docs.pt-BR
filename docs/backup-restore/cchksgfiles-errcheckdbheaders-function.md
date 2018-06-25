---
title: Função CChkSGFiles.ErrCheckDbHeaders
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckDbHeaders
api_type:
- dllExport
ms.assetid: 75289cd2-35b1-4f75-a651-dce01f1ddda1
description: 'Modificado pela última vez: 22 de fevereiro de 2013'
ms.openlocfilehash: a407019063b34970e883a00ca4f4d730935d7cba
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750636"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a>Função CChkSGFiles.ErrCheckDbHeaders

**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 
  
Valida os cabeçalhos dos arquivos de banco de dados que foram especificados pela função **ErrInit** . Essa função também retornará o tamanho de página e o número de páginas em cada um dos bancos de dados especificados. 
  
```cs
Vitual ERRErrCheckDbHeaders  
(
        ULONG  * const pcbDbPageSize,
        ULONG  * const pcHeaderPagesPerDb,
        ULONG   const piDbErrorEncountered,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Par�metros

### <a name="pcbdbpagesize"></a>pcbDbPageSize 
  
Parâmetro de saída. O tamanho de página de cada banco de dados especificados, em bytes.
    
### <a name="pcheaderpagesperdb"></a>pcHeaderPagesPerDb 
  
Parâmetro de saída. O número de páginas no início de cada especificado banco de dados que são reservados pelo mecanismo de banco de dados para uso interno. Observe que você deve *secreta páginas de cabeçalho para a função **ErrCheckDbPages** para validação* . 
    
### <a name="pidberrorencountered"></a>piDbErrorEncountered
  
Parâmetro de saída. Se o valor de retorno da função indica um erro, esse parâmetro será um índice na matriz **[] de rgwszDb** passado para a função **ErrInit** . O elemento de matriz indexada representa o banco de dados no qual o erro foi encontrado. Se a função não retorna um valor de erro, o valor do parâmetro é inválido. 
    
### <a name="ulflags"></a>ulFlags 
  
Parâmetro de entrada opcional. Esse valor é reservado para uso futuro. O valor passado deve ser de 0 (zero).
    
## <a name="return-value"></a>Valor retornado

Essa função retornará um código de erro da [enumeração CChkSGFiles.ERR](cchksgfiles-err-enumeration.md).
  
## <a name="remarks"></a>Comentários

**ErrCheckDbHeaders** certifica-se de que todos os bancos de dados registrados com **ErrInit** tenham o mesmo log assinatura e do banco de dados do tamanho da página. Você também pode usar o menor valor de parâmetro de **genMin** e o maior valor do parâmetro **genMax** para determinar o conjunto de arquivos de log que são necessárias para colocar todos os bancos de dados registrados em um estado de desligamento. 
  
O parâmetro **piDbErrorEncountered** é definido somente quando for detectado um erro, conforme indicado por uma diferente de zero **ErrCheckDbHeaders** o valor de retorno. 
  
Quando ocorre um erro nessa função, será adicionado um evento de erro no log de eventos de erro do Windows.
  
Você pode chamar **ErrCheckDbHeaders** somente depois de chamar **ErrInit**e você deverá chamá-la antes de chamar **ErrCheckDbPages** e **ErrCheckLogs**.
  
Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você deve chamar a função **ErrCheckDbHeaders** na parte com um único segmento e você poderá chamá-lo apenas uma vez para cada objeto **CCheckSGFiles** . 
  
## <a name="requirements"></a>Requisitos

Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.
  

