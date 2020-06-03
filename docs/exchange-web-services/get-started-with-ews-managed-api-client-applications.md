---
title: Introdução aos aplicativos clientes de API gerenciada por EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: c2267733-6f4f-49e5-9614-1e4a24c3af1a
description: Desenvolva um aplicativo de cliente de email Hello World simples para o Exchange usando a API gerenciada do EWS.
localization_priority: Priority
ms.openlocfilehash: 45c1f1c794fc505d1dc3d059d5bde106dc37009f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455391"
---
# <a name="get-started-with-ews-managed-api-client-applications"></a>Introdução aos aplicativos clientes de API gerenciada por EWS

Desenvolva um aplicativo de cliente de email Hello World simples para o Exchange usando a API gerenciada do EWS. 
  
A [API gerenciada do EWS](https://aka.ms/ews-managed-api-readme) fornece um modelo de objeto intuitivo e fácil de usar para enviar e receber mensagens de serviço da Web de aplicativos cliente, aplicativos de portal e aplicativos de serviço. Você pode acessar quase todas as informações armazenadas em um Exchange Online, Exchange Online como parte do Office 365 ou uma caixa de correio do Exchange Server usando a API gerenciada do EWS. Você pode usar as informações deste artigo para ajudá-lo a desenvolver seu primeiro aplicativo cliente da API gerenciada do EWS. 
  
> [!NOTE]
> A API gerenciada do EWS já está disponível como um projeto de código-fonte aberto no [GitHub](https://github.com/officedev/ews-managed-api). É possível usar a biblioteca de software livre para: 
> - Contribui com correções de bug e melhorias à API. 
> - Obtenha correções e melhorias antes que estejam disponíveis em uma versão oficial. 
> - Acesse a implementação mais abrangente e atualizada da API, para usar como referência ou criar novas bibliotecas em novas plataformas.  
>
>  Agradecemos suas [contribuições](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via github. 
  
## <a name="youll-need-an-exchange-server"></a>Você precisará de um servidor do Exchange
<a name="NeedExchange"> </a>

Se você já tem uma conta de caixa de correio do Exchange, você pode ignorar esta seção. Caso contrário, você tem as seguintes opções para configurar uma caixa de correio do Exchange para seu primeiro aplicativo cliente do EWS:
  
- Obter um [site do desenvolvedor do Office 365](https://msdn.microsoft.com/library/office/fp179924.aspx) (recomendado). Essa é a maneira mais rápida de configurar uma caixa de correio do Exchange. 

- Baixar o [Exchange Server](https://office.microsoft.com/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).

    
Depois de verificar se você pode enviar e receber emails do Exchange, você está pronto para configurar seu ambiente de desenvolvimento. Você pode usar o [Outlook Web App](https://technet.microsoft.com/library/jj657718%28v=exchg.150%29.aspx) do cliente do Exchange para verificar se você pode enviar emails. 
  
## <a name="set-up-your-development-environment"></a>Defina seu ambiente de desenvolvimento
<a name="Setup"> </a>

Certifique-se de que você tem acesso ao seguinte:
  
- Qualquer versão do [Visual Studio](https://www.visualstudio.com/downloads/download-visual-studio-vs.aspx) que suporte o .NET Framework 4. Embora tecnicamente, você não precisa do Visual Studio porque você pode usar qualquer compilador C#, recomendamos que você o use. 
    
- A [API gerenciada do EWS](https://aka.ms/ews-managed-api-readme). Você pode usar a versão de 64 bits ou 32 bits, dependendo do seu sistema. Use o local de instalação padrão. 
    
## <a name="create-your-first-ews-managed-api-application"></a>Criar seu primeiro aplicativo de API gerenciada por EWS
<a name="Create"> </a>

Estas etapas pressupõem que você configure um site do desenvolvedor do Office 365. Se você baixou e instalou o Exchange, será necessário [instalar um certificado válido](https://technet.microsoft.com/library/bb310769%28v=exchg.141%29.aspx) no servidor do Exchange ou [implementar um](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) retorno de chamada de validação de certificado para um certificado autoassinado fornecido por padrão. Observe também que essas etapas podem variar um pouco dependendo da versão do Visual Studio que você está usando. 
  
### <a name="step-1-create-a-project-in-visual-studio"></a>Etapa 1: criar um projeto no Visual Studio

1. No Visual Studio, no menu **arquivo** , escolha **novo**e, em seguida, escolha **projeto**. Abre a caixa de diálogo **Novo projeto**. 
    
2. Criar um **aplicativo de console C#**. No painel **modelos** , escolha **Visual C#** e, em seguida, escolha **aplicativo de console**. 
    
3. Nomeie o projeto como HelloWorld e, em seguida, escolha **OK**.
    
O Visual Studio cria o projeto e abre a janela do documento de código do Program.cs.

### <a name="step-2-add-a-reference-to-the-ews-managed-api"></a>Etapa 2: adicionar uma referência à API gerenciada do EWS

1. Se a janela do **Gerenciador de soluções** já estiver aberta, pule esta etapa e vá para a etapa 2. Para abrir a janela **Gerenciador de soluções** , no menu **Exibir** , escolha **Gerenciador de soluções**. 
    
2. No **Gerenciador de soluções** e no projeto **HelloWorld** , abra o menu de atalho (clique com o botão direito do mouse) para obter **referências** e escolha **Adicionar referência** no menu de contexto. Uma caixa de diálogo para gerenciar referências de projeto será aberta. 
    
3. Escolha a opção **procurar** . Navegue até o local onde você instalou a DLL de API gerenciada do EWS. O caminho padrão definido pelo instalador é o seguinte: C:\Arquivos de Files\Microsoft\Exchange\Web Services\<version>\. O caminho pode variar de acordo com o download da versão de 32 ou 64 bits do Microsoft. Exchange. WebServices. dll. Escolha **Microsoft. Exchange. WebServices. dll** e selecione **OK** ou **Adicionar**. Isso adiciona a referência da API gerenciada do EWS ao seu projeto. 
    
4. Se você estiver usando a API gerenciada do EWS 2,0, altere o projeto HelloWorld para direcionar o .NET Framework 4. Outras versões da API gerenciada do EWS podem usar uma versão de destino diferente do .NET Framework.
    
5. Confirme se você está usando a versão de destino correta do .NET Framework. Abra o menu de atalho (clique com o botão direito do mouse) para seu projeto **HelloWorld** no **Gerenciador de soluções**e escolha **Propriedades**. Verifique se o **.NET Framework 4** está selecionado na caixa suspensa **estrutura de destino** . 
    
Agora que você já configurou o projeto e criou uma referência para a API gerenciada do EWS, você está pronto para criar seu primeiro aplicativo. Para simplificar as coisas, adicione seu código ao arquivo Program.cs. Ler [referência o assembly da API gerenciada do EWS](how-to-reference-the-ews-managed-api-assembly.md) para obter mais informações sobre como fazer referência à API gerenciada do EWS. Na próxima etapa, você desenvolverá o código básico para escrever a maioria dos aplicativos clientes da API gerenciada do EWS. 
### <a name="step-3-set-up-url-redirection-validation-for-autodiscover"></a>Etapa 3: configurar a validação de redirecionamento de URL para descoberta automática

- Adicione o seguinte método de retorno de chamada de validação de redirecionamento após o método **principal (String [] args)** . Isso valida se as URLs redirecionadas retornadas pela [descoberta automática](autodiscover-for-exchange.md) representam um ponto de extremidade HTTPS. 
    
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

Esse retorno de chamada de validação será passado para o objeto **ExchangeService** na etapa 4. Isso é necessário para que seu aplicativo confie e siga os redirecionamentos de descoberta automática-os resultados do redirecionamento de descoberta automática fornecem o ponto de extremidade do EWS para nosso aplicativo. 

### <a name="step-4-prepare-the-exchangeservice-object"></a>Etapa 4: preparar o objeto ExchangeService

1. Adicione uma referência de diretiva **using** à API gerenciada do EWS. Adicione o seguinte código após a última diretiva **using** na parte superior de Program.cs. 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

2. No método **Main** , instancie o objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) com a versão de serviço que você pretende direcionar. Este exemplo direciona a versão anterior do esquema do EWS. 
    
   ```cs
    ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);
   ```

3. Se você estiver direcionando um servidor Exchange local e seu cliente estiver associado ao domínio, prossiga para a etapa 4. Se o cliente estiver direcionado para uma caixa de correio de site do desenvolvedor do Exchange Online ou do Office 365, você precisará transmitir credenciais explícitas. Adicione o seguinte código após a instanciação do objeto **ExchangeService** e defina as credenciais da sua conta de caixa de correio. O nome de usuário deve ser o nome principal do usuário. Vá para a etapa 5. 
    
   ```cs
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

4. Clientes associados ao domínio que se destinam a um servidor Exchange local podem usar as credenciais padrão do usuário conectado, supondo que as credenciais estejam associadas a uma caixa de correio. Adicione o seguinte código após a instanciação do objeto **ExchangeService** . 
    
   ```cs
    service.UseDefaultCredentials = true;
   ```

   Se o cliente tiver como destino uma caixa de correio de site do desenvolvedor do Exchange Online ou do Office 365, verifique se [UseDefaultCredentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.usedefaultcredentials%28v=exchg.80%29.aspx) está definido como **false**, que é o valor padrão. O cliente está pronto para fazer a primeira chamada para o serviço de descoberta automática para obter a URL do serviço para chamadas para o serviço do EWS.
    
5. O método **AutodiscoverUrl** no objeto **ExchangeService** executa uma série de chamadas para o serviço de descoberta automática para obter a URL do serviço. Se essa chamada de método for bem-sucedida, a propriedade URL no objeto **ExchangeService** será definida com a URL do serviço. Passe o endereço de email do usuário e o **RedirectionUrlValidationCallback** para o método **AutodiscoverUrl** . Adicione o seguinte código após as credenciais terem sido especificadas na etapa 3 ou 4. Mude `user1@contoso.com` para o seu endereço de email para que o serviço de descoberta automática encontre o ponto de extremidade do EWS. 
    
   ```cs
    service.AutodiscoverUrl("user1@contoso.com", RedirectionUrlValidationCallback);
   ```

Neste ponto, o cliente está configurado para fazer chamadas ao EWS para acessar os dados da caixa de correio. Se você executar o código agora, você pode verificar se a chamada do método **AutodiscoverUrl** funcionou, examinando o conteúdo da propriedade [ExchangeService. URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) . Se essa propriedade contiver uma URL, sua chamada foi bem-sucedida! Isso significa que seu aplicativo foi autenticado com êxito com o serviço e descobriu o ponto de extremidade do EWS para sua caixa de correio. Agora você está pronto para fazer suas primeiras chamadas para o EWS. Leitura [defina a URL do serviço EWS usando a API gerenciada do EWS](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md) para obter mais informações sobre a configuração da URL do EWS. 

### <a name="step-6-create-your-first-hello-world-email-message"></a>Etapa 6: criar sua primeira mensagem de email Hello World

1. Após a chamada do método **AutodiscoverUrl** , crie uma instância de um novo objeto **EmailMessage** e passe o objeto de serviço que você criou. 
    
   ```cs
    EmailMessage email = new EmailMessage(service);
   ```

   Agora você tem uma mensagem de email na qual a associação de serviço está definida. Todas as chamadas iniciadas no objeto **EmailMessage** serão direcionadas para o serviço. 
    
2. Agora defina o destinatário para: linha da mensagem de email. Para fazer isso, altere `user1@contoso.com` para usar seu endereço SMTP. 
    
   ```cs
    email.ToRecipients.Add("user1@contoso.com");
   ```

3. Defina o assunto e o corpo da mensagem de email.
    
   ```cs
    email.Subject = "HelloWorld";
    email.Body = new MessageBody("This is the first email I've sent by using the EWS Managed API.");
   ```

4. Agora você está pronto para enviar sua primeira mensagem de email usando a API gerenciada do EWS. O método **Send** chamará o serviço e enviará a mensagem de email para entrega. Leia [se comunicar com o EWS usando a API gerenciada do EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md) para saber mais sobre outros métodos que você pode usar para se comunicar com o Exchange. 
    
   ```cs
    email.Send();
   ```

5. Você está pronto para executar seu aplicativo Hello World. No Visual Studio, selecione **F5**. Uma janela de console em branco será aberta. Você não verá nada na janela do console enquanto o aplicativo é autenticado, segue redirecionamentos de descoberta automática e, em seguida, faz sua primeira chamada criar uma mensagem de email que você envia para si mesmo. Se você quiser ver as chamadas que estão sendo feitas, adicione as duas linhas de código a seguir antes do método **AutodiscoverUrl** ser chamado. Pressione F5. Isso [rastreará as solicitações e respostas do EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) para a janela do console. 
    
   ```cs
    service.TraceEnabled = true;
    service.TraceFlags = TraceFlags.All;
   ```

Agora você tem um aplicativo cliente da API gerenciada do EWS em funcionamento. Para sua conveniência, o exemplo a seguir mostra todo o código adicionado ao Program.cs para criar seu aplicativo Hello World.

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

Se você estiver pronto para fazer mais com seu primeiro aplicativo cliente da API gerenciada pelo EWS, explore os seguintes recursos:
  
- [Exchange 2013:101 amostras de código](https://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c)   
- [Pastas e itens](folders-and-items-in-ews-in-exchange.md)    
- [EWSEditor](http://ewseditor.codeplex.com/)
    
Se você tiver problemas com o aplicativo, [tente postar uma dúvida ou comentário no fórum](https://social.technet.microsoft.com/Forums/exchange/home?forum=exchangesvrdevelopment) (e não se esqueça de ler a postagem superior). 
  
## <a name="in-this-section"></a>Nesta seção
<a name="Next"> </a>

- [Fazer referência ao assembly da API gerenciada do EWS](how-to-reference-the-ews-managed-api-assembly.md)   
- [Definir a URL do serviço EWS usando a API gerenciada do EWS](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md)   
- [Comunicar-se com o EWS usando a API gerenciada do EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    
## <a name="see-also"></a>Confira também

- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)    
- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)    
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)   
- [Rastrear solicitações e respostas para solucionar problemas de aplicativos de API gerenciada do EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    

