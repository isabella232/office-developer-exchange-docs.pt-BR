---
title: Introdução aos aplicativos clientes de API gerenciada por EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c2267733-6f4f-49e5-9614-1e4a24c3af1a
description: Desenvolva um aplicativo de cliente de email Hello World simple do Exchange usando a API gerenciada de EWS.
ms.openlocfilehash: dafc8cbbf172ad725ab83c93553464ba96ef33b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750678"
---
# <a name="get-started-with-ews-managed-api-client-applications"></a>Introdução aos aplicativos clientes de API gerenciada por EWS

Desenvolva um aplicativo de cliente de email Hello World simple do Exchange usando a API gerenciada de EWS. 
  
A [API gerenciada de EWS](http://aka.ms/ews-managed-api-readme) fornece um modelo de objeto intuitivo e fácil de usar para envio e recebimento de mensagens do serviço web de aplicativos clientes, aplicativos de portal e aplicativos de serviço. Você pode acessar quase todas as informações armazenadas em um Exchange Online, Exchange Online como parte do Office 365 ou uma caixa de correio do Exchange server usando a API gerenciada de EWS. Você pode usar as informações neste artigo para ajudá-lo a desenvolver seu primeiro aplicativo cliente EWS Managed API. 
  
> [!NOTE]
> A API gerenciada de EWS agora está disponível como um projeto de código aberto no [GitHub](https://github.com/officedev/ews-managed-api). Você pode usar a biblioteca de fonte aberta: > correções e melhorias para a API de colaboração. > Obtenha correções e aprimoramentos antes que estejam disponíveis em um lançamento oficial. > Acesso a implementação mais abrangente e atualizado da API, para usar como uma referência ou para criar novas bibliotecas em plataformas novas. > Bem-vindos suas [contribuições](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub. 
  
## <a name="youll-need-an-exchange-server"></a>Você precisará de um servidor do Exchange
<a name="NeedExchange"> </a>

Se você já tiver uma conta de caixa de correio do Exchange, você poderá ignorar esta seção. Caso contrário, você tem as seguintes opções para configurar uma caixa de correio do Exchange para seu primeiro aplicativo cliente EWS:
  
- Obtenha um [Site do desenvolvedor do Office 365](http://msdn.microsoft.com/en-us/library/office/fp179924.aspx) (recomendado). Esta é a maneira mais rápida para configurar uma caixa de correio do Exchange. 
    
- Baixe o [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).
    
Após ter verificado que você pode enviar e receber emails do Exchange, você estará pronto para configurar o ambiente de desenvolvimento. Você pode usar o cliente do Exchange web do [Outlook Web App](http://technet.microsoft.com/en-us/library/jj657718%28v=exchg.150%29.aspx) para verificar se você pode enviar o email. 
  
## <a name="set-up-your-development-environment"></a>Definir seu ambiente de desenvolvimento
<a name="Setup"> </a>

Certifique-se de que você tenha acesso ao seguinte:
  
- Qualquer versão do [Visual Studio](http://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx) que suporta o .NET Framework 4. Embora tecnicamente, Visual Studio não é necessário porque você pode usar qualquer compilador c#, recomendamos que você usá-lo. 
    
- A [API gerenciada de EWS](http://aka.ms/ews-managed-api-readme). Você pode usar tanto a versão de 32 bits ou 64 bits, dependendo do seu sistema. Use o local de instalação padrão. 
    
## <a name="create-your-first-ews-managed-api-application"></a>Crie seu primeiro aplicativo de API gerenciada de EWS
<a name="Create"> </a>

Essas etapas pressupõem que você configure um Site do desenvolvedor do Office 365. Se você baixar e instalar o Exchange, você precisará [instalar um certificado válido](http://technet.microsoft.com/en-us/library/bb310769%28v=exchg.141%29.aspx) no seu Exchange server ou a [implementação de uma validação de certificado](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) retorno de chamada para um certificado autoassinado é fornecido por padrão. Observe também que estas etapas podem variar ligeiramente dependendo da versão do Visual Studio que você está usando. 
  
### <a name="step-1-create-a-project-in-visual-studio"></a>Etapa 1: Criar um projeto no Visual Studio

1. No Visual Studio, no menu **arquivo** , escolha **novo**e, em seguida, selecione o **projeto**. Abre a caixa de diálogo **Novo projeto**. 
    
2. Crie um **aplicativo de Console do c#**. No painel **modelos** , escolha **Visual c#** e, em seguida, escolha o **Aplicativo de Console**. 
    
3. Nome do projeto HelloWorld e escolha **Okey**.
    
Visual Studio cria o projeto e abre a janela de documento de código Module. vb.

### <a name="step-2-add-a-reference-to-the-ews-managed-api"></a>Etapa 2: Adicionar uma referência para a API gerenciada de EWS

1. Se a janela **Explorador** de soluções já estiver aberta, ignore esta etapa e vá para a etapa 2. Para abrir a janela **Solution Explorer** , no menu **Exibir** , escolha **Solution Explorer**. 
    
2. No **Solution Explorer** e o projeto **HelloWorld** , abra o menu de atalho (botão direito do mouse) para **referências** e escolha **Adicionar referência** no menu de contexto. Uma caixa de diálogo de gerenciamento de referências de projeto será aberta. 
    
3. Escolha a opção **Procurar** . Navegue até o local onde você instalou a DLL de API gerenciada do EWS. O caminho padrão definido pelo instalador é o seguinte: C:\Program Files\Microsoft\Exchange\Web serviços\<versão >\. O caminho pode variar com base em se você baixe o 32 ou a versão de 64 bits do Microsoft.Exchange.WebServices.dll. Escolha **Microsoft.Exchange.WebServices.dll** e selecione **Okey** ou **Adicionar**. Isso adiciona a referência de API gerenciada de EWS ao seu projeto. 
    
4. Se você estiver usando o EWS gerenciadas API 2.0, altere o projeto HelloWorld para direcionar o .NET Framework 4. Outras versões do EWS Managed API podem usar uma versão de destino diferente do .NET Framework.
    
5. Confirme que você está usando a versão de destino correto do .NET Framework. Abra o menu de atalho (botão direito do mouse) para o seu projeto **HelloWorld** no **Solution Explorer**e escolha **Propriedades**. Verifique se o **.NET Framework 4** é selecionado na caixa de lista suspensa de **estrutura de destino** . 
    
Agora que você ter seu projeto configurado e você criou uma referência para a API gerenciada de EWS, você estará pronto para criar seu primeiro aplicativo. Para manter a simplicidade, adicione o código no arquivo Module. vb. Leia [o assembly do EWS Managed API de referência](how-to-reference-the-ews-managed-api-assembly.md) para obter mais informações sobre como fazer referência a API gerenciada de EWS. Na próxima etapa, você irá desenvolver o código básico para gravar o cliente de API gerenciada de EWS a maioria dos aplicativos. 
### <a name="step-3-set-up-url-redirection-validation-for-autodiscover"></a>Etapa 3: Configurar a validação de redirecionamento de URL de descoberta automática

- Adicione o seguinte método de retorno de chamada de validação de redirecionamento após o método **Main (string [] args)** . Isso valida se redirecionado URLs retornado pela [descoberta automática](autodiscover-for-exchange.md) representam um ponto de extremidade HTTPS. 
    
  ```cs
  private static bool RedirectionUrlValidationCallback(string redirectionUrl)
  {
     // The default for the validation callback is to reject the URL.
     bool result = false;
     Uri redirectionUri = new Uri(redirectionUrl);
     // Validate the contents of the redirection URL. In this simple validation
     // callback, the redirection URL is considered valid if it is using HTTPS
     // to encrypt the authentication credentials. 
     if (redirectionUri.Scheme == "https")
     {
        result = true;
     }
     return result;
  }
  ```

Esse retorno de chamada de validação será passado para o objeto **ExchangeService** na etapa 4. Você precisa para que seu aplicativo será confiar e seguir redirecionamentos de descoberta automática - os resultados do redirecionamento de descoberta automática fornece o ponto de extremidade do EWS para nosso aplicativo. 

### <a name="step-4-prepare-the-exchangeservice-object"></a>Etapa 4: Preparar o objeto ExchangeService

1. Adicione uma referência de diretiva **usando** para a API gerenciada de EWS. Adicione o código a seguir após a última diretiva **using** na parte superior da Module. vb. 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

2. No método **Main** , instanciar o objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) com a versão do serviço que você pretende de destino. Este exemplo refere-se a versão mais antiga do esquema do EWS. 
    
   ```cs
    ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);
   ```

3. Se você está direcionando um servidor do Exchange no local e seu cliente está unido ao domínio, vá para a etapa 4. Se você cliente concentrando-se uma caixa de correio do Site do desenvolvedor do Office 365 ou Exchange Online, você precisa passar credenciais explícitas. Adicione o código a seguir após a instanciação do objeto **ExchangeService** e definir as credenciais para a sua conta de caixa de correio. O nome de usuário deve ser o nome principal do usuário. Vá para a etapa 5. 
    
   ```cs
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

4. Clientes do domínio que um servidor do Exchange no local de destino podem usar as credenciais padrão do usuário que está conectado, supondo que as credenciais estão associadas uma caixa de correio. Adicione o código a seguir após a instanciação do objeto **ExchangeService** . 
    
   ```cs
    service.UseDefaultCredentials = true;
   ```

   Se seu cliente destinada a uma caixa de correio do Exchange Online ou o Site do desenvolvedor do Office 365, verifique se que [UseDefaultCredentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.usedefaultcredentials%28v=exchg.80%29.aspx) está definido como **false**, que é o valor padrão. Seu cliente está pronto para fazer a chamada primeira para o serviço Descoberta automática para obter a URL do serviço de chamadas para o serviço do EWS.
    
5. O método **AutodiscoverUrl** no objeto **ExchangeService** realiza uma série de chamadas para o serviço de descoberta automática para obter a URL do serviço. Se essa chamada de método tiver êxito, a propriedade URL no objeto **ExchangeService** será definida com a URL do serviço. Passe o endereço de email do usuário e o **RedirectionUrlValidationCallback** para o método **AutodiscoverUrl** . Depois que as credenciais tiverem sido especificadas na etapa 3 ou 4, adicione o código a seguir. Alterar `user1@contoso.com` para seu email para que o serviço Descoberta automática encontra seu ponto de extremidade do EWS de endereços. 
    
   ```cs
    service.AutodiscoverUrl("user1@contoso.com", RedirectionUrlValidationCallback);
   ```

Neste ponto, seu cliente estiver configurado para fazer chamadas para o EWS para acessar dados de caixa de correio. Se você executar o seu código agora, você pode verificar se a chamada do método **AutodiscoverUrl** funcionou examinando o conteúdo da propriedade [ExchangeService.Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) . Se essa propriedade contém uma URL, sua chamada foi um sucesso! Isso significa que seu aplicativo com êxito autenticado com o serviço e descoberto o ponto de extremidade do EWS para sua caixa de correio. Agora você está pronto para fazer primeira suas chamadas EWS. Leia a [definir a URL do serviço do EWS usando a API gerenciada de EWS](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md) para obter mais informações sobre como definir a URL do EWS. 

### <a name="step-6-create-your-first-hello-world-email-message"></a>Etapa 6: Criar sua primeira mensagem de email Olá mundo

1. Após chamar o método **AutodiscoverUrl** , instanciar um novo objeto **EmailMessage** e passe o objeto de serviço que você criou. 
    
   ```cs
    EmailMessage email = new EmailMessage(service);
   ```

   Agora você tem uma mensagem de email no qual a ligação do serviço é definida. Todas as chamadas iniciadas no objeto **EmailMessage** serão direcionadas no serviço. 
    
2. Agora definida para: destinatário de linha da mensagem de email. Para fazer isso, altere `user1@contoso.com` usar seu endereço SMTP. 
    
   ```cs
    email.ToRecipients.Add("user1@contoso.com");
   ```

3. Defina o assunto e o corpo da mensagem de email.
    
   ```cs
    email.Subject = "HelloWorld";
    email.Body = new MessageBody("This is the first email I've sent by using the EWS Managed API.");
   ```

4. Agora você está pronto para enviar sua primeira mensagem de email usando a API gerenciada de EWS. O método **Send** irá chamar o serviço e enviar a mensagem de email para entrega. Leia [Communicate with EWS usando a API gerenciada de EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md) para conhecer outros métodos que você pode usar para se comunicar com o Exchange. 
    
   ```cs
    email.Send();
   ```

5. Você está pronto para executar seu aplicativo Hello World. No Visual Studio, selecione **F5**. Será aberta uma janela de console em branco. Você não verá algo na janela do console enquanto o seu aplicativo autentica, segue redirecionamentos de descoberta automática e então faz sua chamada primeira para criar uma mensagem de email que você envie para você mesmo. Se você quiser ver as chamadas sejam feitas, adicione as duas linhas de código a seguintes antes do método **AutodiscoverUrl** é chamado. Em seguida, pressione F5. Isso irá [Rastrear check-out do EWS solicitações e respostas](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) na janela do console. 
    
   ```cs
    service.TraceEnabled = true;
    service.TraceFlags = TraceFlags.All;
   ```

Agora você tem um aplicativo de cliente do EWS Managed API em funcionamento. Para sua conveniência, o exemplo a seguir mostra o código que você adicionou à Module. vb para criar seu aplicativo Hello World.

```cs
using System;
using Microsoft.Exchange.WebServices.Data;
namespace HelloWorld
{
  class Program
  {
    static void Main(string[] args)
    {
      ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);
      service.Credentials = new WebCredentials("user1@contoso.com", "password");
      service.TraceEnabled = true;
      service.TraceFlags = TraceFlags.All;
      service.AutodiscoverUrl("user1@contoso.com", RedirectionUrlValidationCallback);
      EmailMessage email = new EmailMessage(service);
      email.ToRecipients.Add("user1@contoso.com");
      email.Subject = "HelloWorld";
      email.Body = new MessageBody("This is the first email I've sent by using the EWS Managed API");
      email.Send();
    }
    private static bool RedirectionUrlValidationCallback(string redirectionUrl)
    {
      // The default for the validation callback is to reject the URL.
      bool result = false;
      Uri redirectionUri = new Uri(redirectionUrl);
      // Validate the contents of the redirection URL. In this simple validation
      // callback, the redirection URL is considered valid if it is using HTTPS
      // to encrypt the authentication credentials. 
      if (redirectionUri.Scheme == "https")
      {
        result = true;
      }
      return result;
    }
  }
}
```

## <a name="next-steps"></a>Próximas etapas
<a name="Next"> </a>

Se você estiver pronto para fazer mais com seu primeiro aplicativo de cliente do EWS Managed API, explore os recursos a seguir:
  
- [Exchange 2013:101 amostras de código](http://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c)
    
- [Pastas e itens](folders-and-items-in-ews-in-exchange.md)
    
- [EWSEditor](http://ewseditor.codeplex.com/)
    
Se você tiver algum problema com o seu aplicativo, [Experimente postar uma pergunta ou um comentário no fórum](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (e não se esqueça de ler a postagem superior). 
  
## <a name="in-this-section"></a>Nesta seção
<a name="Next"> </a>

- [Faça referência ao conjunto de API gerenciada de EWS](how-to-reference-the-ews-managed-api-assembly.md)
    
- [Definir a URL de serviço do EWS usando a API gerenciada de EWS](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md)
    
- [Comunicar-se com o EWS usando a API gerenciada de EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    
## <a name="see-also"></a>Confira também

- [Start using web services in Exchange](start-using-web-services-in-exchange.md)    
- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md)    
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)   
- [Solicitações e respostas para solucionar problemas de aplicativos do EWS Managed API de rastreamento](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    

