---
title: Fazer referência ao assembly da API gerenciada do EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 130990db-6297-42dc-9f5d-f68a2400872a
description: Encontre informações sobre como fazer referência ao assembly da API gerenciada do EWS.
localization_priority: Priority
ms.openlocfilehash: d49091781da279d87a1eab35608f19ece43a0333
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527758"
---
# <a name="reference-the-ews-managed-api-assembly"></a>Fazer referência ao assembly da API gerenciada do EWS

Encontre informações sobre como fazer referência ao assembly da API gerenciada do EWS.
  
A API gerenciada do EWS fornece uma interface simples e com recursos completos para desenvolver e estender aplicativos que usam os serviços Web do Exchange (EWS). Se você estiver usando o Visual Studio ou outro editor de código para desenvolver seu aplicativo de API gerenciada do EWS, será necessário fazer uma referência ao assembly da API gerenciada do EWS. Se você ainda não instalou a API gerenciada do EWS, não se esqueça de [baixar a API](https://aka.ms/ews-managed-api-readme).
  
> [!NOTE]
> A API gerenciada do EWS já está disponível como um projeto de código-fonte aberto no [GitHub](https://github.com/officedev/ews-managed-api). É possível usar a biblioteca de software livre para: 
> - Contribui com correções de bug e melhorias à API. 
> - Obtenha correções e melhorias antes que estejam disponíveis em uma versão oficial. 
> - Acesse a implementação mais abrangente e atualizada da API, para usar como referência ou criar novas bibliotecas em novas plataformas. 
> 
>  Agradecemos suas [contribuições](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via github. 
  
## <a name="referencing-the-assembly"></a>Fazer referência ao assembly

A maneira mais comum de adicionar uma referência é usar o Visual Studio. Sabemos que alguns desenvolvedores gostam de usar outros editores, portanto, estamos incluindo instruções para usar o compilador de linha de comando e instruções para usar o Visual Studio. Você pode notar que os exemplos de código a seguir têm as mesmas instruções **using** . A diferença entre os dois métodos é que o compilador de linha de comando precisa do local do arquivo de assembly. A referência do Visual Studio trata isso para você em segundo plano. 
  
### <a name="to-add-a-reference-by-using-visual-studio"></a>Para adicionar uma referência usando o Visual Studio

1. Coloque o arquivo Microsoft. Exchange. WebServices. dll e o arquivo Microsoft. Exchange. WebServices. xml em uma pasta de sua escolha. Por padrão, os arquivos são instalados no `C:\Program Files\Microsoft\Exchange\Web Services\2.0\` , mas você pode armazenar os arquivos em qualquer lugar no seu computador.
    
2. No painel Gerenciador de soluções no Visual Studio, selecione **referências**e, em seguida, escolha **Adicionar referência**. Isso abre a janela Adicionar referência.
    
3. Na janela Adicionar referência, navegue até a guia **procurar** , navegue até o local do arquivo Microsoft. Exchange. WebServices. dll, selecione esse arquivo e, em seguida, selecione **OK**. 
    
4. Para usar a API gerenciada do EWS em seu aplicativo, adicione uma instrução **using** para o namespace **Microsoft. Exchange. WebServices. Data** . 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

### <a name="to-add-a-reference-and-build-your-application-with-the-command-line-compiler"></a>Para adicionar uma referência e compilar seu aplicativo com o compilador de linha de comando

1. Coloque o arquivo Microsoft. Exchange. WebServices. dll em uma pasta de sua escolha. Esta pasta será a pasta de saída para o compilador.
    
2. No editor de código-fonte, adicione uma instrução **using** ao código-fonte do namespace **Microsoft. Exchange. WebServices. Data** . 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

3. Execute o compilador de linha de comando para compilar o aplicativo. O comando a seguir usa o compilador C# do .NET Framework para criar o aplicativo do Windows definido no arquivo de código-fonte "program.cs". Ele pressupõe que o compilador está localizado no diretório de instalação padrão e que o arquivo Microsoft. Exchange. WebServices. dll está em um subdiretório do diretório atual chamado "Build".
    
   ```cs
    c:\Windows\Microsoft.NET\Framework\3.5\csc /target: winexe /out: build\testApplication /reference: build\Microsoft.Exchange.WebServices.dll program.cs
   ```

## <a name="see-also"></a>Confira também

- [Introdução aos aplicativos clientes de API gerenciada por EWS](get-started-with-ews-managed-api-client-applications.md)    
- [Configurando seu ambiente de desenvolvimento de aplicativos do Exchange](setting-up-your-exchange-application-development-environment.md)   
- [Comunicar-se com o EWS usando a API gerenciada do EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

