---
title: Função função cchksgfiles. ErrCheckDbHeaders
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
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: a62c5940322d3d7a71f2db93214f1e970fc6859b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455244"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a>Função função cchksgfiles. ErrCheckDbHeaders

**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 
  
Valida os cabeçalhos dos arquivos de banco de dados que foram especificados pela função **ErrInit** . Essa função também retorna o tamanho da página e o número de páginas em cada um dos bancos de dados especificados. 
  
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
  
Parâmetro de saída. O tamanho de página de cada um dos bancos de dados especificados, em bytes.
    
### <a name="pcheaderpagesperdb"></a>pcHeaderPagesPerDb 
  
Parâmetro de saída. O número de páginas no início de cada banco de dados especificado que são reservados pelo mecanismo de banco de dados para uso interno. Observe que você *não* deve passar páginas de cabeçalho para a função **ErrCheckDbPages** para validação. 
    
### <a name="pidberrorencountered"></a>piDbErrorEncountered
  
Parâmetro de saída. Se o valor de retorno da função indicar um erro, esse parâmetro será um índice na matriz **rgwszDb []** passada para a função **ErrInit** . O elemento de matriz indexada representa o banco de dados no qual o erro foi encontrado. Se a função não retornar um valor de erro, esse valor de parâmetro é inválido. 
    
### <a name="ulflags"></a>ulFlags 
  
Parâmetro de entrada opcional. Esse valor é reservado para uso futuro. O valor passado deve ser 0 (zero).
    
## <a name="return-value"></a>Valor de retorno

Essa função retorna um código de erro da [Enumeração função cchksgfiles. err](cchksgfiles-err-enumeration.md).
  
## <a name="remarks"></a>Comentários

**ErrCheckDbHeaders** verifica se todos os bancos de dados registrados com **ErrInit** têm a mesma assinatura de log e o tamanho da página do banco de dados. Você também pode usar o menor valor de parâmetro **genMin** e o valor de parâmetro de **genMax** mais alto para determinar o conjunto de arquivos de log que são necessários para colocar todos os bancos de dados registrados em um estado de desligamento normal. 
  
O parâmetro **piDbErrorEncountered** é definido somente quando um erro é detectado, conforme indicado por um valor de retorno diferente de zero **ErrCheckDbHeaders** . 
  
Quando ocorrer um erro nesta função, um evento de erro será adicionado ao log de eventos de erro do Windows.
  
Você pode chamar **ErrCheckDbHeaders** somente depois de chamar **ErrInit**e deve chamá-lo antes de chamar **ErrCheckDbPages** e **ErrCheckLogs**.
  
Se você estiver usando o CHKSGFILES em um aplicativo multi-threaded, deverá chamar a função **ErrCheckDbHeaders** na parte de thread único e você poderá chamá-la apenas uma vez para cada objeto **CCheckSGFiles** . 
  
## <a name="requirements"></a>Requirements

O Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

