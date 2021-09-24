---
title: Função CChkSGFiles.ErrTerm
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ErrTerm
api_type:
- dllExport
ms.assetid: eea20a55-4a2a-4209-ae79-dc1ee1cd631b
description: 'Última modificação: 25 de fevereiro de 2013'
ms.openlocfilehash: 152fd613ef461d8c1ef69401237cfea09cd32b08
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516283"
---
# <a name="cchksgfileserrterm-function"></a>Função CChkSGFiles.ErrTerm
  
**Aplica-se a: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Fornece um status geral do banco de dados e da verificação de log, que indica se todas as páginas e logs do banco de dados foram verificados com êxito.
  
> [!IMPORTANT]
> Armazenamento grupos não estão disponíveis no Exchange 2013. Para compatibilidade com bancos de dados e grupos de armazenamento em versões do Exchange anteriores ao Exchange Server 2010, a API CHKSGFILES permite especificar grupos de armazenamento. Ao executar CHKSGFILES em Exchange bancos de dados 2013, você deve definir parâmetros que especificam um identificador de grupo de armazenamento como uma cadeia de caracteres vazia. 
  
```cs
Vitual ERRErrTerm 
(
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Parâmetros

### <a name="ulflags"></a>ulFlags
  
Parâmetro de entrada opcional. Esse valor é reservado para uso futuro. O valor passado por esse parâmetro deve ser 0 (zero).
    
## <a name="return-value"></a>Valor de retorno

Um código de erro da [enumeração ERR.](cchksgfiles-err-enumeration.md) 
  
## <a name="remarks"></a>Comentários

O **objeto CChkSGFiles** determina se todos os bancos de dados registrados com a **função ErrInit** foram realmente verificados. Esse objeto usa a **função ErrCheckDbPages** para verificar se o mesmo número de páginas de banco de dados identificadas pela **função ErrCheckDbHeaders** foi realmente verificado. Se o número correto de páginas em cada banco de dados não for verificado com êxito, a **função ErrTerm** retornará um erro. 
  
Se o número de páginas de banco de dados verificadas com **ErrCheckDbPages** for menor do que o indicado por **ErrCheckDbHeaders,** essa função criará um erro no log de eventos Windows e **ErrTerm** retornará um erro. 
  
Se o número de páginas de banco de dados verificadas com **ErrCheckDbPages** for maior do que o indicado por **ErrCheckDbHeaders,** essa função criará um aviso no log de eventos do Windows para indicar que o aplicativo pode estar verificando desnecessariamente algumas páginas de banco de dados mais de uma vez. Nesse caso, no entanto, a **função ErrTerm** é bem-sucedida. 
  
O **objeto CChkSGFiles** também determina se os arquivos de log registrados com **ErrInit** foram realmente verificados. Se nem todos os logs foram verificados com êxito, a **função ErrTerm** retornará um erro. 
  
Quando **ErrTerm** retorna um erro, ele será o primeiro erro encontrado, mesmo que ele verifique o status de verificação de todos os bancos de dados registrados com **ErrInit**.
  
Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você deve chamar a função **ErrTerm** na parte de thread único do aplicativo e não pode chamá-la mais de uma vez para cada **objeto CCheckSGFiles.** 
  
## <a name="requirements"></a>Requisitos

Exchange 2013 inclui apenas uma versão de 64 bits do CHKSGFILES.
  
A conta em que o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

