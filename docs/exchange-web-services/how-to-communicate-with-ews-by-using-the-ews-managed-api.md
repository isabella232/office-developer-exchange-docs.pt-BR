---
title: Comunicar-se com o EWS usando a API gerenciada do EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: d1b78293-da02-413a-875c-681e99146af3
description: Encontre informações sobre como usar a API gerenciada do EWS para se comunicar com o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: be807f2d936bf79d181476ec8eb12f20fca7950f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528241"
---
# <a name="communicate-with-ews-by-using-the-ews-managed-api"></a>Comunicar-se com o EWS usando a API gerenciada do EWS

Encontre informações sobre como usar a API gerenciada do EWS para se comunicar com o EWS no Exchange.
  
A classe [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) na API gerenciada do EWS contém os métodos e as propriedades que você usa para definir as credenciais do usuário, identificar o ponto de extremidade do EWS, enviar e receber mensagens SOAP e configurar a associação para se comunicar com o EWS. Antes de poder usar a API gerenciada do EWS para executar qualquer tarefa, você precisa criar uma instância da classe **ExchangeService** e associá-la ao EWS. 
  
Depois de configurar um objeto [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) com credenciais de usuário e o ponto de extremidade do EWS, qualquer objeto Mailbox que faz referência ao objeto [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) pode usar os seguintes tipos de método para se comunicar com o EWS: 
  
- Métodos de objeto ExchangeService — todos os métodos no objeto **ExchangeService** que não são herdados do tipo de **objeto** base fazem chamadas para EWS. 
    
- Métodos de tipo de pasta e de caixa de correio do Exchange.
    
**Tabela 1. Item de caixa de correio e métodos de tipo de pasta que se comunicam com o EWS**

|Method|Função|Operações que ele chama|
|:-----|:-----|:-----|
|[Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.load%28v=exchg.80%29.aspx) <br/> |Obtém as propriedades de um objeto de configuração de item, anexo ou usuário.  <br/> |[Operação GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/><br/> [Operação GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/><br/> [Operação GetUserConfiguration](https://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |
|[Associá](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |Preenche um novo item no cliente com informações de um item existente no servidor.  <br/> |[Operação GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|[Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) <br/> |Salva a cópia do item do cliente no servidor.  <br/> |[Operação UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/> [Operação UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/><br/>[Operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/><br/>[Operação CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|[Atualização](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> |Atualiza o servidor com as alterações feitas no cliente.<br/><br/>Para itens e pastas, o método **Update** usa a [operação UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) e a [operação UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx).  <br/> |[Operação UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/>[Operação UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|[Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> |Exclui um item no servidor.<br/><br/>Para itens e pastas, o método **delete** usa o e a [operação DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx).  <br/> |[Operação DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/><br/> [Operação DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
|[Copy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> |Cria uma cópia do item ou das pastas no servidor.  <br/> |[Operação CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/><br/> [Operação CopyFolder](https://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx) <br/> |
|[Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> |Move itens ou pastas no servidor.  <br/> |[Operação MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/><br/> [Operação MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
## <a name="to-use-the-ews-managed-api-to-communicate-with-ews"></a>Para usar a API gerenciada do EWS para se comunicar com o EWS

1. Instanciar a classe **ExchangeService** . 
    
   ```csharp
    ExchangeService service = new ExchangeService();
   ```

   > [!NOTE]
   > Instanciar **ExchangeService** com um construtor vazio criará uma instância que está vinculada à última versão conhecida do Exchange. Como alternativa, você pode direcionar uma versão específica do Exchange especificando a versão como um parâmetro. `ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);`
  
2. Definir as credenciais do usuário que envia solicitações ao servidor Exchange. Se você deseja se conectar ao EWS de um computador que está conectado ao domínio, usando as credenciais do usuário autenticado, defina a propriedade **UseDefaultCredentials** no objeto **ExchangeService** como **true**.
    
   ```cs
    // Connect by using the default credentials of the authenticated user.
    service.UseDefaultCredentials = true;
   ```

   Se você não quiser se conectar usando as credenciais de usuário padrão, defina a propriedade **Credentials** no objeto **ExchangeService** para especificar explicitamente as credenciais de um usuário diferente. Se você estiver usando o Exchange Online ou o Exchange Online como parte do Office 365, você usará a autenticação básica, com apenas um nome de usuário e senha. Um nome de domínio é necessário para a autenticação NTLM. 
    
   ```cs
    // Connect by using the credentials of user1 at contoso.com.
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

   Você também pode especificar as credenciais do usuário usando o nome de domínio e a senha do usuário.
    
   ```cs
    // Connect by using the credentials of contoso/user1.
    service.Credentials = new WebCredentials("user1", "password", "contoso");
   ```

   > [!NOTE]
   > Se a propriedade **UseDefaultCredentials** for definida como **true**, o valor da propriedade **Credentials** será ignorado. 
  
3. Defina a URL do ponto de extremidade do EWS. Essa URL localiza o arquivo Exchange. asmx no servidor de acesso para cliente.
    
   ```cs
    // Use Autodiscover to set the URL endpoint.
    service.AutodiscoverUrl("user1@contoso.com");
   ```

   > [!NOTE]
   >  Embora você possa definir explicitamente a propriedade **URL** do **ExchangeService** como um valor codificado, recomendamos que você use o serviço de descoberta automática, pelos seguintes motivos: > autodiscover determina o melhor ponto de extremidade para um determinado usuário (o ponto de extremidade mais próximo ao servidor de caixa de correio do usuário). > a URL do EWS pode ser alterada se novos servidores de acesso para cliente forem implantados. Neste cenário, o uso da [descoberta automática](autodiscover-for-exchange.md) significa que nenhuma alteração de código é necessária. > você deve definir a URL explicitamente ou chamar **AutodiscoverUrl**, mas não faça ambas. 
  
## <a name="see-also"></a>Confira também

- [Introdução aos aplicativos clientes de API gerenciada por EWS](get-started-with-ews-managed-api-client-applications.md) 
- [Usar a Descoberta Automática para localizar os pontos de conexão](how-to-use-autodiscover-to-find-connection-points.md)   
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    

