# Consciência como Loop Autopreditivo com Peso Sináptico

## Uma hipótese neurocomputacional motivada por simulações do conectoma de *Drosophila melanogaster*

**Davi D'Artemis Sousa**  
Pesquisador independente  
Versão 2 — outubro de 2026 (versão 1: junho de 2026)

*Ensaio de hipótese: este texto propõe uma hipótese e um modo de testá-la; não relata resultados experimentais
sistematizados.*

---

## Resumo

Quando se injeta ruído e um sinal artificial de fome numa simulação do conectoma da mosca-da-fruta, o cérebro
simulado produz saídas motoras que parecem organizadas. A pergunta que motiva este ensaio é o que separa essa
atividade organizada de algo que mereça o nome de consciência. A resposta proposta é que a consciência do eu exige
um loop fechado no qual o sistema usa sua memória física, isto é, seus pesos sinápticos, e seus estados internos
para prever o próprio estado futuro. Duas objeções são examinadas. A primeira é que a ideia não é nova, e de fato
ela se sobrepõe ao processamento preditivo e às teorias do eu como modelo ou laço; o ensaio indica o que resta de
próprio. A segunda é mais séria: qualquer sistema com retroalimentação fica mais estável e recorrente, de modo que
estabilidade e recorrência não testam nada. Em resposta, propõe-se um controle em que a retroalimentação tem a
mesma estatística mas deixa de ser consequência das ações do próprio sistema, o que permite separar autorreferência
de mera recorrência. Por fim, o ensaio reconhece o que essa resposta não resolve: o teste mede autopredição, não
experiência, e os simuladores de conectoma atuais não têm plasticidade, sem a qual o papel da memória não pode ser
testado.

**Palavras-chave:** consciência; autopredição; processamento preditivo; recorrência; conectoma; *Drosophila
melanogaster*; memória; peso sináptico.

---

## 1. O problema: atividade organizada não é consciência

O conectoma completo do cérebro adulto da *Drosophila melanogaster* está mapeado [1, 2], e já é possível simular o
cérebro inteiro com modelos neuronais simples. Shiu et al. mostraram que um modelo de integração e disparo
construído só a partir da anatomia reproduz corretamente circuitos sensório-motores de alimentação e de limpeza [3].
Isso torna concreta uma pergunta que costuma ficar no plano abstrato: se uma simulação produz comportamento
coerente, o que, exatamente, estaria faltando para chamá-la de consciente?

Este ensaio nasceu de experimentos informais com esse tipo de simulação. Ao injetar ruído neural no conectoma, a
atividade se propagava e ativava vias motoras. Com estímulos externos presentes, as saídas pareciam coerentes. Sem
eles, a atividade se desorganizava ou entrava em regimes de alta atividade síncrona, que chamei informalmente de
"convulsivos". Quando acrescentei um sinal interno análogo à fome, o sistema ficou mais responsivo e passou a
produzir saídas compatíveis com busca de alimento. Essas observações não foram coletadas com protocolo fixo nem
quantificadas, e não são apresentadas aqui como evidência. Elas servem para formular o problema.

<!-- Para transformar estas observações em evidência, informar: conectoma usado (FlyWire, hemibrain, outro),
simulador e modelo neuronal, parâmetros e intensidade do ruído, quais neurônios foram lidos como "saída motora",
duração das simulações, número de repetições e uma definição operacional de "padrão convulsivo". -->

O problema é que nada nessas observações exige consciência para ser explicado. Num modelo com pesos fixos, um
estado interno como a fome funciona como uma mudança de limiar e de ganho em circuitos específicos. Na mosca real,
o mushroom body faz exatamente esse papel, integrando sinais sensoriais com o estado fisiológico do corpo [4, 5], e
neuromoduladores como dopamina, serotonina e, em insetos, octopamina ajustam excitabilidade e seleção de respostas
[6]. Comportamento organizado pode surgir inteiramente desse tipo de modulação. Uma simulação pode, portanto,
*parecer* buscar comida sem que haja ninguém buscando.

Para falar disso com precisão, é útil separar níveis que costumam ser confundidos. Estar vivo é ser um sistema
químico autossustentável, capaz de evolução darwiniana [7], e isso nada diz sobre experiência. Reagir é converter
estímulos em mudanças de estado e em ação, o que reflexos e circuitos modulados fazem sem precisar de um sujeito.
Acima disso, Damasio distingue um proto-self, ligado à regulação do corpo, uma consciência central do momento
presente e um eu autobiográfico que se estende no tempo [8, 9]. É nesse último nível, o de um eu com
continuidade, que este ensaio se concentra. A pergunta passa a ser: que tipo de dinâmica transforma um sistema que
reage num sistema que tem um eu?

## 2. A proposta: o eu como loop autopreditivo

A resposta proposta é a seguinte:

> **A consciência do eu emerge quando um sistema neural com peso sináptico suficiente passa a usar memória física,
> modulação química e recorrência de circuito para prever e atualizar continuamente o próprio estado.**

A ideia central é que o sistema não apenas reage ao mundo, mas reage às próprias reações. Sua saída volta como
entrada, e essa entrada é usada para prever o que o próprio sistema fará e sentirá em seguida. O eu, nessa leitura,
não é um objeto guardado em algum lugar do cérebro; é essa dinâmica autorreferente em funcionamento.

A hipótese depende de três ingredientes, e o argumento é que nenhum deles basta sozinho.

O primeiro é a **memória entendida como estrutura física**: alterações de conectividade e de força sináptica, e
redes de engramas que podem ser reativadas [10, 11]. Tratar a memória assim permite separá-la da consciência. Um
traço de memória continua existindo durante o sono profundo ou a anestesia, quando o processo que o usa está
interrompido. A memória é necessária para o eu autobiográfico, porque é ela que dá continuidade e histórico ao
sistema; mas, sem um processo ativo que a use, ela é só estrutura.

O segundo são os **estados internos**. Fome, sede, sono e estresse mudam o que é relevante para o organismo e,
portanto, o que vale a pena prever. Sem eles, um loop autopreditivo não teria nada de *seu* para prever; é por isso
que Seth coloca a predição dos estados do corpo, a interocepção, no centro da experiência de ser um eu [12]. Mas,
como se viu na Seção 1, estados internos sozinhos produzem apenas modulação.

O terceiro é o **loop fechado**: a saída do sistema, por exemplo o movimento que ele produz e o que esse movimento
muda no que ele sente, volta como entrada e é comparada com o que o sistema havia previsto. O erro dessa comparação
atualiza os pesos. Esquematicamente:

```python
while sistema_integrado:
    entrada = sinais_externos + sinais_internos + feedback_recorrente
    predicao = modelo_do_sistema(entrada, memoria_fisica, estado_interno)
    saida = resposta_motora_ou_cognitiva(predicao)
    erro = comparar(predicao, entrada_seguinte)
    memoria_fisica = atualizar_pesos(memoria_fisica, erro)
    feedback_recorrente = consequencias_da(saida)
```

O esquema descreve relações funcionais, não uma implementação de consciência.

Resta dizer o que significa "peso sináptico suficiente". Não há, nesta versão, um número. A definição adotada é
qualitativa: um sistema tem peso suficiente quando sua conectividade e sua memória acumulada permitem que o estado
interno de agora melhore a previsão do próprio estado futuro além do que as entradas externas já explicam. Na
Seção 4 essa definição se torna uma medida.

## 3. Primeira objeção: a ideia já existe

A objeção mais imediata é que nada disso é novo, e ela está em boa parte correta.

A ideia de que o cérebro é essencialmente uma máquina de predição está no princípio da energia livre de Friston
[13] e foi desenvolvida por Clark e Hohwy [14, 15]. Seth leva essa ideia para o eu: a experiência de ser alguém
seria a predição que o organismo faz de seus próprios estados corporais [12, 16]. Essa é a teoria mais próxima da
presente hipótese. A ênfase na recorrência também não é nova: para Lamme, a consciência depende de processamento
recorrente entre áreas, e não da simples passagem da informação para a frente [17]. E a ideia de que o eu não é um
objeto, mas um processo autorreferente, aparece no modelo de si de Metzinger [18] e no "laço estranho" de
Hofstadter [19].

As duas grandes teorias rivais seguem outro caminho. A Teoria da Informação Integrada identifica a consciência com a
estrutura causal integrada de um sistema, medida por Φ, independentemente do que ele faz ao longo do tempo [20, 21]. A
teoria do Espaço de Trabalho Global trata do acesso consciente a conteúdos, que se tornam conscientes quando são
difundidos por uma rede de longo alcance [22]. Nenhuma das duas é formulada em termos de um eu com continuidade, que
é o foco aqui. Uma revisão comparativa dessas teorias está em Seth e Bayne [23].

O que sobra de próprio, então? Duas coisas, ambas modestas. A primeira é tratar a memória física acumulada como
condição explícita: distinguir a autopredição momentânea, que poderia existir com pouca memória, da autopredição que
se apoia num histórico e por isso sustenta um eu que dura. A segunda, mais importante, aparece quando se enfrenta a
segunda objeção.

## 4. Segunda objeção: qualquer loop faz isso

A versão anterior deste ensaio propunha testar a hipótese comparando três condições numa simulação: ruído simples,
ruído com estado interno e loop fechado. A previsão era que o loop fechado produziria padrões mais estáveis,
recorrentes e persistentes. O problema é que essa previsão vale para praticamente qualquer sistema com
retroalimentação. Um termostato fica mais estável com o laço fechado; uma rede recorrente arbitrária também. Se o
loop fechado ganhar das outras duas condições, isso não diz nada sobre autopredição, muito menos sobre consciência.
O teste não teria como falhar.

A resposta a essa objeção é o que a hipótese realmente afirma. Ela não diz que a consciência do eu depende de
recorrência; diz que depende de recorrência **sobre si mesmo**. O que importa não é que algo volte como entrada, mas
que o que volta seja consequência das ações do próprio sistema, e que ele o use para prever a si mesmo. Isso pode
ser isolado com um controle.

Considere duas versões do loop fechado. Na primeira, a saída motora do sistema é transformada no sinal sensorial que
ela causaria, por exemplo o deslocamento num ambiente simulado, e volta como entrada. Na segunda, a entrada de
retroalimentação é a mesma saída do sistema, mas deslocada no tempo de forma aleatória, ou gravada de outra
execução. As duas entradas têm a mesma estatística: mesma intensidade, mesmos padrões, mesma variabilidade. A única
diferença é que, na segunda, o que volta deixou de ser consequência do que o sistema está fazendo agora. Um sistema
apenas recorrente deveria se comportar de modo parecido nas duas. Um sistema autopreditivo, não.

A medida que separa os dois casos é a **informação autopreditiva**: quanto o estado interno no instante *t* ajuda a
prever o estado do próprio sistema num instante futuro, descontado o que as entradas externas já explicam. Pode ser
estimada por entropia de transferência ou, mais simplesmente, treinando um preditor numa parte da simulação e
testando-o em outra. A previsão da hipótese é que essa informação seja maior com a retroalimentação verdadeira do que
com a embaralhada. Uma medida complementar é a complexidade da resposta a perturbações, em analogia ao índice usado
em humanos para distinguir estados conscientes e inconscientes [24].

O protocolo completo compara, portanto, quatro condições com o mesmo modelo neuronal, a mesma duração e várias
sementes aleatórias: ruído simples, ruído com estado interno, loop com retroalimentação verdadeira e loop com
retroalimentação embaralhada. As duas primeiras servem de referência; o contraste decisivo é entre as duas últimas.

Agora o teste pode falhar, e é isso que o torna útil. Se a retroalimentação verdadeira não produzir mais informação
autopreditiva do que a embaralhada, a hipótese, na forma funcional aqui proposta, fica enfraquecida. Fora da
simulação, ela também seria enfraquecida se, em sistemas biológicos, a perda de consciência no sono profundo ou na
anestesia não fosse acompanhada de queda da autopredição.

## 5. O que a resposta não resolve

Mesmo aceitando esse controle, restam problemas que este ensaio não resolve e que é melhor dizer com clareza.

O primeiro é o mais fundamental. Um resultado positivo mostraria que um sistema prevê a si mesmo; não mostraria que
ele sente algo. A distância entre uma propriedade funcional e a experiência subjetiva é o que Chalmers chamou de
problema difícil [25], e nenhuma medida deste protocolo atravessa essa distância. O que a hipótese oferece é uma
condição necessária plausível e testável, não uma explicação da experiência.

O segundo é técnico, mas atinge o centro da proposta. Os modelos de conectoma atuais usam pesos fixos, derivados da
anatomia [3]. Neles, a memória não muda com a experiência, e o passo de atualizar os pesos simplesmente não
existe. Esses modelos podem testar a diferença entre retroalimentação verdadeira e embaralhada, mas não podem testar
o papel da memória acumulada, que é justamente o que distingue esta hipótese das teorias vizinhas. Para isso seria
preciso acrescentar uma regra de plasticidade, por exemplo a plasticidade dependente de dopamina que ocorre nas
sinapses do mushroom body [4].

O terceiro é que a ênfase na continuidade levanta uma questão sobre identidade que a hipótese não responde. Parfit
discute o caso de uma duplicação perfeita: duas cópias de uma pessoa com exatamente as mesmas memórias [26]. Na
leitura proposta aqui, seriam dois loops distintos que começam de estados semelhantes, e não um mesmo eu, o que
sugere que a identidade está na continuidade do processo e não só no conteúdo da memória. Parfit chega a uma
conclusão relacionada por outro caminho, ao defender que o que importa para a sobrevivência é a continuidade
psicológica. Mas a hipótese apenas se alinha a essa posição; não a demonstra.

Por fim, este ensaio não toma posição sobre se insetos reais têm alguma forma de experiência, questão que Barron e
Klein discutem com seriedade [27]. A mosca entra aqui como sistema-modelo para comparar regimes dinâmicos, e as
observações que motivaram o texto continuam informais até que sejam repetidas com métodos explícitos.

## 6. Conclusão

O ponto de partida foi um problema concreto: uma simulação do cérebro da mosca produz comportamento organizado, e
nada nesse comportamento exige consciência. A proposta foi que o que falta é um loop no qual o sistema use sua
memória física e seus estados internos para prever a si mesmo. Contra a objeção de que a ideia já existe,
reconheceu-se a proximidade com o processamento preditivo e com as teorias do eu como modelo ou laço, e
identificou-se o que resta de próprio: a memória acumulada como condição explícita. Contra a objeção de que
qualquer loop produz estabilidade, propôs-se um controle com retroalimentação embaralhada, que transforma a hipótese
em algo que pode falhar. E reconheceu-se o que permanece em aberto: o teste mede autopredição e não experiência, e
só poderá avaliar o papel da memória quando os simuladores de conectoma incorporarem plasticidade.

O próximo passo é empírico: rodar as quatro condições com métodos explícitos e medir se a autorreferência, e não a
mera recorrência, deixa uma assinatura na dinâmica do sistema.

---

## Referências

1. Dorkenwald, S., Matsliah, A., Sterling, A. R., et al. (2024). Neuronal wiring diagram of an adult brain. *Nature, 634*, 124–138. https://doi.org/10.1038/s41586-024-07558-y
2. Scheffer, L. K., Xu, C. S., Januszewski, M., et al. (2020). A connectome and analysis of the adult *Drosophila* central brain. *eLife, 9*, e57443. https://doi.org/10.7554/eLife.57443
3. Shiu, P. K., Sterne, G. R., Spiller, N., et al. (2024). A *Drosophila* computational brain model reveals sensorimotor processing. *Nature, 634*, 210–219. https://doi.org/10.1038/s41586-024-07763-9
4. Li, F., Lindsey, J. W., Marin, E. C., Otto, N., Dreher, M., Dempsey, G., et al. (2020). The connectome of the adult *Drosophila* mushroom body provides insights into function. *eLife, 9*, e62576. https://doi.org/10.7554/eLife.62576
5. Suárez-Grimalt, R., Grunwald Kadow, I. C., & Scheunemann, L. (2024). An integrative sensor of body states: How the mushroom body modulates behavior depending on physiological context. *Learning & Memory, 31*(5), a053918. https://doi.org/10.1101/lm.053918.124
6. Tsuboi, D., Nagai, T., Yoshimoto, J., & Kaibuchi, K. (2024). Neuromodulator regulation and emotions: Insights from the crosstalk of cell signaling. *Frontiers in Molecular Neuroscience, 17*, 1376762. https://doi.org/10.3389/fnmol.2024.1376762
7. Benner, S. A. (2010). Defining life. *Astrobiology, 10*(10), 1021–1030. https://doi.org/10.1089/ast.2010.0524
8. Damasio, A. (1999). *The Feeling of What Happens: Body and Emotion in the Making of Consciousness*. Harcourt Brace.
9. Damasio, A. (2010). *Self Comes to Mind: Constructing the Conscious Brain*. Pantheon.
10. Rao-Ruiz, P., Visser, E., Mitrić, M., Smit, A. B., & van den Oever, M. C. (2021). A synaptic framework for the persistence of memory engrams. *Frontiers in Synaptic Neuroscience, 13*, 661476. https://doi.org/10.3389/fnsyn.2021.661476
11. Zaki, Y., & Cai, D. J. (2025). Memory engram stability and flexibility. *Neuropsychopharmacology, 50*, 285–293. https://doi.org/10.1038/s41386-024-01979-z
12. Seth, A. K. (2013). Interoceptive inference, emotion, and the embodied self. *Trends in Cognitive Sciences, 17*(11), 565–573. https://doi.org/10.1016/j.tics.2013.09.007
13. Friston, K. (2010). The free-energy principle: A unified brain theory? *Nature Reviews Neuroscience, 11*(2), 127–138. https://doi.org/10.1038/nrn2787
14. Clark, A. (2013). Whatever next? Predictive brains, situated agents, and the future of cognitive science. *Behavioral and Brain Sciences, 36*(3), 181–204. https://doi.org/10.1017/S0140525X12000477
15. Hohwy, J. (2013). *The Predictive Mind*. Oxford University Press.
16. Seth, A. (2021). *Being You: A New Science of Consciousness*. Faber & Faber.
17. Lamme, V. A. F. (2006). Towards a true neural stance on consciousness. *Trends in Cognitive Sciences, 10*(11), 494–501. https://doi.org/10.1016/j.tics.2006.09.001
18. Metzinger, T. (2003). *Being No One: The Self-Model Theory of Subjectivity*. MIT Press.
19. Hofstadter, D. R. (2007). *I Am a Strange Loop*. Basic Books.
20. Tononi, G. (2004). An information integration theory of consciousness. *BMC Neuroscience, 5*, 42. https://doi.org/10.1186/1471-2202-5-42
21. Tononi, G. (2008). Consciousness as integrated information: A provisional manifesto. *The Biological Bulletin, 215*(3), 216–242. https://doi.org/10.2307/25470707
22. Dehaene, S., & Changeux, J.-P. (2011). Experimental and theoretical approaches to conscious processing. *Neuron, 70*(2), 200–227. https://doi.org/10.1016/j.neuron.2011.03.018
23. Seth, A. K., & Bayne, T. (2022). Theories of consciousness. *Nature Reviews Neuroscience, 23*, 439–452. https://doi.org/10.1038/s41583-022-00587-4
24. Casali, A. G., Gosseries, O., Rosanova, M., et al. (2013). A theoretically based index of consciousness independent of sensory processing and behavior. *Science Translational Medicine, 5*(198), 198ra105. https://doi.org/10.1126/scitranslmed.3006294
25. Chalmers, D. J. (1995). Facing up to the problem of consciousness. *Journal of Consciousness Studies, 2*(3), 200–219.
26. Parfit, D. (1984). *Reasons and Persons*. Oxford University Press.
27. Barron, A. B., & Klein, C. (2016). What insects can tell us about the origins of consciousness. *Proceedings of the National Academy of Sciences, 113*(18), 4900–4908. https://doi.org/10.1073/pnas.1520084113

---

## Licença

Este texto está disponível sob a licença **Creative Commons Attribution 4.0 International (CC BY 4.0)**. Veja
[`LICENSE.md`](LICENSE.md).
