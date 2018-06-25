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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750813"
---
# <a name="reference-the-ews-managed-api-assembly"></a><span data-ttu-id="91da8-103">Faça referência ao conjunto de API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="91da8-103">Reference the EWS Managed API assembly</span></span>

<span data-ttu-id="91da8-104">Encontre informações sobre como fazer referência ao conjunto de API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="91da8-104">Find information about how to reference the EWS Managed API assembly.</span></span>
  
<span data-ttu-id="91da8-105">A API gerenciada de EWS fornece uma interface simple e completo para o desenvolvimento e estendendo aplicativos que utilizam serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="91da8-105">The EWS Managed API provides a simple and full-featured interface for developing and extending applications that use Exchange Web Services (EWS).</span></span> <span data-ttu-id="91da8-106">Se você estiver usando o Visual Studio ou outro editor de código para desenvolver seu aplicativo EWS Managed API, você precisará fazer uma referência para o assembly do EWS Managed API.</span><span class="sxs-lookup"><span data-stu-id="91da8-106">Whether you are using Visual Studio or another code editor to develop your EWS Managed API application, you will need to make a reference to the EWS Managed API assembly.</span></span> <span data-ttu-id="91da8-107">Se você já não tiver instalado o EWS Managed API, certifique-se de fazer o [download da API](http://aka.ms/ews-managed-api-readme).</span><span class="sxs-lookup"><span data-stu-id="91da8-107">If you haven't installed the EWS Managed API already, be sure to [download the API](http://aka.ms/ews-managed-api-readme).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="91da8-108">A API gerenciada de EWS agora está disponível como um projeto de código aberto no [GitHub](https://github.com/officedev/ews-managed-api).</span><span class="sxs-lookup"><span data-stu-id="91da8-108">The EWS Managed API is now available as an open source project on [GitHub](https://github.com/officedev/ews-managed-api).</span></span> <span data-ttu-id="91da8-109">Você pode usar a biblioteca de fonte aberta: > correções e melhorias para a API de colaboração.</span><span class="sxs-lookup"><span data-stu-id="91da8-109">You can use the open source library to: >  Contribute bug fixes and enhancements to the API.</span></span> <span data-ttu-id="91da8-110">> Obtenha correções e aprimoramentos antes que estejam disponíveis em um lançamento oficial.</span><span class="sxs-lookup"><span data-stu-id="91da8-110">>  Get fixes and enhancements before they are available in an official release.</span></span> <span data-ttu-id="91da8-111">> Acesso a implementação mais abrangente e atualizado da API, para usar como uma referência ou para criar novas bibliotecas em plataformas novas.</span><span class="sxs-lookup"><span data-stu-id="91da8-111">>  Access the most comprehensive and up-to-date implementation of the API, to use as a reference or to create new libraries on new platforms.</span></span> <span data-ttu-id="91da8-112">> Bem-vindos suas [contribuições](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span><span class="sxs-lookup"><span data-stu-id="91da8-112">>  We welcome your [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span></span> 
  
## <a name="referencing-the-assembly"></a><span data-ttu-id="91da8-113">Fazendo referência o assembly</span><span class="sxs-lookup"><span data-stu-id="91da8-113">Referencing the assembly</span></span>

<span data-ttu-id="91da8-114">A maneira mais comum para adicionar uma referência é usar o Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="91da8-114">The most common way to add a reference is to use Visual Studio.</span></span> <span data-ttu-id="91da8-115">Nós sabemos que alguns desenvolvedores por aí gostam de usar outros editores, portanto incluímos instruções sobre como usar o compilador de linha de comando, assim como as instruções para usar o Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="91da8-115">We know that some developers out there like to use other editors, so we are including instructions for using the command-line compiler as well as instructions for using Visual Studio.</span></span> <span data-ttu-id="91da8-116">Você pode observar que os exemplos de código que seguem tenham as mesmas instruções de **uso** .</span><span class="sxs-lookup"><span data-stu-id="91da8-116">You might notice that the code examples that follow have the same **using** statements.</span></span> <span data-ttu-id="91da8-117">A diferença entre os dois métodos é que o compilador de linha de comando precisa do local do arquivo de assembly.</span><span class="sxs-lookup"><span data-stu-id="91da8-117">The difference between the two methods is that the command-line compiler needs the location of the assembly file.</span></span> <span data-ttu-id="91da8-118">Referência do Visual Studio trata isso para você em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="91da8-118">The Visual Studio reference handles this for you behind the scenes.</span></span> 
  
### <a name="to-add-a-reference-by-using-visual-studio"></a><span data-ttu-id="91da8-119">Para adicionar uma referência usando o Visual Studio</span><span class="sxs-lookup"><span data-stu-id="91da8-119">To add a reference by using Visual Studio</span></span>

1. <span data-ttu-id="91da8-120">Coloca o arquivo Microsoft.Exchange.WebServices.dll e o arquivo de Microsoft.Exchange.WebServices.xml em uma pasta de sua escolha.</span><span class="sxs-lookup"><span data-stu-id="91da8-120">Put the Microsoft.Exchange.WebServices.dll file and the Microsoft.Exchange.WebServices.xml file into a folder of your choice.</span></span> <span data-ttu-id="91da8-121">Por padrão, os arquivos são instalados no `C:\Program Files\Microsoft\Exchange\Web Services\2.0\`, mas você pode armazenar os arquivos em qualquer lugar em seu computador.</span><span class="sxs-lookup"><span data-stu-id="91da8-121">By default, the files are installed in  `C:\Program Files\Microsoft\Exchange\Web Services\2.0\`, but you can store the files anywhere on your computer.</span></span>
    
2. <span data-ttu-id="91da8-122">No painel Gerenciador de soluções no Visual Studio, selecione **referências**e escolha **Adicionar referência**.</span><span class="sxs-lookup"><span data-stu-id="91da8-122">In the Solution Explorer pane in Visual Studio, select **References**, and then choose **Add Reference**.</span></span> <span data-ttu-id="91da8-123">Isso abre a janela de adicionar referência.</span><span class="sxs-lookup"><span data-stu-id="91da8-123">This opens the Add Reference window.</span></span>
    
3. <span data-ttu-id="91da8-124">Na janela Adicionar referência, navegue até a guia **Procurar** , navegue até o local do arquivo Microsoft.Exchange.WebServices.dll, selecione esse arquivo e selecione **Okey**.</span><span class="sxs-lookup"><span data-stu-id="91da8-124">In the Add Reference window, navigate to the **Browse** tab, browse to the location of the Microsoft.Exchange.WebServices.dll file, select that file, and then select **OK**.</span></span> 
    
4. <span data-ttu-id="91da8-125">Para usar a API gerenciada de EWS em seu aplicativo, adicione uma declaração **using** para o namespace **Microsoft.Exchange.WebServices.Data** .</span><span class="sxs-lookup"><span data-stu-id="91da8-125">To use the EWS Managed API in your application, add a **using** statement for the **Microsoft.Exchange.WebServices.Data** namespace.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

### <a name="to-add-a-reference-and-build-your-application-with-the-command-line-compiler"></a><span data-ttu-id="91da8-126">Para adicionar uma referência e criar o seu aplicativo com o compilador de linha de comando</span><span class="sxs-lookup"><span data-stu-id="91da8-126">To add a reference and build your application with the command-line compiler</span></span>

1. <span data-ttu-id="91da8-127">Coloque o arquivo de Microsoft.Exchange.WebServices.dll em uma pasta de sua escolha.</span><span class="sxs-lookup"><span data-stu-id="91da8-127">Put the Microsoft.Exchange.WebServices.dll file into a folder of your choice.</span></span> <span data-ttu-id="91da8-128">Essa pasta será a pasta de saída para o compilador.</span><span class="sxs-lookup"><span data-stu-id="91da8-128">This folder will be the output folder for the compiler.</span></span>
    
2. <span data-ttu-id="91da8-129">No seu editor de código fonte, adicione uma instrução **usando** o código-fonte para o namespace **Microsoft.Exchange.WebServices.Data** .</span><span class="sxs-lookup"><span data-stu-id="91da8-129">In your source code editor, add a **using** statement to the source code for the **Microsoft.Exchange.WebServices.Data** namespace.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

3. <span data-ttu-id="91da8-130">Execute o compilador de linha de comando para criar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="91da8-130">Run the command-line compiler to build the application.</span></span> <span data-ttu-id="91da8-131">O comando a seguir usa o .NET Framework compilador c# para criar o aplicativo do Windows definido no arquivo de código fonte "Module. vb".</span><span class="sxs-lookup"><span data-stu-id="91da8-131">The following command uses the .NET Framework C# compiler to build the Windows application defined in the source code file "program.cs".</span></span> <span data-ttu-id="91da8-132">Ele pressupõe que o compilador está localizado no diretório de instalação padrão e que o arquivo de Microsoft.Exchange.WebServices.dll está em um subdiretório do diretório atual chamado "build".</span><span class="sxs-lookup"><span data-stu-id="91da8-132">It assumes that the compiler is located in the default installation directory and that the Microsoft.Exchange.WebServices.dll file is in a subdirectory of the current directory named "build".</span></span>
    
   ```cs
    c:\Windows\Microsoft.NET\Framework\3.5\csc /target: winexe /out: build\testApplication /reference: build\Microsoft.Exchange.WebServices.dll program.cs
   ```

## <a name="see-also"></a><span data-ttu-id="91da8-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="91da8-133">See also</span></span>

- [<span data-ttu-id="91da8-134">Introdução aos aplicativos de cliente API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="91da8-134">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)    
- [<span data-ttu-id="91da8-135">Configurando o ambiente de desenvolvimento de aplicativos do Exchange</span><span class="sxs-lookup"><span data-stu-id="91da8-135">Setting up your Exchange application development environment</span></span>](setting-up-your-exchange-application-development-environment.md)   
- [<span data-ttu-id="91da8-136">Comunicar-se com o EWS usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="91da8-136">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

