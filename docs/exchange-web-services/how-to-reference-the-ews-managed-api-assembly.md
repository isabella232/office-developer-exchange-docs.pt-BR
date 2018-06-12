---
title: Faça referência ao conjunto de API gerenciada de EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 130990db-6297-42dc-9f5d-f68a2400872a
description: Encontre informações sobre como fazer referência ao conjunto de API gerenciada de EWS.
ms.openlocfilehash: af7b1ec449c24e7fa4db89abb30e5ebc9f8d329e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750813"
---
# <a name="reference-the-ews-managed-api-assembly"></a>Faça referência ao conjunto de API gerenciada de EWS

Encontre informações sobre como fazer referência ao conjunto de API gerenciada de EWS.
  
A API gerenciada de EWS fornece uma interface simple e completo para o desenvolvimento e estendendo aplicativos que utilizam serviços Web do Exchange (EWS). Se você estiver usando o Visual Studio ou outro editor de código para desenvolver seu aplicativo EWS Managed API, você precisará fazer uma referência para o assembly do EWS Managed API. Se você já não tiver instalado o EWS Managed API, certifique-se de fazer o [download da API](http://aka.ms/ews-managed-api-readme).
  
> [!NOTE]
>  A API gerenciada de EWS agora está disponível como um projeto de código aberto no [GitHub](https://github.com/officedev/ews-managed-api). Você pode usar a biblioteca de fonte aberta: > correções e melhorias para a API de colaboração. > Obtenha correções e aprimoramentos antes que estejam disponíveis em um lançamento oficial. > Acesso a implementação mais abrangente e atualizado da API, para usar como uma referência ou para criar novas bibliotecas em plataformas novas. > Bem-vindos suas [contribuições](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub. 
  
## <a name="referencing-the-assembly"></a>Fazendo referência o assembly

A maneira mais comum para adicionar uma referência é usar o Visual Studio. Nós sabemos que alguns desenvolvedores por aí gostam de usar outros editores, portanto incluímos instruções sobre como usar o compilador de linha de comando, assim como as instruções para usar o Visual Studio. Você pode observar que os exemplos de código que seguem tenham as mesmas instruções de **uso** . A diferença entre os dois métodos é que o compilador de linha de comando precisa do local do arquivo de assembly. Referência do Visual Studio trata isso para você em segundo plano. 
  
### <a name="to-add-a-reference-by-using-visual-studio"></a>Para adicionar uma referência usando o Visual Studio

1. Coloca o arquivo Microsoft.Exchange.WebServices.dll e o arquivo de Microsoft.Exchange.WebServices.xml em uma pasta de sua escolha. Por padrão, os arquivos são instalados no `C:\Program Files\Microsoft\Exchange\Web Services\2.0\`, mas você pode armazenar os arquivos em qualquer lugar em seu computador.
    
2. No painel Gerenciador de soluções no Visual Studio, selecione **referências**e escolha **Adicionar referência**. Isso abre a janela de adicionar referência.
    
3. Na janela Adicionar referência, navegue até a guia **Procurar** , navegue até o local do arquivo Microsoft.Exchange.WebServices.dll, selecione esse arquivo e selecione **Okey**. 
    
4. Para usar a API gerenciada de EWS em seu aplicativo, adicione uma declaração **using** para o namespace **Microsoft.Exchange.WebServices.Data** . 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

### <a name="to-add-a-reference-and-build-your-application-with-the-command-line-compiler"></a>Para adicionar uma referência e criar o seu aplicativo com o compilador de linha de comando

1. Coloque o arquivo de Microsoft.Exchange.WebServices.dll em uma pasta de sua escolha. Essa pasta será a pasta de saída para o compilador.
    
2. No seu editor de código fonte, adicione uma instrução **usando** o código-fonte para o namespace **Microsoft.Exchange.WebServices.Data** . 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

3. Execute o compilador de linha de comando para criar o aplicativo. O comando a seguir usa o .NET Framework compilador c# para criar o aplicativo do Windows definido no arquivo de código fonte "Module. vb". Ele pressupõe que o compilador está localizado no diretório de instalação padrão e que o arquivo de Microsoft.Exchange.WebServices.dll está em um subdiretório do diretório atual chamado "build".
    
   ```cs
    c:\Windows\Microsoft.NET\Framework\3.5\csc /target: winexe /out: build\testApplication /reference: build\Microsoft.Exchange.WebServices.dll program.cs
   ```

## <a name="see-also"></a>Confira também

- [Introdução aos aplicativos de cliente API gerenciada de EWS](get-started-with-ews-managed-api-client-applications.md)    
- [Configurando o ambiente de desenvolvimento de aplicativos do Exchange](setting-up-your-exchange-application-development-environment.md)   
- [Comunicar-se com o EWS usando a API gerenciada de EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

