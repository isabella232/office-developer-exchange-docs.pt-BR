---
title: Validar um certificado de servidor para a API gerenciada do EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 1fe0b215-8340-4bc8-a6ce-4f591ca9e353
description: Saiba como criar e referenciar um método de retorno de chamada de validação de certificado para que você possa fazer solicitações de API gerenciada por EWS para um servidor Exchange.
localization_priority: Priority
ms.openlocfilehash: 195c51ca71890d6092e4182d23990bb528d37095
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456723"
---
# <a name="validate-a-server-certificate-for-the-ews-managed-api"></a>Validar um certificado de servidor para a API gerenciada do EWS

Saiba como criar e referenciar um método de retorno de chamada de validação de certificado para que você possa fazer solicitações de API gerenciada por EWS para um servidor Exchange.
  
Por padrão, as versões do Exchange a partir do Exchange 2007 SP1 usam certificados X509 autoassinados para autenticar chamadas do EWS. Quando estiver usando a API gerenciada do EWS, você precisará criar um método de retorno de chamada de validação de certificado; caso contrário, as solicitações de API gerenciada do EWS falharão. Se você estiver usando o serviço de descoberta automática, a chamada para o método autodiscover da API gerenciada do EWS falhará com um erro **AutodiscoverLocalException** . Se você estiver usando um proxy de serviço Web gerado pela Web, também poderá ser necessário criar um método de retorno de chamada de validação, dependendo de como o proxy é criado. 
  
## <a name="prerequisites-for-creating-a-validation-callback-method"></a>Pré-requisitos para a criação de um método de retorno de chamada de validação
<a name="bk_prereq"> </a>

Para configurar a validação de um certificado de servidor, verifique se os seguintes itens são verdadeiros: 
  
- O servidor do Exchange está usando um certificado autoassinado para EWS. Se o administrador tiver instalado um certificado válido que rastreia um certificado raiz, não será necessário criar um método de retorno de chamada de validação. 
    
- Você está criando um aplicativo gerenciado que inclui uma referência para os seguintes namespaces .NET Framework necessários: 
    
  - **System.Net**
  - **System .net. Security**  
  - **System. Security. Cryptography. X509Certificates**
    
## <a name="example-callback-method-to-validate-a-server-certificate-for-the-ews-managed-api"></a>Exemplo: método de retorno de chamada para validar um certificado de servidor para a API gerenciada do EWS
<a name="bk_example"> </a>

O exemplo de código a seguir mostra como criar um método de retorno de chamada de validação de certificado X509 para a API gerenciada do EWS. Este método validará um certificado X509 e retornará apenas true quando um dos seguintes critérios for atendido: 
  
- O certificado é válido e rastreia de volta para um certificado raiz válido.    
- O certificado é válido e é auto-assinado pelo servidor que o retornou. 
    
> [!IMPORTANT]
> O método de retorno de chamada de validação de certificado neste exemplo fornece segurança suficiente para o desenvolvimento e teste de aplicativos da API gerenciada do EWS. No entanto, ele pode não fornecer segurança suficiente para seu aplicativo implantado. Você sempre deve certificar-se de que o método de retorno de chamada de validação de certificado usado atenda aos requisitos de segurança da sua organização. 
  
```cs
      private static bool CertificateValidationCallBack(
         object sender,
         System.Security.Cryptography.X509Certificates.X509Certificate certificate,
         System.Security.Cryptography.X509Certificates.X509Chain chain,
         System.Net.Security.SslPolicyErrors sslPolicyErrors)
    {
      // If the certificate is a valid, signed certificate, return true.
      if (sslPolicyErrors == System.Net.Security.SslPolicyErrors.None)
      {
        return true;
      }
      // If there are errors in the certificate chain, look at each error to determine the cause.
      if ((sslPolicyErrors &amp; System.Net.Security.SslPolicyErrors.RemoteCertificateChainErrors) != 0)
      {
        if (chain != null &amp;&amp; chain.ChainStatus != null)
        {
          foreach (System.Security.Cryptography.X509Certificates.X509ChainStatus status in chain.ChainStatus)
          {
            if ((certificate.Subject == certificate.Issuer) &amp;&amp;
               (status.Status == System.Security.Cryptography.X509Certificates.X509ChainStatusFlags.UntrustedRoot))
            {
              // Self-signed certificates with an untrusted root are valid. 
              continue;
            }
            else
            {
              if (status.Status != System.Security.Cryptography.X509Certificates.X509ChainStatusFlags.NoError)
              {
                // If there are any other errors in the certificate chain, the certificate is invalid,
             // so the method returns false.
                return false;
              }
            }
          }
        }
        // When processing reaches this line, the only errors in the certificate chain are 
    // untrusted root errors for self-signed certificates. These certificates are valid
    // for default Exchange server installations, so return true.
        return true;
      }
      else
      {
     // In all other cases, return false.
        return false;
      }
    }

```

Você usa a classe **ServicePointManager** no namespace do .NET **System.net** para conectar um método de retorno de chamada de validação, definindo a propriedade **ServerCertificateValidationCallback** . Você pode usar código semelhante ao exemplo de código a seguir para definir a propriedade **ServerCertificateValidationCallback** . 
  
```cs
ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;

```

## <a name="next-steps"></a>Próximas etapas
<a name="bk_example"> </a>

Depois de criar o método de retorno de chamada de validação para a API gerenciada do EWS, você pode usar o serviço de descoberta automática para obter pontos de conexão e configurações de usuário e domínio de um servidor Exchange. Para saber mais, confira os seguintes artigos:
  
- [Usar a Descoberta Automática para localizar os pontos de conexão](how-to-use-autodiscover-to-find-connection-points.md)
    
- [Obter as configurações de usuário do Exchange usando a Descoberta Automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [Obter as configurações de domínio de um servidor do Exchange](how-to-get-domain-settings-from-an-exchange-server.md)
    
## <a name="see-also"></a>Confira também

- [Configurando o aplicativo EWS](setting-up-your-ews-application.md)  
- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
    

