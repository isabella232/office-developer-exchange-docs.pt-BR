---
title: Referência da classe CChkSGFiles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9347d5f6-95bb-4045-9c86-0dc0ded24fe8
description: Encontre informações de referência para a API CHKSGFILES no Exchange 2013.
ms.openlocfilehash: 2daf31c41a47684b85ede196b415884335c3ca79
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510529"
---
# <a name="cchksgfiles-class-reference"></a>Referência da classe CChkSGFiles

Encontre informações de referência para a API CHKSGFILES no Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013 
  
A API CHKSGFILES permite que aplicativos de backup e restauração verifiquem Exchange Server arquivos de log de transações e bancos de dados de 2013 programaticamente. Você pode usar essa API em aplicativos de backup e restauração que usam o Serviço de Cópia de Sombra de Volume (VSS).
  
> [!NOTE]
> Armazenamento grupos não estão disponíveis no Exchange 2013. O suporte para grupos de armazenamento foi removido das versões do Exchange a partir do Exchange Server 2010. Para compatibilidade com bancos de dados e grupos de armazenamento em versões do Exchange anteriores ao Exchange 2010, a API CHKSGFILES permite especificar grupos de armazenamento. Ao executar CHKSGFILES em Exchange bancos de dados 2013, você deve definir parâmetros que especificam um identificador de grupo de armazenamento como uma cadeia de caracteres vazia. 
  
## <a name="file-location"></a>Local do arquivo
<a name="bk_fileslocation"> </a>

A API CHKSGFILES é Exchange 2013. Você pode usar essa API em um computador que tenha a função de servidor de Caixa de Correio instalada. 
  
Por padrão, a DLL CHKSGFILES é instalada no diretório C:\Program Files\Microsoft\Exchange\V15\Bin.
  
Exchange 2013 inclui apenas uma versão de 64 bits (amd64) da API CHKSGFILES. 
  
Você pode baixar um arquivo .zip que inclui a biblioteca CHKSGFILE.lib e os arquivos de header CHKSGFILES.hxx para uso em seu aplicativo personalizado do Centro de Download da [Microsoft](https://www.microsoft.com/download/details.aspx?id=36802).
  
## <a name="development-languages"></a>Idiomas de desenvolvimento
<a name="bk_developmentlanguages"> </a>

A API CHKSGFILES destina-se a ser usada com versões do Visual Studio começando com Visual Studio 2005 em C/C++nativo. A API CHKSGFILES não se destina ao uso no código gerenciado. Embora você possa criar um assembly de interop COM com CHKSGFILES, não enviaremos um assembly de interop COM com suporte com Exchange 2013.
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Função CChkSGFiles.CMaxDbPerSG](cchksgfiles-cmaxdbpersg-function.md)
    
- [Função CChkSGFiles.Delete](cchksgfiles-delete-function.md)
    
- [Enumeração CChkSGFiles.ERR](cchksgfiles-err-enumeration.md)
    
- [Função CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md)
    
- [Função CChkSGFiles.ErrCheckDbPages](cchksgfiles-errcheckdbpages-function.md)
    
- [Função CChkSGFiles.ErrCheckLogs](cchksgfiles-errchecklogs-function.md)
    
- [Função CChkSGFiles.ErrGetHeader (reservada)](cchksgfiles-errgetheader-function-reserved.md)
    
- [Função CChkSGFiles.ErrInit](cchksgfiles-errinit-function.md)
    
- [Função CChkSGFiles.ErrTerm](cchksgfiles-errterm-function.md)
    
- [Enumeração CChkSGFiles.iDbInvalid](cchksgfiles-idbinvalid-enumeration.md)
    
- [Função CChkSGFiles.New](cchksgfiles-new-function.md)
    
- [Enumeração CChkSGFiles.NO_FLAGS](cchksgfiles-no_flags-enumeration.md)
    
- [Estrutura CChkSGFiles.PAGE_INFO](cchksgfiles-page_info-struct.md)
    
- [Função CChkSGFiles.PgnoFromFileOffset](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a>Confira também

- [Desenvolvimento do Exchange Online e do Exchange](../exchange-server-development.md)
- [Backup, restauração e recuperação de desastres](https://technet.microsoft.com/library/dd876874)
    

