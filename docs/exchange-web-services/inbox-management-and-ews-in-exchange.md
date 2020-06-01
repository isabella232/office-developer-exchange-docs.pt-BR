---
title: Gerenciamento de caixa de entrada e EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3dfa0fc9-64bb-4d18-bff7-bf6b3bed4a0d
description: Descubra como você pode gerenciar sua caixa de entrada na API gerenciada do EWS ou no aplicativo EWS usando regras de caixa de entrada e a lista de remetentes bloqueados.
ms.openlocfilehash: 7c88015386dc882f14184765e0046a866e8c0e10
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456308"
---
# <a name="inbox-management-and-ews-in-exchange"></a>Gerenciamento de caixa de entrada e EWS no Exchange

Descubra como você pode gerenciar sua caixa de entrada na API gerenciada do EWS ou no aplicativo EWS usando regras de caixa de entrada e a lista de remetentes bloqueados.
  
As caixas de correio do Exchange vêm equipadas com recursos para ajudar os usuários a organizar seus emails de entrada automaticamente. Todos esses recursos operam no servidor sem a intervenção do usuário, mas atendem a necessidades diferentes. A API gerenciada do EWS e o EWS fornecem acesso a esses recursos, permitindo que os usuários gerenciem suas caixas de entrada.
  
**Tabela 1. Recursos de gerenciamento de caixa de entrada**

|**Se você quiser...**|**Use...**|
|:-----|:-----|
|Executar uma ação em mensagens de entrada (como movê-las para outra pasta ou excluí-las) com base em critérios específicos (como remetente, assunto ou anexos)  <br/> |Regras da Caixa de Entrada  <br/> |
|Excluir todos os emails de entrada de um remetente específico  <br/> |Lista de Remetentes Bloqueados  <br/> |
   
## <a name="inbox-rules"></a>Regras da Caixa de Entrada
<a name="bk_InboxRules"> </a>

Vamos encarar: nem todas as mensagens de email são criadas iguais. Para todos os emails que um usuário recebe do seu gerente, há uma lista de distribuição de vídeo de gato da Internet que ingressou em anos atrás e nunca se encontrava. Embora os vídeos de gato da Internet sejam divertidos, a quantidade de tráfego que a lista de distribuição Obtém pode ser desligada e as mensagens importantes podem ser perdidas facilmente no mar de email da lista de distribuição em uma caixa de entrada. Muitos usuários desativam as regras de caixa de entrada para ajudá-lo a reduzir essas mensagens e tornar a caixa de entrada um ponto muito mais interessante. Com os serviços Web do Exchange (EWS), seu aplicativo pode trazer o poder das regras para o urso.
  
A API gerenciada do EWS fornece os métodos [ExchangeService. GetInboxRules](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getinboxrules%28v=exchg.80%29.aspx) e [ExchangeService. UpdateInboxRules](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.updateinboxrules%28v=exchg.80%29.aspx) para trabalhar com regras. O EWS fornece as operações [GetInboxRules](https://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx) e [UpdateInboxRules](https://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx) para trabalhar com regras. No entanto, observe que a API gerenciada do EWS e o EWS têm as seguintes limitações ao trabalhar com regras de caixa de entrada: 
  
- O EWS não pode acessar ou criar regras ou regras do "somente cliente" que estão definidas no Outlook para executar "somente neste computador".
    
- Para alterar o conjunto atual de regras usando o EWS, você deve remover o BLOB de regras do Outlook, se ele estiver presente. Isso significa que o uso do EWS para modificar regras exclui qualquer regra que tenha sido desativada anteriormente (desabilitada) usando o Outlook. 
    
### <a name="how-do-rules-work"></a>Como as regras funcionam?
<a name="bk_HowRulesWork"> </a>

O mecanismo de regras atua como um gatekeeper para a caixa de correio de um usuário. Quando uma mensagem chega na caixa de correio do usuário, mas antes de a mensagem aparecer na caixa de entrada, essa mensagem é avaliada em relação a uma lista ordenada de regras. Observe que isso ocorre apenas no momento da chegada e apenas na caixa de entrada. Essas regras são compostas por três partes: [condições](#bk_Conditions), [ações](#bk_Actions)e [exceções](#bk_Exceptions).
  
A partir da regra na parte superior da lista de regras, o mecanismo de regras executa as etapas a seguir até chegar ao fim da lista de regras:
  
1. Verifica a mensagem para determinar se ela atende a todas as condições especificadas na regra.
    
1. Se ele atender a todas as condições, a avaliação continuará com a etapa 2.
    
2. Se ele não atender a todas as condições, o mecanismo de regras carregará a próxima regra na lista de regras e começará na etapa 1.
    
2. Verifica a mensagem para determinar se ela atende a qualquer uma das exceções especificadas na regra.
    
1. Se ele atender a qualquer uma das exceções, o mecanismo de regras carregará a próxima regra na lista de regras e começará na etapa 1.
    
2. Se ele não atender a nenhuma das exceções, a avaliação continuará com a etapa 3.
    
3. Executa as ações especificadas na regra da mensagem.
    
1. Se a ação "parar processamento de mais regras" for especificada, o mecanismo de regras executará todas as outras ações na mensagem e sairá sem avaliar nenhuma regra adicional contra a mensagem.
    
2. Se a ação "parar de processar mais regras" não for especificada, o mecanismo de regras carregará a próxima regra na lista de regras e começará pela etapa 1.
    
A figura a seguir mostra o processo que o mecanismo de regras segue.
  
**Figura 1: visão geral do mecanismo de regras**

![Um diagrama que mostra as etapas usadas pelo mecanismo de regras, começando pela avaliação da regra, determinando em seguida se os critérios da regra são atendidos e, por fim, executando a ação ou movendo para a regra seguinte até ser concluído.](media/Ex15_Rules_EngineOverview.png)
  
### <a name="putting-the-pieces-together---parts-of-a-rule"></a>Colocar as partes juntas de uma regra
<a name="bk_Pieces"> </a>

Uma maneira de visualizar as partes de uma regra é imaginar que você está fornecendo instruções a alguém que está com a tarefa de organizar seus emails de entrada. Você pode dizer a essa pessoa: "quando uma mensagem chega \<insert conditions here\> , faça \<insert actions here\> , a menos que a mensagem \<insert exceptions here\> . Vamos examinar mais detalhadamente cada parte.
  
#### <a name="conditions"></a>Condições
<a name="bk_Conditions"> </a>

As [condições](https://msdn.microsoft.com/library/f049a48c-9585-43f7-8549-0b8cb19a5eea%28Office.15%29.aspx) descrevem quando uma regra deve ser aplicada. Embora você possa omitir as condições de uma regra (resultando em uma regra que se aplica a todas as mensagens recebidas), é muito mais comum que as regras tenham condições que se apliquem a um subconjunto de mensagens de entrada. Alguns exemplos são "quando uma mensagem é de Sadie" ou "quando uma mensagem é enviada para a lista de distribuição" Cat Video amantes "". As regras podem ter várias condições. Quando as regras têm mais de uma condição, todas as condições devem ser atendidas para que o mecanismo de regras execute a ação especificada. 
  
#### <a name="actions"></a>Ações
<a name="bk_Actions"> </a>

As [ações](https://msdn.microsoft.com/library/c5aa96b1-2d8b-422f-8c2f-f118572ab23f%28Office.15%29.aspx) descrevem o que acontece quando uma regra se aplica. Os exemplos são "mover a mensagem para a pasta" gatos "ou" marcar a mensagem com prioridade "baixa" ". As regras podem ter várias ações. Quando você especifica várias ações para uma regra, todas as ações são executadas quando a regra é aplicada. 
  
#### <a name="exceptions"></a>Exceções
<a name="bk_Exceptions"> </a>

As [exceções](https://msdn.microsoft.com/library/7cd63ac2-3441-4ed4-915b-6f90af4b28fc%28Office.15%29.aspx) descrevem quando uma regra não deve se aplicar, mesmo se os critérios especificados nas condições forem atendidos. Os exemplos são "exceto se a mensagem for enviada apenas para mim" ou "exceto se a mensagem for do MOM". Uma regra pode ter várias exceções. Quando as regras têm mais de uma exceção, e qualquer uma das exceções é atendida, a regra não é aplicada. 
  
### <a name="example-herding-those-cats"></a>Exemplo: herding esses gatos
<a name="bk_Example"> </a>

Vamos dar uma olhada em como os usuários podem usar regras para eliminar o tráfego dessa lista de distribuição de vídeo de Internet gato. Vamos supor o seguinte:
  
- Essas mensagens são enviadas para uma lista de distribuição chamada "entusiastas de vídeo de Internet gato".
    
- Os usuários desejam ler essas mensagens eventualmente, elas simplesmente não querem obstruir a caixa de entrada. Eles devem arquivar em uma pasta chamada "gatos".
    
- Seus usuários desejam ler as mensagens enviadas para esta lista de distribuição pela mãe imediatamente, pois o MOM envia os vídeos do Funniest.
    
Isso informa ao mecanismo de regras o seguinte: "quando uma mensagem chega a ser enviada para a lista de distribuição entusiastas de vídeo do Internet gato", mova-a para a pasta ' gatos ', a menos que a mensagem seja da mamãe. " 
  
**Tabela 2. Definição de regra**

|**Parte de regra**|**Valor**|
|:-----|:-----|
|Condições  <br/> |Enviado para a lista de distribuição dos fãs de vídeo de gato da Internet  <br/> |
|Ações  <br/> |Mover a mensagem para a pasta ' gatos '  <br/> E parar de processar mais regras  <br/> |
|Exceções  <br/> |De ' mom '  <br/> |
   
> [!NOTE]
> Observe que "parar de processar mais regras" é uma das ações na regra resultante. Em geral, é uma boa ideia incluir esta ação para evitar confusão sobre quais regras atuam em uma determinada mensagem. No entanto, omitindo essa ação e ordenando adequadamente suas regras, você pode obter processamento mais avançado de seus emails de entrada. Nesse caso, provavelmente é uma aposta segura de que as mensagens de vídeo do gato da Internet não exigem muito na forma de processamento avançado. 
  
Logo após a criação da regra, uma nova mensagem entra. Uma esperança de um colaborador envia uma mensagem para a lista de distribuição. Se Mentally realizar o trabalho do mecanismo de regras, a mensagem atenderá a todas as condições (ela é enviada para "entusiastas de vídeos de gato na Internet") e não atenderá a nenhuma das exceções (ela não é de ' mom '), portanto, a regra será aplicada à pasta ' gatos '.
  
A figura a seguir mostra como a regra é aplicada a uma mensagem de email de entrada.
  
**Figura 2. A mensagem de entrada é processada por uma regra**

![Uma ilustração que mostra uma nova mensagem enviada à lista de distribuição de um colaborador. A mensagem atende a todas as condições e a nenhuma das exceções definidas na regra, e é movida para a pasta Cats.](media/Ex15_Rules_RuleEvaluationSample.png)
  
## <a name="blocking-senders"></a>Bloqueando remetentes
<a name="bk_Blocking"> </a>

Embora você possa criar uma regra que mova todos os emails de um remetente específico para a pasta lixo eletrônico, você também pode fazer isso usando a lista de remetentes bloqueados em suas opções de lixo eletrônico. Como há um limite para quantas regras um usuário pode ter, faz sentido usar a lista de remetentes bloqueados. Você pode [Adicionar ou remover endereços de email específicos da lista de remetentes bloqueados](how-to-add-and-remove-email-addresses-from-blocked-senders-list-by-using-ews.md) usando o método [ExchangeService. MARKASJUNK](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) EWS Managed API ou a operação [MarkAsJunk](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) do EWS. Observe que para que o EWS acesse a lista de remetentes bloqueados, a caixa de correio do usuário deve conter uma mensagem de email do endereço de email que você deseja adicionar ou remover. 
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_InThisSection"> </a>

- [Gerenciar regras de caixa de entrada usando o EWS no Exchange](how-to-manage-inbox-rules-by-using-ews-in-exchange.md)
    
- [Adicionar e remover endereços de email da lista de remetentes bloqueados usando o EWS no Exchange](how-to-add-and-remove-email-addresses-from-blocked-senders-list-by-using-ews.md)
    
## <a name="see-also"></a>Também consulte


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Operação GetInboxRules](https://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx)
    
- [Operação UpdateInboxRules](https://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx)
    
- [Operação MarkAsJunk](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)
    

