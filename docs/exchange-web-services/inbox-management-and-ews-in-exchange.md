---
title: Gerenciamento de caixa de entrada e EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3dfa0fc9-64bb-4d18-bff7-bf6b3bed4a0d
description: Descubra como você pode gerenciar sua caixa de entrada na sua API gerenciada de EWS ou aplicativos do EWS usando regras de caixa de entrada e a lista de remetentes bloqueados.
ms.openlocfilehash: fe06c5ee87e2679506ca7247c5fc2c96912dee86
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750845"
---
# <a name="inbox-management-and-ews-in-exchange"></a>Gerenciamento de caixa de entrada e EWS no Exchange

Descubra como você pode gerenciar sua caixa de entrada na sua API gerenciada de EWS ou aplicativos do EWS usando regras de caixa de entrada e a lista de remetentes bloqueados.
  
Caixas de correio do Exchange vêm equipadas com recursos para ajudar os usuários a organizar seus emails de entrada automaticamente. Todos esses recursos operam no servidor sem intervenção do usuário, mas eles atendem a diferentes necessidades. A API gerenciada de EWS e EWS fornecem acesso a esses recursos, permitindo que os usuários gerenciem suas caixas de entrada.
  
**Tabela 1. Recursos de gerenciamento de caixa de entrada**

|**Se você quiser …**|**Use …**|
|:-----|:-----|
|Ação de Take nas mensagens de entrada (por exemplo, movê-las para outra pasta ou excluí-los) com base em critérios específicos (por exemplo, remetente, o assunto ou anexos)  <br/> |Regras de caixa de entrada  <br/> |
|Excluir todas as mensagens recebidas de um remetente específico  <br/> |Lista de remetentes bloqueados  <br/> |
   
## <a name="inbox-rules"></a>Regras de caixa de entrada
<a name="bk_InboxRules"> </a>

Analisando os fatos: não todas as mensagens de email são criadas iguais. Para cada email que um usuário obtém do seu gerente, há um uma lista de distribuição de vídeo de gato Internet que ele ingressou anos atrás e nunca entendeu ao redor para sair. Vídeos do Internet cat são entretenimento, a quantidade de tráfego que obtém da lista de distribuição pode obter sai do controle e mensagens importantes facilmente pode ser perdida no excesso de email da lista de distribuição em uma caixa de entrada. Muitos usuários ativar às regras de caixa de entrada para ajudar a diminuir a essas mensagens e faça um melhor local para ser de suas caixas de entrada. Com o Exchange Web Services (EWS), seu aplicativo pode trazer o poder de regras de responsabilidade sua.
  
A API gerenciada de EWS fornece os métodos [ExchangeService.GetInboxRules](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getinboxrules%28v=exchg.80%29.aspx) e [ExchangeService.UpdateInboxRules](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.updateinboxrules%28v=exchg.80%29.aspx) para trabalhar com as regras. EWS fornece as operações de [GetInboxRules](http://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx) e [UpdateInboxRules](http://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx) para trabalhar com as regras. No entanto, observe que o EWS Managed API e EWS ter as seguintes limitações ao trabalhar com as regras de caixa de entrada: 
  
- EWS não consigo acessar ou criar regras de "somente cliente" ou que são definidas no Outlook para executar "em somente este computador".
    
- Para alterar o conjunto atual de regras usando o EWS, você precisa remover as regras do Outlook BLOB, se ele estiver presente. Isso significa que o usando o EWS para modificar as regras exclui todas as regras que foram anteriormente desativadas (disabled) usando o Outlook. 
    
### <a name="how-do-rules-work"></a>Como funcionam as regras?
<a name="bk_HowRulesWork"> </a>

O mecanismo de regras atua como um gatekeeper à caixa de correio do usuário. Como uma mensagem é recebida na caixa de correio do usuário, mas antes que a mensagem é exibida na caixa de entrada, a mensagem é avaliada em relação a uma lista ordenada de regras. Observe que isso ocorre apenas a hora de chegada e somente na caixa de entrada. Essas regras são compostas de três partes: [condições](#bk_Conditions), [exceções](#bk_Exceptions)e [ações](#bk_Actions).
  
O mecanismo de regras começando com a regra na parte superior da lista de regras, executa as seguintes etapas até alcançar o final da lista de regras:
  
1. Verifica a mensagem para determinar se ele atende a todas as condições especificadas na regra.
    
1. Se ela atender a todas as condições, avaliação continua com a etapa 2.
    
2. Se ele não atender a todas as condições, o mecanismo de regras carrega a próxima regra na lista de regras e inicia novamente na etapa 1.
    
2. Verifica a mensagem para determinar se ele atende a qualquer uma das exceções especificadas na regra.
    
1. Se ela atender a qualquer uma das exceções, o mecanismo de regras carrega a próxima regra na lista de regras e inicia novamente na etapa 1.
    
2. Se qualquer uma das exceções não atender, avaliação continua com a etapa 3.
    
3. Executa as ações especificadas na regra na mensagem.
    
1. Se a ação de "parar o processamento de mais regras" for especificada, o mecanismo de regras executa todas as ações na mensagem e sai sem avaliar quaisquer regras adicionais em relação a mensagem.
    
2. Se a ação de "parar o processamento de mais regras" não for especificada, o mecanismo de regras carrega a próxima regra na lista de regras e inicia novamente na etapa 1.
    
A figura a seguir mostra o processo que o mecanismo de regras segue.
  
**Figura 1: Visão geral mecanismo de regras**

![Um diagrama que mostra as etapas usadas pelo mecanismo de regras, começando pela avaliação da regra, determinando em seguida se os critérios da regra são atendidos e, por fim, executando a ação ou movendo para a regra seguinte até ser concluído.](media/Ex15_Rules_EngineOverview.png)
  
### <a name="putting-the-pieces-together---parts-of-a-rule"></a>Juntando as partes - partes de uma regra
<a name="bk_Pieces"> </a>

Imagine que você está concedendo instruções para alguém que estiver designado para organizar seu email de entrada é uma maneira de visualizar as partes de uma regra. Você pode dizer para essa pessoa: "quando uma mensagem que chega \<inserir condições aqui\>, faça \<inserir aqui ações\>, a menos que a mensagem \<inserir aqui para exceções\>. Vamos examinar mais detalhadamente cada parte.
  
#### <a name="conditions"></a>Condições
<a name="bk_Conditions"> </a>

[Condições](http://msdn.microsoft.com/library/f049a48c-9585-43f7-8549-0b8cb19a5eea%28Office.15%29.aspx) descrevem quando uma regra deve ser aplicada. Enquanto você pode omitir as condições de uma regra (resultando em uma regra que se aplica a todas as mensagens recebidas), é muito mais comum para regras ter condições que se aplicam a um subconjunto de mensagens de entrada. Alguns exemplos são "quando uma mensagem é de Sadie" ou "quando uma mensagem é enviada à lista de distribuição 'Cat vídeo amantes'". Regras podem ter várias condições. Quando as regras tem mais de uma condição, todas as condições devem ser atendidas para que o mecanismo de regras executar a ação especificada. 
  
#### <a name="actions"></a>Ações
<a name="bk_Actions"> </a>

[Ações](http://msdn.microsoft.com/library/c5aa96b1-2d8b-422f-8c2f-f118572ab23f%28Office.15%29.aspx) descrevem o que acontece quando uma regra se aplica. Exemplos são "mover a mensagem para a pasta 'Gatos'" ou "marcar a mensagem com prioridade 'Baixa'". Regras podem ter várias ações. Quando você especificar várias ações para uma regra, todas as ações são executadas quando a regra é aplicada. 
  
#### <a name="exceptions"></a>Exceções
<a name="bk_Exceptions"> </a>

[Exceções](http://msdn.microsoft.com/library/7cd63ac2-3441-4ed4-915b-6f90af4b28fc%28Office.15%29.aspx) descrevem quando não deve ser aplicadas a uma regra, mesmo se os critérios especificados nas condições forem atendidos. Exemplos são ", exceto se a mensagem é enviada somente para mim" ou ", exceto se a mensagem for de Mom". Uma regra pode ter várias exceções. Quando as regras têm mais de uma exceção e qualquer uma das exceções forem atendidas, a regra não é aplicada. 
  
### <a name="example-herding-those-cats"></a>Exemplo: Herding esses gatos
<a name="bk_Example"> </a>

Vamos dar uma olhada em como seus usuários podem usar as regras para eliminar o tráfego dessa lista de distribuição de vídeo de gato de Internet. Vamos pressupor o seguinte:
  
- Essas mensagens são enviadas para uma lista de distribuição chamada "Internet entusiastas de vídeo de gato".
    
- Seus usuários desejam ler essas mensagens eventualmente, elas simplesmente não desejam que elas congestionar suas caixas de entrada. Em vez disso, eles seriam arquivá-las em uma pasta chamada "Gatos".
    
- Os usuários desejam ler as mensagens enviadas para essa lista de distribuição por seu mãe imediatamente, pois Mom envia os vídeos funniest.
    
Isso instrui o mecanismo de regras a seguir: "quando uma mensagem é recebida ou seja enviada à lista de distribuição 'Internet Cat vídeo entusiastas', movê-lo para a pasta 'Gatos', a menos que a mensagem é de Mom." 
  
**Tabela 2. Definição de regra**

|**Parte da regra**|**Valor**|
|:-----|:-----|
|Condições  <br/> |Enviado à lista de distribuição 'Internet Cat vídeo entusiastas'  <br/> |
|Ações  <br/> |Move a mensagem para a pasta 'Gatos'  <br/> E parar o processamento de mais regras  <br/> |
|Exceções  <br/> |A partir de 'Mom'  <br/> |
   
> [!NOTE]
> Observe que "parar o processamento de mais regras" é uma das ações na regra resultante. Em geral é uma boa ideia incluir essa ação para evitar a confusão sobre quais regras de atuam em qualquer mensagem de determinado. No entanto, ao omitir esta ação e ordenação corretamente suas regras, é possível conseguir processamento mais avançado de seu email de entrada. Nesse caso, provavelmente é uma opção de segura que mensagens de vídeo de gato da Internet não exigem muita no caminho de processamento avançado. 
  
Logo depois de criar esta regra, uma nova mensagem vem em. Uma colega de trabalho espero envia uma mensagem à lista de distribuição. Se mentalmente executamos o trabalho do mecanismo de regras, a mensagem atenda a todas as condições (é enviada para 'Internet Cat vídeos entusiastas') e ela atende a nenhuma das exceções (não é de 'Mom'), então a regra será aplicada e a mensagem obtém movida para a pasta 'Gatos'.
  
A figura a seguir mostra como a regra é aplicada a uma mensagem de email de entrada.
  
**Figura 2. Mensagem de entrada é processada por uma regra**

![Uma ilustração que mostra uma nova mensagem enviada à lista de distribuição de um colaborador. A mensagem atende a todas as condições e a nenhuma das exceções definidas na regra, e é movida para a pasta Cats.](media/Ex15_Rules_RuleEvaluationSample.png)
  
## <a name="blocking-senders"></a>Bloquear remetentes
<a name="bk_Blocking"> </a>

Embora você possa criar uma regra que moverá todas as mensagens de um remetente específico para a pasta Lixo eletrônico, você também pode fazer isso usando a lista de remetentes bloqueados em suas opções de lixo eletrônico. Como não há um limite para quantos regras que um usuário pode ter, faz sentido usar a lista de remetentes bloqueados. Você pode [Adicionar ou remover os endereços de email específicos da lista de remetentes bloqueados](how-to-add-and-remove-email-addresses-from-blocked-senders-list-by-using-ews.md) usando o método de API gerenciada de EWS [ExchangeService.MarkAsJunk](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) ou a operação de EWS [MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) . Observe que, na ordem para o EWS acessar a lista de remetentes bloqueados, caixa de correio do usuário deve conter uma mensagem de email a partir do endereço de email que você deseja adicionar ou remover. 
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_InThisSection"> </a>

- [Gerenciar regras de caixa de entrada usando o EWS no Exchange](how-to-manage-inbox-rules-by-using-ews-in-exchange.md)
    
- [Adicionar e remover os endereços de email da lista de remetentes bloqueados usando o EWS no Exchange](how-to-add-and-remove-email-addresses-from-blocked-senders-list-by-using-ews.md)
    
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Operação GetInboxRules](http://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx)
    
- [Operação UpdateInboxRules](http://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx)
    
- [Operação MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)
    

