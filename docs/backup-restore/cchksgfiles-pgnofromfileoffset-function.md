---
title: Função CChkSGFiles.PgnoFromFileOffset
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PgnoFromFileOffset
api_type:
- dllExport
ms.assetid: 3d69ca6d-5ed1-4038-859e-106e776eeec1
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: 3e2845cc326520ad875dc8bda52bac3d7c2e2cfa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516241"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a>Função CChkSGFiles.PgnoFromFileOffset

**Aplica-se a: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Retorna o número de página do banco de dados lógico que corresponde ao índice de byte especificado no arquivo de banco de dados físico. Se o deslocamento de arquivo for inválido ou se a **função ErrCheckDbHeaders** não tiver sido chamada para os bancos de dados, essa função retornará 0 (zero). 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a>Parâmetros

### <a name="ibfileoffset"></a>ibFileOffset
  
Parâmetro de entrada. O deslocamento em um arquivo de banco de dados, em bytes.
    
## <a name="return-value"></a>Valor de retorno

O número da página lógica do arquivo de banco de dados que inclui o deslocamento especificado.
  
## <a name="remarks"></a>Comentários

Se o **parâmetro ibFileOffset** for inválido, a **função PgnoFromFileOffset** retornará 0 (zero). 
  
**PgnoFromFileOffset** também retornará 0 (zero) se você não tiver chamado a **função ErrCheckDbHeaders** na **instância CCheckSGFiles.** Você deve chamar **ErrCheckDbHeaders** para inicializar o tamanho da página do banco de dados e o número de páginas alocadas aos headers do banco de dados. 
  
Você deve usar **PgnoFromFileOffset** para preencher os elementos da estrutura **PAGE \_ INFO** em preparação para chamar **ErrCheckDbPages**. O **parâmetro rgPageInfo** para **ErrCheckDbPages** exige que  cada elemento na matriz seja uma estrutura PAGE_INFO, com os valores de membro **ulPgno** inicializados corretamente. 
  
Se você estiver usando CHKSGFILES em um aplicativo multithreaded, poderá chamar a **função PgnoFromFileOffset** na parte multithreaded do aplicativo. Observe que você normalmente chamaria essa função várias vezes para cada banco de dados que está sendo verificado. 
  
## <a name="requirements"></a>Requisitos

Exchange Server 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta em que o aplicativo está sendo executado deve ter permissão de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

