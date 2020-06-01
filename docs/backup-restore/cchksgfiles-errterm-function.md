---
title: Função função cchksgfiles. ErrTerm
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrTerm
api_type:
- dllExport
ms.assetid: eea20a55-4a2a-4209-ae79-dc1ee1cd631b
description: 'Última modificação: 25 de fevereiro de 2013'
ms.openlocfilehash: 12b07fba69054d327c7250bbf83e4c77016e8b3f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466196"
---
# <a name="cchksgfileserrterm-function"></a>Função função cchksgfiles. ErrTerm
  
**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Fornece um status geral do banco de dados e verificação de log, que indica se todas as páginas de banco de dados e logs foram verificadas com êxito.
  
> [!IMPORTANT]
> Os grupos de armazenamento não estão disponíveis no Exchange 2013. Para compatibilidade com versões anteriores com bancos de dados e grupos de armazenamento em versões do Exchange anteriores ao Exchange Server 2010, a API CHKSGFILES permite que você especifique grupos de armazenamento. Ao executar o CHKSGFILES em bancos de dados do Exchange 2013, você deve definir parâmetros que especificam um identificador de grupo de armazenamento para uma cadeia de caracteres vazia. 
  
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

Um código de erro da enumeração [Err](cchksgfiles-err-enumeration.md) . 
  
## <a name="remarks"></a>Comentários

O objeto **função cchksgfiles** determina se todos os bancos de dados registrados com a função **ErrInit** foram realmente verificados. Este objeto usa a função **ErrCheckDbPages** para verificar se o mesmo número de páginas de banco de dados identificadas pela função **ErrCheckDbHeaders** foram realmente verificados. Se o número correto de páginas em cada banco de dados não for verificado com êxito, a função **ErrTerm** retornará um erro. 
  
Se o número de páginas de banco de dados verificadas com **ErrCheckDbPages** for menor que o indicado por **ErrCheckDbHeaders**, essa função cria um erro no log de eventos do Windows e **ErrTerm** retorna um erro. 
  
Se o número de páginas de banco de dados verificadas com **ErrCheckDbPages** for maior que o indicado por **ErrCheckDbHeaders**, essa função cria um aviso no log de eventos do Windows para indicar que o aplicativo pode estar desnecessariamente verificando algumas páginas de banco de dados mais de uma vez. Nesse caso, no entanto, a função **ErrTerm** é bem-sucedida. 
  
O objeto **função cchksgfiles** também determina se os arquivos de log registrados no **ErrInit** foram realmente verificados. Se nem todos os logs foram verificados com êxito, a função **ErrTerm** retornará um erro. 
  
Quando **ErrTerm** retornar um erro, ele será o primeiro erro encontrado, mesmo que verifique o status de verificação de todos os bancos de dados registrados no **ErrInit**.
  
Se você estiver usando o CHKSGFILES em um aplicativo multi-threaded, deverá chamar a função **ErrTerm** na parte de thread único do aplicativo, e poderá chamá-la não mais do que uma vez para cada objeto **CCheckSGFiles** . 
  
## <a name="requirements"></a>Requirements

O Exchange 2013 inclui apenas uma versão de 64 bits do CHKSGFILES.
  
A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

