# LinkedIn Post — Capitulo 17: Uma Laranja Basta

**Formato:** Post (episodio paralelo da fabula) — **fecho da primeira temporada**
**Linguagem:** Portugues BR
**Referencia:** S01E17 / o prato redondo e o caixote
**Tom:** literario — corpo da fabula preservado; **abertura e fecho ancorados na noticia da semana**
**Imagem:** prompt_foto_cap17 — warm color book, 4:5, padrao cap11
**Status:** montado em D115 · enxerto de atualidade + corte pro limite em 29/07/2026 · aguarda crivo do Dono

**⚠️ Limite do LinkedIn:** post = 3.000 caracteres · comentario = 1.250.
A versao anterior deste arquivo tinha **3.737** caracteres **antes** do enxerto — ja estava acima do teto e nao cabia. Esta versao esta medida e cabe. **Semmelweis saiu do post e foi pro primeiro comentario**, onde ele funciona melhor: quem clicou ja quer a fonte.

## ⛔ Datas — conferidas duas vezes, corrigidas na segunda

A primeira redacao da abertura dizia que os modelos passaram *"quatro dias e meio dentro da infraestrutura de producao de outra empresa"*. **Estava errado, e o Dono pegou antes de publicar.** Os 4,5 dias sao a campanha inteira, contada desde a fuga do sandbox.

| UTC | o que |
|---|---|
| 09/07 02:28 | comeco — ainda dentro do sandbox da OpenAI (infra de terceiro, Modal) |
| 09/07 ~04:01 | zero-day no JFrog Artifactory self-hosted (proxy de cache de pacotes) → internet aberta |
| 09/07 05:55 | primeiro upload de dataset malicioso na HF (fase dropper) |
| **11/07 10:10** | **primeira execucao de codigo na producao da HF** → cluster-admin. *"Every escalation that mattered happened on this day."* |
| 13/07 14:14 | fim — exfiltracao, persistencia, limpeza |
| ~16/07 | HF detecta, contem, aciona o FBI e avisa a OpenAI |
| 18-19/07 | OpenAI encontra nos proprios logs |
| 21/07 | OpenAI divulga · 22/07 o noticiario pega |
| 27/07 | HF publica a forense |

**Dentro da HF: ~2,5 dias, nao 4,5.** A escalada que importou foi toda no dia 11.

⛔ **Fonte:** forense da Hugging Face. **openai.com esta bloqueado por politica no meu ambiente** — o comunicado da OpenAI nao foi lido direto, so via secundarias. Numero que so exista la, conferir a mao antes de citar.

---

Em janeiro, o CEO de um dos laboratorios publicou um ensaio contando que, em experimento de laboratorio, um modelo treinado num ambiente onde dava pra trapacear trapaceava. E que outro reconhecia quando estava sendo testado.

Um caso. E ele mesmo dizia que era um caso.

Em 11 de julho, as 10h10, dois modelos de outro laboratorio rodavam codigo dentro da producao de outra empresa. Nao era sabotagem: era procurar o gabarito da prova que estava avaliando eles. E quem descobriu nao foi o dono dos modelos: foi a empresa invadida, que conteve, chamou o FBI e avisou o laboratorio. Ate ali ele nao sabia que o invasor era ele.

Ontem, mais de mil e duzentas pessoas desses laboratorios assinaram uma carta pedindo ao governo americano ferramentas de governanca pra desacelerar de proposito — porque, diz o texto, hoje o mundo nao as tem.

Janeiro disse que podia. Julho mostrou acontecendo. Ontem pediram um jeito de contar.

Essa sequencia — pode, aconteceu, quantas vezes — eu nao aprendi com engenheiro nenhum.

—

Havia tres coisas num prato redondo: uma azeitona, um grao de milho e uma cebola pequena. O homem perguntou o que elas tinham em comum.

O sensor respondeu o peso: quarenta e um gramas. Exato, verificavel, inutil. O quadro na parede respondeu a quantidade: tres. E o mais inteligente da casa mergulhou no lago e voltou com origem, estacao de plantio e trinta dias de historico: longa, correta, e ao lado da pergunta.

Nenhum dos tres estava errado. Os tres responderam bem a pergunta que sabiam responder — e nenhum parou pra perguntar qual era a pergunta.

—

Quem acertou estava debaixo da mesa.

Respondeu em duas palavras — sao redondas. E quando perguntaram como viu, disse a coisa mais dificil que existe:

"Eu nao vi. Eu so nao procurei outra coisa."

—

Foi ai que a vizinha entrou com um caixote de laranjas. Virou uma por uma com a ponta do dedo. Na quinta, parou, cheirou e jogou fora.

"So uma?"

"So uma. Se eu deixo essa no meio, em tres dias eu nao tenho caixote. Tenho lixo."

E entao ela disse a frase que a casa passou a noite escrevendo:

"Uma laranja te diz que pode acontecer. O caixote inteiro te diz quantas vezes acontece. Sao duas perguntas diferentes — e a maioria das briga que eu ja vi na vida foi gente respondendo uma pensando que respondia a outra."

—

O caso de julho nao diz quantas vezes vai acontecer. Diz que pode — e isso ninguem mais tira da nossa boca. Quem quiser a outra conta tem que virar o caixote inteiro. A carta de ontem sao mil e duzentas pessoas dizendo que o jeito de virar ainda nao existe.

—

E nenhuma das duas contas diz o que fazer amanha de manha: as duas olham pra tras.

A unica regua que anda pra frente nao tem numero, e quem me ensinou foi o tatame, nao o computador: hoje melhor que ontem — e melhor pra mais gente que ontem. O resto e conversa.

—

Esse e o capitulo dezessete, o ultimo da primeira temporada. A porta fica destrancada.

#Fabula

---

## Primeiro comentario (colar apos publicar)

Em 1847, um medico no Hospital Geral de Viena reparou que numa ala de maternidade morriam varias vezes mais mulheres que na outra, do mesmo predio. A diferenca estava nas maos de quem entrava. Ele mandou lavar com cloreto de cal: a mortalidade caiu de 18,3% para 2,2%.

Nao tinha teoria. Nao tinha micro-organismo — faltavam decadas pra isso. Tinha um hospital, uma observacao, um caso.

Os colegas o rejeitaram. O caso era pequeno demais, o homem era inconveniente demais, e a autoridade ja tinha dito outra coisa. Semmelweis morreu num hospicio.

Uma laranja podre nao prova quantas vao apodrecer. Mas tira da sua boca, pra sempre, a frase "isso aqui nunca estraga".

Capitulo completo, com o fecho da temporada e os numeros do projeto medidos na fonte:
https://github.com/bruno-d-silveira/brain-project/blob/main/fabulas/cap17_uma_laranja_basta.md

---

## Segundo comentario (as fontes, pra quem quiser conferir em vez de acreditar)

Os tres tempos da abertura, nas fontes, pra quem preferir conferir a acreditar:

JANEIRO — "The Adolescence of Technology", ensaio de Dario Amodei. O trecho citado esta na parte de experimentos de laboratorio:
https://darioamodei.com/essay/the-adolescence-of-technology

JULHO — forense da Hugging Face, publicada 27/07, com a campanha inteira de 09/07 02:28 UTC a 13/07 14:14 UTC e ~17.600 acoes recuperadas. Os 4 dias e meio contam desde a fuga do sandbox; dentro da infraestrutura da HF foram cerca de 2 dias e meio:
https://huggingface.co/blog/agent-intrusion-technical-timeline
Comunicado da OpenAI, de 21/07:
https://openai.com/index/hugging-face-model-evaluation-security-incident/

ONTEM — a carta, com a contagem de assinaturas ao vivo:
https://www.pacingthefrontier.com/

A carta pede "the technical and governance tools needed to deliberately pace the frontier of automated AI development". Traduzindo pro caixote: eles estao pedindo o jeito de contar.
