# Consciência como Loop Autopreditivo com Peso Sináptico

## Uma hipótese neurocomputacional motivada por simulações do conectoma de *Drosophila melanogaster*

**Davi D'Artemis Sousa**  
Pesquisador independente  
Versão 2 — outubro de 2026 (versão 1: junho de 2026)

**Tipo de trabalho:** ensaio de hipótese. Este texto propõe uma hipótese e um protocolo para testá-la; não relata
resultados experimentais sistematizados.

---

## Resumo

Este ensaio propõe uma hipótese sobre a consciência do eu como um processo recorrente de autopredição, sustentado
por memória física (pesos sinápticos), modulação neuroquímica e recorrência de circuito. A motivação vem de
observações preliminares, não sistematizadas, em simulações do conectoma de *Drosophila melanogaster*. Nelas, a
injeção de ruído neural e de estados internos artificiais produziu atividade e saídas motoras organizadas, o que
levou à pergunta sobre o que faltaria para que essa atividade constituísse algo além de reatividade.

O argumento distingue quatro níveis: vida, reatividade neural, proto-consciência e consciência do eu, numa linha
próxima à de Damasio. A memória é tratada como infraestrutura física, necessária para a continuidade do eu mas
insuficiente para explicá-la. A proposta é que a consciência do eu exige um circuito fechado no qual a saída do
sistema volta como entrada e é usada para prever o próprio estado futuro.

A hipótese é próxima de teorias existentes: o processamento preditivo (Friston, Clark, Seth, Hohwy), o
processamento recorrente (Lamme), o modelo de si (Metzinger) e a ideia do eu como "laço estranho" (Hofstadter).
Indicamos em que ela coincide com essas teorias e em que difere. Propomos um protocolo com quatro condições em
conectomas simulados, incluindo um controle com retroalimentação embaralhada que separa a autorreferência da mera
recorrência, e discutimos explicitamente o que as medidas propostas podem e não podem mostrar.

**Palavras-chave:** consciência; autopredição; processamento preditivo; recorrência; conectoma; *Drosophila
melanogaster*; memória; engrama; peso sináptico; mushroom body.

---

## 1. Introdução

A consciência continua sendo um dos problemas centrais da neurociência e da filosofia da mente [5, 11]. A biologia
tem definições operacionais razoáveis de vida, como a de sistema químico autossustentável capaz de evolução
darwiniana [1], mas essas definições não dizem nada sobre experiência subjetiva nem sobre a continuidade de um eu.
Um organismo pode estar vivo, reagir ao ambiente e ter atividade neural sem que isso implique consciência
autobiográfica.

Este ensaio distingue quatro níveis de organização: vida, reatividade neural, proto-consciência e consciência do
eu. A hipótese é que a consciência do eu não se reduz a nenhum componente isolado: não é só ruído neural, nem só
memória, nem só resposta motora, nem só integração sensorial. Ela é proposta como um **loop autopreditivo fechado**,
no qual a atividade recorrente usa pesos sinápticos de memória, modulação excitatória/inibitória e sinais internos
do organismo para gerar predições contínuas sobre o próprio sistema.

A motivação surgiu de experimentos informais com simulações do conectoma de *Drosophila melanogaster*. Nelas, a
introdução de ruído e de estados internos artificiais produziu saídas motoras aparentemente organizadas, enquanto a
remoção de estímulos externos levou a padrões difusos e instáveis (Seção 5). Essas observações não foram
sistematizadas e não são apresentadas como evidência; elas apenas sugerem que atividade neural e saída coerente
podem ser necessárias, mas não suficientes, para algo que mereça o nome de consciência.

**Contribuição.** Este texto não propõe uma teoria inteiramente nova. A ideia de que o eu é um processo recorrente
e autorreferente, e de que o cérebro é essencialmente um sistema de predição, já existe em várias formas (Seção 2).
A contribuição pretendida é mais modesta:

1. uma formulação compacta que junta três ingredientes — memória física, modulação por estado interno e
   retroalimentação autopreditiva — e afirma que nenhum deles basta sozinho;
2. um protocolo comparativo em conectomas simulados, com um controle que distingue **autorreferência** de **mera
   recorrência**;
3. uma discussão explícita dos limites do que esse tipo de medida pode mostrar.

---

## 2. Trabalhos relacionados

**Teoria da Informação Integrada (IIT).** A IIT identifica a consciência com a informação integrada de um sistema,
medida por Φ [2, 3]. Ela é uma teoria da *quantidade e estrutura* da experiência, definida pela organização causal
do sistema, não pela sua dinâmica preditiva. A presente hipótese não usa Φ; ela coloca a ênfase na função
(autopredição) e não na estrutura causal em si.

**Espaço de Trabalho Global (GNW).** Para a GNW, um conteúdo se torna consciente quando é difundido amplamente por
uma rede de longo alcance, num evento de "ignição" [4]. A GNW explica o acesso consciente a conteúdos; ela não trata
diretamente do eu nem da continuidade autobiográfica, que são o foco aqui.

**Processamento recorrente (RPT).** Lamme propõe que a consciência fenomenal depende de processamento recorrente
(retroalimentação) entre áreas sensoriais, e não apenas da varredura feedforward [12]. A presente hipótese
compartilha a ênfase na recorrência, mas exige algo mais forte: que a recorrência carregue uma *predição sobre o
próprio sistema*, e não apenas reverberação de conteúdos sensoriais.

**Processamento preditivo e inferência ativa.** No princípio da energia livre, o cérebro minimiza erro de predição
sobre suas entradas [13]; Clark e Hohwy desenvolvem a ideia do cérebro como máquina de predição [14, 15]. Seth
estende essa ideia para o eu: a experiência de ser um eu seria a predição que o organismo faz dos próprios estados
corporais, com papel central da interocepção [16, 17]. Essa é a teoria mais próxima da presente hipótese. A
diferença que propomos é de ênfase: tratar a *memória física acumulada* (o peso sináptico) como condição necessária
explícita para o eu autobiográfico, separando a autopredição momentânea (que poderia existir com pouca memória) da
autopredição que mantém continuidade ao longo do tempo.

**O eu como modelo e como laço.** Metzinger propõe que não existe um eu como objeto, mas um modelo de si
transparente que o sistema não reconhece como modelo [18]. Hofstadter descreve o eu como um "laço estranho": um
padrão autorreferente que emerge quando um sistema representa a si mesmo [19]. A frase "o eu não é um objeto
armazenado, mas uma dinâmica recorrente" (Seção 2.4) é essencialmente compatível com essas duas posições.

**Níveis de consciência.** A distinção entre proto-self, consciência central e eu autobiográfico é de Damasio
[20, 21]. Os termos "proto-consciência" e "consciência autobiográfica" usados aqui seguem de perto essa divisão.

**Consciência em insetos.** Barron e Klein argumentam que estruturas do cérebro de insetos poderiam sustentar uma
forma básica de experiência subjetiva [22]. Este ensaio não toma posição sobre essa questão; usa a *Drosophila*
apenas como sistema-modelo para comparar regimes dinâmicos.

**Simulações do conectoma da mosca.** O conectoma completo do cérebro adulto da *Drosophila* (FlyWire) [23] e o
conectoma do cérebro central (hemibrain) [24] permitem simular o cérebro inteiro com modelos neuronais simples. Shiu
et al. mostraram que um modelo de integração e disparo sobre o conectoma completo prevê corretamente circuitos
sensório-motores de alimentação e limpeza [25]. Esses modelos usam pesos fixos derivados da anatomia, sem
plasticidade, o que é relevante para o protocolo da Seção 9.

---

## 3. Definições conceituais

### 3.1 Vida

Vida é entendida aqui como um sistema químico autossustentável, capaz de manter organização interna, trocar energia
com o ambiente e, em escala evolutiva, participar de processos darwinianos [1]. A definição serve para separar
metabolismo de experiência subjetiva: um sistema vivo pode não ser consciente, assim como um sistema reativo pode
não ter um eu.

### 3.2 Reatividade neural

Reatividade neural é a capacidade de converter estímulos externos ou internos em mudanças de estado, respostas
motoras ou padrões de atividade. Reflexos, respostas a odores, orientação visual, modulação por fome e acionamento
motor podem ocorrer como dinâmica de circuito sem exigir consciência autobiográfica.

Comportamento organizado não é, por si só, prova de experiência subjetiva.

### 3.3 Proto-consciência

Proto-consciência é um estado intermediário de integração sensorial e interna, com regulação por estados corporais,
modulação de limiar e possível experiência primária, mas sem evidência de um eu autobiográfico estável. A categoria
corresponde aproximadamente ao proto-self e à consciência central de Damasio [20].

### 3.4 Consciência do eu

Consciência do eu é definida como um loop autopreditivo estável e recorrente, sustentado por memória física e
modulação neuroquímica, que mantém continuidade temporal e produz predições sobre as próprias mudanças internas.

Nessa formulação, o eu não é um objeto armazenado no cérebro; é uma dinâmica recorrente que usa a memória como peso
histórico para interpretar, prever e atualizar o próprio estado [18, 19].

### 3.5 Peso sináptico suficiente

A hipótese usa a expressão "peso sináptico suficiente". Ela não tem, nesta versão, uma definição quantitativa. A
definição qualitativa adotada é: **um sistema tem peso sináptico suficiente quando sua conectividade e sua memória
acumulada permitem que o estado interno em um instante melhore a predição do próprio estado em instantes futuros,
além do que as entradas externas já explicam.** A Seção 9.4 propõe uma medida que torna essa definição
operacional. Definir um limiar numérico fica como problema em aberto.

---

## 4. Memória como infraestrutura física

A memória costuma ser descrita de modo abstrato, como conteúdo mental ou informação armazenada. Para esta hipótese,
ela é tratada antes de tudo como fenômeno físico: alterações de conectividade, força sináptica, padrões de
reativação e redes de engramas [6, 7].

Isso permite separar memória de consciência. Um traço de memória pode persistir como estrutura física enquanto o
sistema está inconsciente, desde que o loop que usa e atualiza esse traço esteja interrompido.

A memória é, portanto, necessária para a consciência autobiográfica, mas não suficiente. Ela dá peso, continuidade
e histórico ao sistema; o loop é a dinâmica ativa que usa esses pesos para gerar autopredição. Sem memória, o eu
perderia continuidade; sem o loop, a memória seria estrutura inerte.

### 4.1 Memória curta e memória autobiográfica

Distinguimos dois usos funcionais da memória. Em sistemas simples, ela pode operar como retenção curta, ajuste de
limiar e repetição de padrões recentes. Em sistemas mais densos e recorrentes, passa a sustentar continuidade
autobiográfica, identidade e predição de longo alcance. A distinção permite falar de formas iniciais de experiência
sem supor que toda experiência já contenha um eu narrativo.

---

## 5. Excitação, inibição e estados internos

A atividade de um circuito não depende só da anatomia. Glutamato, GABA, dopamina, serotonina, acetilcolina e, em
insetos, octopamina regulam excitabilidade, limiar de disparo, ganho sensorial, motivação e seleção de respostas
[10]. Estados internos como fome, sede, sono ou estresse podem mudar muito o comportamento sem que seja preciso
invocar consciência.

Na *Drosophila*, o mushroom body integra sinais sensoriais com estados fisiológicos e modula o comportamento de
acordo com o contexto corporal [8, 9]. Em organismos, a fome aumenta a saliência de odores associados a alimento;
em conectomas simulados, um estado interno artificial pode aumentar a sensibilidade a certos estímulos e facilitar
saídas motoras.

A hipótese interpreta esses fenômenos como modulação de circuito: estados internos não criam consciência por si
mesmos, mas fornecem parte das condições para um loop autopreditivo biologicamente relevante — em particular, a
dimensão interoceptiva que Seth considera central para o eu [16].

---

## 6. Observações preliminares em conectomas simulados

*Esta seção descreve observações informais que motivaram a hipótese. Elas não foram coletadas com protocolo fixo,
não foram quantificadas e não devem ser lidas como resultado experimental.*

<!-- Para transformar esta seção em evidência, informar: conectoma usado (FlyWire, hemibrain, outro), simulador e
modelo neuronal (por exemplo, o modelo de integração e disparo de Shiu et al.), parâmetros e intensidade do ruído,
quais neurônios foram lidos como "saída motora", duração das simulações, número de repetições, e uma definição
operacional de "padrão convulsivo". -->

Nas simulações que motivaram este ensaio, a injeção de ruído neural no conectoma gerou atividade e ativação de vias
motoras. Com estímulos externos presentes, o sistema produzia saídas que pareciam coerentes. Sem estímulos externos,
a atividade tendia a ficar desorganizada ou a entrar em regimes de alta atividade síncrona (descritos informalmente
como "convulsivos").

A introdução de um estado interno artificial análogo à fome aumentou a responsividade e facilitou saídas
compatíveis com busca de alimento. Isso é esperado: em modelos com pesos fixos, um estado interno funciona como
mudança de limiar e de ganho em circuitos específicos, e circuitos sensório-motores de alimentação já foram
reproduzidos dessa forma [25].

A leitura proposta é cautelosa: **ruído e estados internos ativam o circuito, mas nada nessas observações indica um
loop autopreditivo.** O conectoma pode produzir saída funcional sem que se possa concluir nada sobre consciência.
É essa lacuna que motiva o protocolo da Seção 9.

---

## 7. Hipótese central

> **A consciência do eu emerge quando um sistema neural com peso sináptico suficiente passa a usar memória física,
> modulação química e recorrência de circuito para prever e atualizar continuamente o próprio estado.**

O sistema não apenas reage ao mundo: reage às próprias reações, transformando sua saída em nova entrada e usando
essa entrada para prever a si mesmo.

Nessa formulação, a consciência não está numa área, numa substância ou numa memória isolada; é uma organização
dinâmica. A memória dá o peso histórico; excitação e inibição regulam a estabilidade; os estados internos definem o
que é relevante; os sensores fornecem entrada; e o loop fechado produz continuidade autopreditiva.

### 7.1 Formulação esquemática

```python
estado_interno = ruido_basal + modulacao_neuroquimica
memoria_fisica = pesos_sinapticos + redes_de_engrama

while sistema_integrado:
    entrada = sinais_externos + sinais_internos + feedback_recorrente

    predicao = modelo_do_sistema(entrada, memoria_fisica, estado_interno)

    saida = resposta_cognitiva_ou_motora(predicao)
    erro = comparar(predicao, entrada_atualizada)

    memoria_fisica = atualizar_pesos(memoria_fisica, erro, saida)

    feedback_recorrente = transformar_saida_em_nova_entrada(saida)
```

O esquema é conceitual: descreve as relações funcionais propostas, não uma implementação de consciência. Note que
ele inclui `atualizar_pesos`, isto é, plasticidade. Simulações de conectoma com pesos fixos não implementam esse
passo (Seção 9.5).

---

## 8. Predições e critérios de refutação

### 8.1 Predições

1. Ruído neural sem estímulo deve aumentar a atividade, mas não produzir estados internos que prevejam o próprio
   futuro do sistema.
2. Estados internos simulados devem alterar ganho, limiar e seleção de respostas, podendo gerar saída coerente sem
   autopredição.
3. Um loop fechado entre regiões sensoriais, de memória e motoras deve produzir padrões mais estáveis e recorrentes
   do que ruído difuso.
4. **Previsão distintiva:** com a retroalimentação do próprio sistema, o estado interno deve conter mais informação
   sobre o estado futuro do próprio sistema do que com uma retroalimentação de mesma estatística, mas desacoplada no
   tempo (Condição D, Seção 9).
5. Interromper a retroalimentação deve reduzir essa informação autopreditiva e fragmentar a continuidade.
6. Com plasticidade, a informação autopreditiva deve crescer com a experiência acumulada (o "peso").

### 8.2 O que essas predições podem e não podem mostrar

As predições 1 a 3 valem para praticamente qualquer sistema dinâmico com retroalimentação: um termostato ou uma rede
recorrente qualquer também fica mais estável com o laço fechado. Elas são **marcadores funcionais**, não testes de
consciência. A predição 4 é a que distingue esta hipótese de "recorrência genérica", porque compara autorreferência
com recorrência de mesma estatística. Mesmo ela mede uma propriedade funcional (autopredição), e não experiência
subjetiva: nenhuma medida deste protocolo resolve o problema difícil [5].

### 8.3 Critérios de refutação

A hipótese, na forma funcional aqui proposta, seria enfraquecida se:

- a Condição C (retroalimentação do próprio sistema) não superar a Condição D (retroalimentação embaralhada) na
  medida de informação autopreditiva;
- em sistemas biológicos, perdas de consciência (sono profundo, anestesia) não forem acompanhadas de queda da
  autopredição, ou se a autopredição se mantiver intacta quando a consciência é perdida.

---

## 9. Protocolo proposto

Comparar quatro condições numa simulação do conectoma da *Drosophila* [23, 25], com o mesmo modelo neuronal, a mesma
duração e várias sementes aleatórias por condição.

### 9.1 Condição A: ruído neural simples

Ruído basal sem estímulos externos relevantes. Medir propagação, estabilidade, entropia da atividade e ativação de
vias motoras. Predição: atividade sem autopredição sustentada.

### 9.2 Condição B: ruído com estado interno

Adicionar um modulador interno artificial (fome, sede ou mudança do balanço excitação/inibição). Medir se ele
altera a sensibilidade a estímulos específicos e facilita saídas coerentes. Predição: saída mais direcionada, ainda
explicável por limiar e ganho.

### 9.3 Condição C: loop autopreditivo fechado

Fechar um circuito entre regiões sensoriais, mushroom body, circuitos moduladores e saída motora: a saída motora,
transformada em sinal sensorial (por exemplo, pelo deslocamento que ela causaria num ambiente simulado), volta como
entrada.

### 9.4 Condição D: controle com retroalimentação embaralhada

Igual à Condição C, mas a entrada de retroalimentação é a saída do próprio sistema **deslocada no tempo de forma
aleatória** (ou gravada de outra execução). A estatística da entrada é a mesma, mas ela deixa de ser consequência
das ações atuais do sistema. A diferença entre C e D isola o efeito da autorreferência.

### 9.5 Métricas

- **Informação autopreditiva:** informação mútua entre o estado interno no instante *t* e o estado do próprio
  sistema em *t + k*, condicionada às entradas externas (por exemplo, por entropia de transferência ou por um
  preditor linear treinado em uma parte da simulação e testado em outra). É a medida que torna operacional a
  definição da Seção 3.5.
- **Complexidade de resposta a perturbações:** perturbar o sistema e medir a complexidade da resposta, em analogia
  ao índice de complexidade perturbacional usado em humanos para distinguir estados conscientes e inconscientes [26].
- Estabilidade temporal e autocorrelação dos padrões de ativação.
- Persistência de estados sem estímulo externo.
- Com plasticidade: variação dos pesos após ciclos recorrentes.

**Sobre plasticidade.** Os modelos de conectoma atuais usam pesos fixos [25]. Nessa forma, eles podem testar as
predições 1 a 5, mas não a predição 6. Testar o papel da memória acumulada exige acrescentar uma regra de
plasticidade (por exemplo, plasticidade dependente de dopamina nas sinapses do mushroom body [8]).

---

## 10. Discussão

A hipótese tenta evitar dois reducionismos: reduzir consciência à memória e reduzir consciência à reatividade. A
memória é essencial para a continuidade do eu, mas não explica a experiência; e comportamento organizado pode
surgir de circuitos modulados por estados internos sem consciência.

**Identidade e continuidade.** Considere o caso, discutido por Parfit, de uma duplicação perfeita: duas cópias de um
sistema neural com as mesmas memórias [27]. Na leitura proposta aqui, as cópias não seriam a mesma consciência em
continuidade, mas dois loops distintos iniciados de estados semelhantes. Isso sugere que a identidade do eu não está
só no conteúdo da memória, mas na continuidade física e funcional do processo recorrente. Parfit chega a uma
conclusão relacionada por outro caminho: o que importa para a sobrevivência seria a continuidade psicológica, e não
a identidade em sentido estrito.

**Relação com o processamento preditivo.** A hipótese pode ser lida como um caso particular do processamento
preditivo aplicado ao eu [16, 17], com duas ênfases próprias: (i) a memória física acumulada como condição explícita
para o eu *autobiográfico*, e (ii) a exigência de que a autopredição seja testada contra um controle de recorrência
sem autorreferência. Se essas ênfases acrescentam algo de substantivo às formulações existentes é uma questão em
aberto, que o protocolo da Seção 9 pode ajudar a responder.

**Gradação.** A consciência é tratada como gradual: de reatividade, para proto-consciência, para autopredição
estável com continuidade. A hipótese não trata do desenvolvimento humano; ela se restringe a sistemas-modelo
simulados.

---

## 11. Limitações

- É um ensaio de hipótese. As observações que o motivaram são informais e não quantificadas (Seção 6).
- Não demonstra a presença ou ausência de consciência em *Drosophila* ou em sistemas artificiais, e não resolve o
  problema da experiência subjetiva [5].
- As medidas propostas são funcionais. Um resultado positivo mostraria autopredição, não experiência.
- "Peso sináptico suficiente" tem apenas uma definição qualitativa.
- Conectomas anatômicos não capturam neuromodulação real, plasticidade, glia, metabolismo, oscilações nem o corpo.
  Toda simulação conectômica é um modelo parcial.
- A hipótese se sobrepõe a teorias existentes (Seção 2); sua contribuição está na combinação dos ingredientes e no
  protocolo, não na ideia de loop autorreferente em si.

---

## 12. Conclusão

Segundo a hipótese apresentada, a consciência do eu não é uma substância nem um elemento isolado, mas uma dinâmica
recorrente: um loop autopreditivo que usa memória física, modulação química, estados internos e retroalimentação
para manter continuidade temporal e prever o próprio estado.

Um conectoma pode reagir ao mundo sem consciência autobiográfica; pode ter integração sensorial e interna sem um eu
estável; e pode conter memórias físicas sem que elas estejam operando num processo consciente. Peso sináptico
suficiente seria condição necessária, mas não suficiente: ele precisa estar incorporado a um loop ativo, integrado e
autorreferente.

O próximo passo é empírico: comparar, em simulações do conectoma, ruído, modulação por estado interno, loop fechado
e loop com retroalimentação embaralhada, medindo a informação autopreditiva de cada condição.

---

## Referências

1. Benner, S. A. (2010). Defining life. *Astrobiology, 10*(10), 1021–1030. https://doi.org/10.1089/ast.2010.0524
2. Tononi, G. (2004). An information integration theory of consciousness. *BMC Neuroscience, 5*, 42. https://doi.org/10.1186/1471-2202-5-42
3. Tononi, G. (2008). Consciousness as integrated information: A provisional manifesto. *The Biological Bulletin, 215*(3), 216–242. https://doi.org/10.2307/25470707
4. Dehaene, S., & Changeux, J.-P. (2011). Experimental and theoretical approaches to conscious processing. *Neuron, 70*(2), 200–227. https://doi.org/10.1016/j.neuron.2011.03.018
5. Chalmers, D. J. (1995). Facing up to the problem of consciousness. *Journal of Consciousness Studies, 2*(3), 200–219.
6. Rao-Ruiz, P., Visser, E., Mitrić, M., Smit, A. B., & van den Oever, M. C. (2021). A synaptic framework for the persistence of memory engrams. *Frontiers in Synaptic Neuroscience, 13*, 661476. https://doi.org/10.3389/fnsyn.2021.661476
7. Zaki, Y., & Cai, D. J. (2025). Memory engram stability and flexibility. *Neuropsychopharmacology, 50*, 285–293. https://doi.org/10.1038/s41386-024-01979-z
8. Li, F., Lindsey, J. W., Marin, E. C., Otto, N., Dreher, M., Dempsey, G., et al. (2020). The connectome of the adult *Drosophila* mushroom body provides insights into function. *eLife, 9*, e62576. https://doi.org/10.7554/eLife.62576
9. Suárez-Grimalt, R., Grunwald Kadow, I. C., & Scheunemann, L. (2024). An integrative sensor of body states: How the mushroom body modulates behavior depending on physiological context. *Learning & Memory, 31*(5), a053918. https://doi.org/10.1101/lm.053918.124
10. Tsuboi, D., Nagai, T., Yoshimoto, J., & Kaibuchi, K. (2024). Neuromodulator regulation and emotions: Insights from the crosstalk of cell signaling. *Frontiers in Molecular Neuroscience, 17*, 1376762. https://doi.org/10.3389/fnmol.2024.1376762
11. Seth, A. K., & Bayne, T. (2022). Theories of consciousness. *Nature Reviews Neuroscience, 23*, 439–452. https://doi.org/10.1038/s41583-022-00587-4
12. Lamme, V. A. F. (2006). Towards a true neural stance on consciousness. *Trends in Cognitive Sciences, 10*(11), 494–501. https://doi.org/10.1016/j.tics.2006.09.001
13. Friston, K. (2010). The free-energy principle: A unified brain theory? *Nature Reviews Neuroscience, 11*(2), 127–138. https://doi.org/10.1038/nrn2787
14. Clark, A. (2013). Whatever next? Predictive brains, situated agents, and the future of cognitive science. *Behavioral and Brain Sciences, 36*(3), 181–204. https://doi.org/10.1017/S0140525X12000477
15. Hohwy, J. (2013). *The Predictive Mind*. Oxford University Press.
16. Seth, A. K. (2013). Interoceptive inference, emotion, and the embodied self. *Trends in Cognitive Sciences, 17*(11), 565–573. https://doi.org/10.1016/j.tics.2013.09.007
17. Seth, A. (2021). *Being You: A New Science of Consciousness*. Faber & Faber.
18. Metzinger, T. (2003). *Being No One: The Self-Model Theory of Subjectivity*. MIT Press.
19. Hofstadter, D. R. (2007). *I Am a Strange Loop*. Basic Books.
20. Damasio, A. (1999). *The Feeling of What Happens: Body and Emotion in the Making of Consciousness*. Harcourt Brace.
21. Damasio, A. (2010). *Self Comes to Mind: Constructing the Conscious Brain*. Pantheon.
22. Barron, A. B., & Klein, C. (2016). What insects can tell us about the origins of consciousness. *Proceedings of the National Academy of Sciences, 113*(18), 4900–4908. https://doi.org/10.1073/pnas.1520084113
23. Dorkenwald, S., Matsliah, A., Sterling, A. R., et al. (2024). Neuronal wiring diagram of an adult brain. *Nature, 634*, 124–138. https://doi.org/10.1038/s41586-024-07558-y
24. Scheffer, L. K., Xu, C. S., Januszewski, M., et al. (2020). A connectome and analysis of the adult *Drosophila* central brain. *eLife, 9*, e57443. https://doi.org/10.7554/eLife.57443
25. Shiu, P. K., Sterne, G. R., Spiller, N., et al. (2024). A *Drosophila* computational brain model reveals sensorimotor processing. *Nature, 634*, 210–219. https://doi.org/10.1038/s41586-024-07763-9
26. Casali, A. G., Gosseries, O., Rosanova, M., et al. (2013). A theoretically based index of consciousness independent of sensory processing and behavior. *Science Translational Medicine, 5*(198), 198ra105. https://doi.org/10.1126/scitranslmed.3006294
27. Parfit, D. (1984). *Reasons and Persons*. Oxford University Press.

---

## Licença

Este texto está disponível sob a licença **Creative Commons Attribution 4.0 International (CC BY 4.0)**. Veja
[`LICENSE.md`](LICENSE.md).
