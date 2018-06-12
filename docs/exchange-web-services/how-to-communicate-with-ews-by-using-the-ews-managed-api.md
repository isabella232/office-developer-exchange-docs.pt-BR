---
title: Comunicar-se com o EWS usando a API gerenciada de EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d1b78293-da02-413a-875c-681e99146af3
description: Encontre informações sobre como usar a API gerenciada de EWS para se comunicar com o EWS no Exchange.
ms.openlocfilehash: 773fcc3f7e95d25effb5a686d4b79ec22610df8c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750705"
---
# <a name="communicate-with-ews-by-using-the-ews-managed-api"></a>Comunicar-se com o EWS usando a API gerenciada de EWS

Encontre informações sobre como usar a API gerenciada de EWS para se comunicar com o EWS no Exchange.
  
A classe [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) na API gerenciada do EWS contém os métodos e propriedades que você usa para definir as credenciais de usuário, identificar o ponto de extremidade do EWS, enviar e receber mensagens SOAP e configurar a ligação para se comunicar com o EWS. Antes de poder usar a API gerenciada de EWS para executar qualquer tarefa, você precisa criar uma instância da classe **ExchangeService** e vinculá-lo a EWS. 
  
Depois de configurar um objeto [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) com credenciais de usuário e o ponto de extremidade do EWS, qualquer objeto de caixa de correio que faz referência ao objeto [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) pode usar os seguintes tipos de método para se comunicar com o EWS: 
  
- Métodos do objeto ExchangeService — todos os métodos no objeto **ExchangeService** que não são herdados do tipo de **objeto** base fazem chamadas para o EWS. 
    
- Métodos de tipo de item de caixa de correio do Exchange e pasta.
    
**Tabela 1. Item de caixa de correio e pasta Digite métodos que se comunicam com o EWS**

|Método|O que ele faz|Operações que ele chama|
|:-----|:-----|:-----|
|[Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.load%28v=exchg.80%29.aspx) <br/> |Obtém as propriedades em um objeto de configuração do item, anexo ou usuário.  <br/> |[Operação GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/><br/> [Operação GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/><br/> [Operação GetUserConfiguration](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |
|[Vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |Preenche um novo item no cliente com informações de um item existente no servidor.  <br/> |[Operação GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|[Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) <br/> |Salva a cópia do item cliente no servidor.  <br/> |[Operação UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/> [Operação UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/><br/>[Operação CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/><br/>[Operação CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|[Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> |Atualiza o servidor com as alterações feitas no cliente.<br/><br/>Para itens e pastas, o método **Update** usa a [operação UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) e a [operação UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx).  <br/> |[Operação UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/>[Operação UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|[Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> |Exclui um item no servidor.<br/><br/>Para itens e pastas, o método **Delete** usa o e a [operação DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx).  <br/> |[Operação DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/><br/> [Operação DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
|[Copiar](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> |Cria uma cópia do item ou pastas no servidor.  <br/> |[Operação CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/><br/> [Operação CopyFolder](http://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx) <br/> |
|[Mover](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> |Move itens ou pastas no servidor.  <br/> |[Operação MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/><br/> [Operação MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
## <a name="to-use-the-ews-managed-api-to-communicate-with-ews"></a>Usar a API gerenciada de EWS para se comunicar com o EWS

1. Criar uma instância da classe **ExchangeService** . 
    
   ```csharp
    ExchangeService service = new ExchangeService();
   ```

   > [!NOTE]
   > Instanciação **ExchangeService** com um construtor vazio criará uma instância que está acoplada a última versão conhecida do Exchange. Como alternativa, é possível direcionar uma versão específica do Exchange, especificando a versão como um parâmetro. `ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);`
  
2. Defina as credenciais do usuário que enviar solicitações para o Exchange server. Se você deseja se conectar ao EWS de um computador que está conectado ao domínio, usando as credenciais do usuário autenticado, defina a propriedade **UseDefaultCredentials** no objeto **ExchangeService** como **true**.
    
   ```cs
    // Connect by using the default credentials of the authenticated user.
    service.UseDefaultCredentials = true;
   ```

   Se não desejar conectar usando as credenciais de usuário padrão, defina a propriedade de **credenciais** no objeto **ExchangeService** para especificar explicitamente as credenciais de um usuário diferente. Se você estiver usando o Exchange Online ou Exchange Online como parte do Office 365, você usará a autenticação básica, com apenas um nome de usuário e uma senha. Um nome de domínio é necessário para a autenticação NTLM. 
    
   ```cs
    // Connect by using the credentials of user1 at contoso.com.
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

   Você também pode especificar as credenciais do usuário usando o nome de domínio do usuário e senha.
    
   ```cs
    // Connect by using the credentials of contoso/user1.
    service.Credentials = new WebCredentials("user1", "password", "contoso");
   ```

   > [!NOTE]
   > Se a propriedade **UseDefaultCredentials** estiver definida como **true**, o valor da propriedade **credenciais** será ignorado. 
  
3. Defina a URL do ponto de extremidade do EWS. Essa URL localiza o arquivo de exchange.asmx no servidor de acesso para cliente.
    
   ```cs
    // Use Autodiscover to set the URL endpoint.
    service.AutodiscoverUrl("user1@contoso.com");
   ```

   > [!NOTE]
   >  Embora você pode definir a propriedade **Url** do **ExchangeService** explicitamente como um valor de atributos, recomendamos que você use o serviço Descoberta automática em vez disso, pelos seguintes motivos: > descoberta automática determina o ponto de extremidade recomendado para um determinado usuário (o ponto de extremidade mais próximo ao servidor de caixa de correio do usuário). > A URL do EWS pode ser alterados se novos servidores de acesso para cliente forem implantados. Neste cenário, usando a [descoberta automática](autodiscover-for-exchange.md) significa que nenhuma alteração de código é necessárias. > Você deve definir a URL explicitamente ou chamada **AutodiscoverUrl**, mas você não deve fazer ambos. 
  
## <a name="see-also"></a>Confira também

- [Introdução aos aplicativos de cliente API gerenciada de EWS](get-started-with-ews-managed-api-client-applications.md) 
- [Usar descoberta automática para encontrar os pontos de conexão](how-to-use-autodiscover-to-find-connection-points.md)   
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    

