# 2024.2 Avaliação do 1o período de Sistemas Operacionais

## Informações gerais
- **Objetivo do repositório**: Avaliação do 1o bimestre da Disciplina de sistemas operacionais do curso de TADS do IFRN-CNAT
- **Público alvo**: alunos da disciplina de SO (Sistemas Operacionais) do curso de TADS (Superior em Tecnologia em Análise e Desenvolvimento de Sistemas) no CNAT-IFRN (Instituto Federal de Educação, Ciência e Tecnologia do Rio Grande do Norte - Campus Natal-Central).
- disciplina: **SO** Sistemas Operacionais
- professor: [Leonardo A. Minora](https://github.com/leonardo-minora)
- Aluna: [Yasmim Fernandes de O. Raposo](https://github.com/YasmimRaposo)
- Matrícula: 20231014040007

## Avaliação
- **Lembre de fazer o fork deste repositório**
- As questões foram construídas com o auxílio do [copilot](https://copilot.microsoft.com/)

# Questão 1. Introdução a sistemas operacionais

Considere as funções e objetivos principais de um sistema operacional conforme discutido no texto. Explique como um sistema operacional gerencia os recursos de hardware e software de um computador para garantir eficiência e segurança. Em sua resposta, aborde os seguintes pontos:

- Gerenciamento de processos
- Gerenciamento de memória
- Gerenciamento de dispositivos de entrada e saída
- Gerenciamento de arquivos

**Dica**: Pense em exemplos práticos de como o sistema operacional realiza essas tarefas no dia a dia de um usuário.

#### **RESPOSTA DA QUESTÃO 1:** 
O sistema operacional é o primeiro programa executado ao ligar o computador. Ele gerencia os recursos do computador conforme as necessidades do usuário, como memória e execução de aplicativos. Para garantir que os programas rodem de forma eficiente e evitar conflitos, o sistema operacional deve atuar de diversas formas, já que os recursos de um sistema possui suas particularidades e para mitigar possíveis problemas o SO possui funcionalidades específicas para abstrair e gerenciar os recursos. Essas funcionalidades são:<br>
- Gerenciamento processador → visa distribuir de forma justa a capacidade do processador para executar tarefas. Exemplo: quando você está com o site do spotify aberto e abre outra aba para realizar outra atividade na web, o SO aloca tempo de CPU para cada atividade. <br>
- Gerenciamento de memória → visa fornecer de modo independente uma área de memória para cada aplicação.Exemplo: quando você está jogando um jogo com um bom consumo de memória RAM e com outras tarefas abertas, como o software do word.<br>
- Gerenciamento de dispositivos → tem como objetivo implementar a interação com cada dispositivo por meio de drivers e criar modelos abstratos que permitam agrupar vários dispositivos similares sob a mesma interface de acesso. Exemplo: Ao utilizar fones de ouvido e conectá-los ao PC, notebook..., o SO detecta os dispositivos de entrada <br>
- Gerenciamento de arquivos → visa criar arquivos e diretórios, definindo sua interface de acesso e as regras
para seu uso. Exemplo: O gerenciamento de arquivos ocorre quando você cria e renomea pastas no "Explorador de arquivos" <br>
- Gerenciamento de proteção → responsável por garantir que apenas o destinatário tenha acesso à algo restrito e garantir segurança. Exemplo: quando há aviso de site de proteção duvidosa e o SO usa firewall para bloquear acessos não autorizados e um antivírus para detectar e remover possíveis ameaças.<br>


# Questão 2. Estrutura de sistemas operacionais

## Texto informativo
### Estrutura de Sistemas Operacionais: Custo de Desenvolvimento e Segurança da Informação

A estrutura de um sistema operacional (SO) é fundamental para determinar tanto o custo de desenvolvimento e manutenção quanto a segurança da informação. Existem várias arquiteturas de SO, como monolítica, microkernel e em camadas, cada uma com suas próprias implicações em termos de custo e segurança.

#### Custo de Desenvolvimento e Manutenção

1. **Arquitetura Monolítica**:
   - **Desenvolvimento**: Geralmente, mais rápida de desenvolver inicialmente, pois todos os componentes do SO são integrados em um único bloco de código.
   - **Manutenção**: Pode ser mais complexa e cara, pois qualquer alteração em um componente pode afetar todo o sistema, exigindo testes extensivos e cuidadosos.

2. **Arquitetura Microkernel**:
   - **Desenvolvimento**: Pode ser mais demorada e cara inicialmente, pois envolve a criação de um núcleo mínimo e a implementação de serviços adicionais como processos separados.
   - **Manutenção**: Mais fácil e menos custosa, já que os componentes são isolados. Atualizações e correções podem ser feitas em módulos específicos sem impactar o núcleo do sistema.

3. **Arquitetura em Camadas**:
   - **Desenvolvimento**: Moderadamente complexa, pois cada camada deve ser bem definida e interagir corretamente com as outras.
   - **Manutenção**: Relativamente fácil, pois problemas podem ser isolados e corrigidos em camadas específicas sem afetar o restante do sistema.

#### Segurança da Informação

1. **Arquitetura Monolítica**:
   - **Segurança**: Pode ser mais vulnerável, pois uma falha em qualquer parte do sistema pode comprometer todo o SO. A integração de todos os componentes em um único bloco de código pode dificultar a implementação de medidas de segurança robustas.

2. **Arquitetura Microkernel**:
   - **Segurança**: Geralmente mais segura, pois isola os serviços em processos separados. Isso limita o impacto de uma falha ou ataque a um único componente, protegendo o núcleo do sistema e outros serviços.

3. **Arquitetura em Camadas**:
   - **Segurança**: Oferece um bom equilíbrio, pois cada camada pode implementar suas próprias medidas de segurança. No entanto, a comunicação entre camadas deve ser cuidadosamente gerenciada para evitar vulnerabilidades.

### Conclusão

A escolha da arquitetura de um sistema operacional tem um impacto significativo tanto no custo de desenvolvimento e manutenção quanto na segurança da informação. Arquiteturas monolíticas podem ser mais rápidas e baratas de desenvolver inicialmente, mas podem acarretar custos de manutenção mais altos e maiores riscos de segurança. Por outro lado, arquiteturas microkernel e em camadas podem exigir um investimento inicial maior, mas oferecem vantagens em termos de manutenção e segurança.

## Questão
Com base no texto sobre a estrutura de sistemas operacionais, analise como as diferentes arquiteturas (monolítica, microkernel e camadas) impactam o custo com a equipe de desenvolvimento e a segurança do sistema operacional. Em sua resposta, considere os seguintes pontos:
- Complexidade de implementação e manutenção
- Necessidade de especialização da equipe
- Potenciais vulnerabilidades de segurança
- Facilidade de atualização e correção de falhas

**Dica:** Utilize exemplos de sistemas operacionais reais que adotam essas arquiteturas para ilustrar sua análise.

**Copilot informa**: Essa questão incentiva os alunos a considerarem tanto os aspectos econômicos quanto os de segurança ao avaliar diferentes arquiteturas de sistemas operacionais.

#### **RESPOSTA DA QUESTÃO 2:** 
**Arquitetura Monolítica:**<br>
A arquitetura monolítica integra todos os componentes do sistema operacional em um **único bloco de código**, facilitando o desenvolvimento inicial, mas tornando a **manutenção mais complexa e cara**. A equipe precisa ter conhecimento abrangente do sistema, pois **qualquer mudança pode afetar todo o sistema**, exigindo testes extensivos. Em termos de segurança, **uma falha em qualquer parte pode comprometer todo o SO**, dificultando a implementação de medidas robustas. As atualizações e correções são desafiadoras, pois qualquer alteração pode impactar significativamente o sistema. Um exemplo clássico de SO com arquitetura monolítica é o Unix, conhecido por sua estrutura integrada, que simplifica o desenvolvimento inicial, mas apresenta desafios em manutenção e segurança.<br>

![image](https://github.com/user-attachments/assets/ce309153-f28d-4a09-8683-ed7f51c90784)
> Na foto temos a estrutura de uma arquitetura monolítica, ou seja, todas as funções do aplicativo são gerenciadas e executadas em um só lugar, e o estilo de arquitetura que desenvolve um conjunto de pequenos serviços chamado "Microsserviços". 

<br>

**Arquitetura Microkernel:**<br>
A arquitetura microkernel envolve a **criação de um núcleo mínimo e a implementação de serviços adicionais como processos separados**, tornando a implementação mais demorada e cara inicialmente. No entanto, a **manutenção é mais fácil e menos custosa**, pois os componentes são isolados, permitindo atualizações e correções em módulos específicos sem impactar o núcleo. A equipe de desenvolvimento precisa ter conhecimento especializado para criar e manter módulos separados. Em termos de segurança, essa arquitetura é geralmente mais segura, pois **isola os serviços em processos distintos, limitando o impacto de falhas** ou ataques a um único componente e protegendo o núcleo do sistema. A facilidade de atualização e correção de falhas é um ponto forte dessa arquitetura, já que alterações podem ser feitas em módulos específicos sem afetar o restante do sistema. Um exemplo de sistema operacional que utiliza a arquitetura microkernel é o Minix.<br>

![image](https://github.com/user-attachments/assets/1c215e74-88a0-4739-be1d-9b3590015dd9)


**Arquitetura em Camadas:**<br>
A arquitetura em camadas possui uma **implementação moderadamente complexa**, já que cada **camada** deve ser bem definida e **interagir corretamente com as outras**. A **manutenção é relativamente fácil**, pois **problemas podem ser isolados e corrigidos em camadas específicas**, sem afetar o restante do sistema. A equipe precisa ter conhecimento especializado em cada camada, mas a compartimentação facilita a manutenção. Em termos de segurança, essa arquitetura oferece um bom equilíbrio, pois **cada camada pode implementar suas próprias medidas de segurança**. No entanto, a comunicação entre camadas deve ser bem gerenciada para evitar vulnerabilidades. A facilidade de atualização e correção de falhas é uma vantagem, já que problemas podem ser isolados e corrigidos em camadas específicas. Um exemplo prático de sistema operacional que utiliza essa arquitetura é o OS/2.<br>

![image](https://github.com/user-attachments/assets/2dd08956-63e6-4944-8438-eda58d6abd0d)


# Questão 3. Introdução à Segurança de Sistemas Operacionais

## Texto informativo

A segurança de um sistema operacional é um aspecto crucial que visa proteger os recursos do sistema contra acessos não autorizados, ataques maliciosos e falhas. Um sistema operacional seguro deve garantir a integridade, confidencialidade e disponibilidade dos dados e serviços. Para alcançar esses objetivos, várias técnicas e mecanismos são implementados, incluindo:

1. **Controle de Acesso**: Define quem pode acessar o sistema e quais recursos podem ser utilizados. Isso é feito através de autenticação (verificação de identidade) e autorização (permissão de acesso).

2. **Criptografia**: Utilizada para proteger dados em trânsito e em repouso, garantindo que apenas usuários autorizados possam acessar informações sensíveis.

3. **Auditoria e Monitoramento**: Registra atividades do sistema para detectar e responder a comportamentos suspeitos ou anômalos.

4. **Isolamento de Processos**: Garante que os processos sejam executados em ambientes isolados, evitando que um processo comprometa a segurança de outro.

5. **Atualizações e Patches**: Manter o sistema operacional atualizado é essencial para corrigir vulnerabilidades conhecidas e proteger contra novas ameaças.


## Questão

Considerando os mecanismos de segurança discutidos, analise como a implementação de controles de acesso e criptografia pode impactar a performance e a usabilidade de um sistema operacional. Em sua resposta, aborde os seguintes pontos:
- Benefícios e desafios de cada mecanismo
- Impacto na experiência do usuário
- Exemplos de situações onde esses mecanismos são críticos

**Dica:** Pense em como esses mecanismos são aplicados em sistemas operacionais que você utiliza no dia a dia, como Windows, Linux ou macOS.

**Copilot informa**: Essa questão incentiva os alunos a refletirem sobre o equilíbrio entre segurança, performance e usabilidade, aplicando conceitos teóricos a contextos práticos.

#### **RESPOSTA DA QUESTÃO 3:** 
**Controle de acesso:**<br>
Benefícios:<br>
- Impedir acesso de pessoas má-intencionadas<br>
- Monitor de referências(saber quem acessou, horário, etc)<br>
- Proteção de dados, ou seja, garantir  que apenas usuários autorizados tenham acesso a informações sensíveis.<br>
  
Desvantagens:<br>
- Gerenciamento complexo, ou seja, manutenção de políticas de acesso podem ser complexas.<br>
- Sobrecarga do sistema, ou seja, verificação contínua de permissões pode consumir recursos do sistema.<br>
 
Impacto na experiência do usuário: <br>
- Aumento da segurança e da confiança do usuário.<br>
- Pode gerar frustração se as políticas de acesso forem muito restritivas ao impedir o usuário de realizar algumas tarefas.<br>
  
Exemplo de situação: <br> 
- Sistemas financeiros. <br>

**Criptografia:**<br>
Benefícios:<br>
- Confidencialidade, ou seja, protege os dados em trânsito e em repouso, tornando-os ilegíveis para intrusos.<br>
- Integridade, ou seja, garante que os dados não sejam alterados durante a transmissão ou armazenamento.<br>
- Autenticação, ou seja, verifica a identidade de usuários e dispositivos, garantindo que apenas entidades autorizadas tenham acesso aos dados.<br>

Desvantagens:<br>
- Impacto na performance: Os algoritmos de criptografia consomem recursos computacionais, podendo afetar a velocidade de processamento e a responsividade do sistema.<br>
- Gerenciamento de chaves: A geração, armazenamento e distribuição de chaves criptográficas exigem cuidados especiais para evitar sua exposição e perda.<br>
- Complexidade: A implementação correta de sistemas criptográficos requer conhecimento técnico especializado.<br>

Impacto na experiência do usuário: <br>
- Aumento da segurança e da confiança do usuário, pois seus dados estão mais protegidos.<br>
- Pode exigir que o usuário digite senhas com frequência, o que pode ser inconveniente. Além disso, a criptografia pode aumentar o tempo de inicialização do sistema e o tempo de acesso aos arquivos.<br>

Exemplo de situação:: <br>
- WhatsApp: Todas as mensagens, chamadas de voz e videochamadas são criptografadas de ponta a ponta. Isso significa que apenas o remetente e o destinatário podem ler ou ouvir as mensagens, e nem mesmo o WhatsApp pode decifrá-las.

# Questão 4. Custo de Processamento versus Algoritmo Ótimo de Escalonamento

## Texto informativo

O escalonamento de processos é uma função crítica de um sistema operacional, responsável por determinar a ordem em que os processos são executados pelo processador. O objetivo é maximizar a eficiência do sistema, garantindo que os recursos sejam utilizados de maneira justa e eficaz. No entanto, encontrar o algoritmo de escalonamento ótimo envolve um equilíbrio delicado entre o custo de processamento e a eficiência do escalonamento.

### Custo de Processamento

O custo de processamento refere-se ao tempo e aos recursos necessários para executar um algoritmo de escalonamento. Algoritmos mais complexos podem oferecer melhores resultados em termos de tempo de resposta e utilização do processador, mas também podem exigir mais recursos computacionais para tomar decisões de escalonamento. Isso pode incluir tempo de CPU, memória e outras operações de sistema.

### Algoritmo Ótimo de Escalonamento

Um algoritmo ótimo de escalonamento é aquele que maximiza a eficiência do sistema operacional, minimizando o tempo de espera dos processos, o tempo de resposta e o tempo de retorno. Alguns dos algoritmos de escalonamento mais comuns incluem:

- **First-Come, First-Served (FCFS)**: Simples e fácil de implementar, mas pode levar a longos tempos de espera para processos curtos.
- **Shortest Job Next (SJN)**: Minimiza o tempo médio de espera, mas pode ser difícil de implementar devido à necessidade de prever o tempo de execução dos processos.
- **Round Robin (RR)**: Oferece uma abordagem justa, atribuindo fatias de tempo iguais a todos os processos, mas pode resultar em maior sobrecarga de contexto.
- **Priority Scheduling**: Processos com maior prioridade são executados primeiro, mas pode levar à inanição de processos de baixa prioridade.


## Questão

Considerando os conceitos de custo de processamento e algoritmo ótimo de escalonamento, analise como diferentes algoritmos de escalonamento podem impactar a performance de um sistema operacional em termos de tempo de resposta, tempo de espera e utilização do processador. Em sua resposta, aborde os seguintes pontos:
- Vantagens e desvantagens de pelo menos dois algoritmos de escalonamento
- Impacto do custo de processamento na escolha do algoritmo
- Exemplos de situações onde um algoritmo pode ser preferível a outro

**Dica:** Pense em como esses algoritmos são aplicados em diferentes cenários, como sistemas de tempo real, servidores web e sistemas operacionais de uso geral.

**Copilot informa**: Essa questão incentiva os alunos a refletirem sobre a complexidade e os trade-offs envolvidos na escolha de um algoritmo de escalonamento, aplicando conceitos teóricos a contextos práticos.


#### **RESPOSTA DA QUESTÃO 4:**<br>
**First-come, first served:**<br>
Vantagem:<br>
- atende processos na ordem de chegada, como uma fila(FIFO).<br>

Desvantagem:<br>
Pode ocorrer atrasos se houver muitos processos longos na frente, fazendo com que os processos curtos fiquem à muito tempo na fila, conhecido como "efeito comboio".<br>

Impacto: <br>
- Desempenho, pois aumenta significativamente o tempo de espera médio, especialmente em cenários com uma mistura de processos longos e curtos<br>

Exemplo: <br>
- Em um servidor de impressão compartilhada, os documentos enviados para impressão são processados na ordem em que chegam.<br>

**Round Robin (RR):**<br>
Vantagem: <br>
- cada processo recebe uma fatia de tempo da CPU de forma justa.<br>

Desvantagem:<br>
- trocas de contexto podem diminuir a eficiência, principalmente se a fatia de tempo de CPU for curta.<br>

Impacto:<br>
- Desempenho, pois frequentemente gera um overhead devido às trocas de contexto.<br>

Exemplo:<br>
- Jogos Multiplayer: Em um servidor de jogos multiplayer, cada jogador recebe uma fatia de tempo de processamento de forma justa.


**Shortest Job Next (SJN):**<br>
Vantagem:<br>
- seleciona o processo com o menor tempo de execução previsto para ser executado primeiro, minimizando, assim, o tempo de espera médio<br>

Desvantagem:<br>
- possibilidade de inanição de processos longos quando há fluxo constante de muitos processos curtos.<br>
- Dificil implementação para prever o tempo médio, tornando-a imprecisa.<br>

Impacto: <br>
- Desempenho (relacionado ao tempo de execução)<br>
- Implementação complexa.<br>

Exemplo: <br>
- Algumas impressoras utilizam o algoritmo SJN e imprimem os documentos menores que levam menos tempo, como uma página de texto, antes de imprimir documentos mais longos, como relatórios extensos.

**Priority Scheduling:**<br>
Vantagem:<br>
- seleciona o processo de maior prioridade<br>

Desvantagem:<br>
- possibilidade de inanição de processos de baixa prioridade, que podem ser adiados indefinidamente se processos de alta prioridade continuarem chegando<br>

Impacto: <br>
- Desempenho: Melhora o tempo de resposta para processos prioritários, mas pode prejudicar processos de baixa prioridade.<br>
- Implementação: Pode ser complexa, especialmente ao definir e gerenciar as prioridades dos processos.<br>

Exemplo: <br>
- Em Sistemas operacionais de uso geral o scheduler de prioridade é usado para garantir que processos críticos do sistema (como atualizações de segurança, gerenciamento de memória, ou drivers de hardware) sejam executados antes de processos de baixa prioridade (como aplicativos de usuário que estão em segundo plano)<br>









# Questão 5. Aplicativo em python vs aplicativos em c

## Questão

Explique o caminho que as instruções seguem desde um aplicativo escrito em Python e um aplicativo escrito em linguagem C até serem executadas pelo hardware. Em sua resposta, considere os seguintes pontos:
- O papel do interpretador no caso do Python
- O processo de compilação no caso do C
- A interação entre o kernel do sistema operacional e os drivers de dispositivo
- A tradução final das instruções para o formato binário (0 e 1) executado pelo hardware

**Dica:** Compare e contraste os dois processos, destacando as principais diferenças e semelhanças na forma como as instruções são processadas e executadas.

**Copilot informa**: Essa questão incentiva os alunos a refletirem sobre os diferentes caminhos que as instruções seguem em linguagens interpretadas e compiladas, aplicando conceitos teóricos a contextos práticos.

#### **RESPOSTA DA QUESTÃO 5:**<br>

### Aplicativo em Python:<br>

- Papel do Interpretador: Python é uma linguagem interpretada. O código-fonte é executado diretamente pelo interpretador, que o **converte em bytecode, uma representação intermediária próxima ao código de máquina**. Este bytecode é então executado pela Máquina Virtual Python (PVM).<br>
- Interação com Kernel e Drivers: Durante a execução, o interpretador pode fazer **chamadas ao sistema operacional para interagir com hardware**, como entrada/saída de dados e acesso a arquivos. Essas chamadas são **enviadas ao kernel**, que usa drivers apropriados para o hardware.<br>
- Tradução para Código Binário: O interpretador **converte dinamicamente o bytecode em instruções de máquina durante a execução**, oferecendo flexibilidade, mas com desempenho inferior devido à sobrecarga da interpretação em tempo real.<br>

### Aplicativo em C:<br>

- Processo de Compilação: C é uma linguagem compilada, **transformando o código-fonte em código de máquina antes da execução**. O processo **envolve pré-processamento**, compilação, montagem (assembly) e linkagem, resultando em um executável.<br>
- Interação com Kernel e Drivers: O executável pode **fazer chamadas ao sistema operacional para interagir com hardware, gerenciadas pelo kernel e drivers de dispositivos**.<br>
- Tradução para Código Binário: A **conversão para código binário ocorre durante a compilação**, criando um executável otimizado para a arquitetura alvo.<br>

### Comparação entre os Processos:<br>

- Tradução de Código: Python usa interpretação em tempo de execução, enquanto C usa compilação prévia.<br>
- Desempenho: Python pode ser mais lento devido à interpretação em tempo real. C geralmente é mais rápido, pois o código já está em formato binário otimizado.<br>
- Flexibilidade e Portabilidade: Python é altamente portátil, rodando em várias plataformas com o interpretador adequado. C é menos portável, podendo exigir ajustes e recompilação para diferentes plataformas.<br>
- Interação com o Sistema Operacional: Em ambos os casos, a interação com o hardware é mediada pelo kernel e drivers. No entanto, C oferece ao desenvolvedor mais controle sobre essas interações, permitindo otimizações de desempenho e uso de recursos.<br>

