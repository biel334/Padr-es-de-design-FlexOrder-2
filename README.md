# Padr-es-de-design-FlexOrder-2
🧩 Strategy (Estratégia)

Problema:
O sistema era completamente engessado — se eu quisesse mudar a forma de pagamento ou o tipo de frete, precisava alterar várias partes do código. Isso deixava o sistema difícil de manter e perigoso de modificar.

Solução:
Implementei o padrão Strategy, criando uma forma inteligente de trocar comportamentos sem alterar o restante do código.
Agora o sistema entende diferentes estratégias de pagamento (Pix, cartão, crédito interno, etc.) e estratégias de frete (normal, expresso ou até “teletransporte” 🚀).

Tudo funciona de forma modular — basta escolher qual estratégia usar.
Nada de ifs gigantes ou código duplicado: o sistema se adapta automaticamente à opção escolhida.

👉 Analogia: É como escolher o método de pagamento ou o tipo de entrega em um app de compras — o sistema continua o mesmo, só muda o “modo de operação”.


---

🎁 Decorator (Decorador)

Problema:
As regras de desconto, taxas e adicionais estavam todas misturadas no código principal.
Cada modificação virava um pesadelo: era preciso alterar várias partes do sistema e testar tudo de novo.

Solução:
Usei o padrão Decorator para criar uma estrutura flexível que permite empilhar funcionalidades.
Agora posso criar decoradores como:

Um que aplica desconto em pedidos grandes;

Outro que adiciona taxa de embalagem de presente;

Ou até um que oferece frete grátis em promoções especiais.


Posso combinar esses decoradores livremente, sem tocar nas regras originais — tudo se conecta como peças de LEGO. 🧱

👉 Analogia: É como montar um sanduíche: você escolhe o que quer adicionar (queijo, bacon, molho…), sem precisar refazer o pão toda vez. 🥪


---

🏗 Facade (Fachada)

Problema:
Para finalizar um pedido, era necessário interagir manualmente com várias partes do sistema — estoque, pagamento, nota fiscal, envio… Um verdadeiro labirinto de chamadas e dependências.

Solução:
Implementei o padrão Facade, criando uma interface simples que centraliza tudo isso.
Agora, basta um único comando para finalizar o pedido — a “fachada” cuida de chamar internamente todos os serviços necessários (registro, pagamento, emissão de nota, notificação ao cliente, etc.).

👉 Analogia: É como apertar o botão “Finalizar compra” em um e-commerce. O usuário vê apenas o botão, mas o sistema resolve toda a mágica por trás dos bastidores. ✨


---

🚀 Resultado Final

Com essa nova arquitetura:

✅ O código ficou organizado, modular e fácil de manter
✅ É simples adicionar novas funções sem quebrar o que já existe
✅ Cada parte pode ser testada isoladamente, com clareza e segurança
✅ O sistema ganhou flexibilidade e escalabilidade, pronto para crescer junto com o negócio

💡 Em resumo:
Transformei um código cheio de condições e dependências em um sistema limpo, extensível e profissional.
Agora posso mudar comportamentos, adicionar recursos e integrar novos serviços sem dores de cabeça — só escolhendo a estratégia certa. 😎💻