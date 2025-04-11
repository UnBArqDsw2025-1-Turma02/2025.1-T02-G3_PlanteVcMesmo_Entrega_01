# 1.2.4. Léxico

## Visão Geral
Refere-se ao conjunto de termos e definições específicos utilizados em um projeto ou domínio. Em engenharia de requisitos, o léxico garante que todos os stakeholders tenham uma compreensão comum dos termos e conceitos empregados nos requisitos. Isso inclui definições de termos técnicos, nomes de entidades e processos, e pode ajudar a evitar ambiguidades e mal-entendidos ao comunicar e documentar requisitos.

## Trabalho realizado

###  Introdução

O léxico é um artefato fundamental da Engenharia de Requisitos, utilizado para descrever de maneira estruturada os elementos conceituais de um sistema. Neste documento, apresentamos o léxico do sistema **Plante Você Mesmo**, uma plataforma digital educativa voltada à instrução e engajamento de usuários no cuidado com plantas, promovendo uma comunidade sustentável e acessível.

O objetivo deste léxico é garantir a consistência na comunicação entre desenvolvedores, stakeholders e usuários, por meio da definição clara de termos essenciais do domínio do sistema.

###  Metodologia

A construção do léxico foi baseada nos princípios de engenharia semiótica, utilizando a técnica de elaboração de Léxicos de entidades, ações e estados. Foram analisadas as necessidades levantadas em brainstorming e sessões de *Design Sprint*, em especial o Dia 1 (Entendimento). Foram considerados elementos identificados em entrevistas, pesquisas com usuários e *benchmarks* de sistemas similares.

Cada termo foi classificado em uma das três categorias: **Objeto** (substantivo), **Verbo** (ação) ou **Estado** (condição), e descrito com:

- **Notação**: nome do termo.  
- **Sinônimos** (quando houver).  
- **Descrição**: definição detalhada.  
- **Impacto no sistema**: implicações práticas do termo.  
- **Relacionamentos**: outros termos do léxico com os quais se conecta.

###  Objetos

#### 🌱 Planta

- **Sinônimos**: espécie, vegetal  
- **Descrição**: Organismo vivo que será cultivado, estudado e monitorado na plataforma.  
- **Impacto**: É o elemento central do sistema. Cada planta terá um cadastro com informações específicas sobre cuidados, ambiente ideal, frequência de rega, etc.  
- **Relacionamentos**: Cuidados, Usuário, Ambiente

#### 👤 Usuário

- **Sinônimos**: participante, membro, visitante  
- **Descrição**: Pessoa que utiliza a plataforma, podendo ser iniciante, entusiasta ou especialista.  
- **Impacto**: Suas interações determinam o fluxo da plataforma. Recebem recomendações personalizadas e acessam conteúdos diversos.  
- **Relacionamentos**: Fórum, Perfil, Comunidade, Planta

#### 🧠 Recomendação

- **Sinônimos**: sugestão, orientação  
- **Descrição**: Informações oferecidas ao usuário com base no perfil, localização e espécies cadastradas.  
- **Impacto**: Serve para auxiliar na escolha e cuidado com plantas.  
- **Relacionamentos**: Usuário, IA, Planta

#### 🧩 Comunidade

- **Descrição**: Espaço colaborativo para troca de experiências entre usuários.  
- **Impacto**: Fortalece a retenção de usuários e promove aprendizagem coletiva.  
- **Relacionamentos**: Fórum, Postagem, Discussão

#### 💬 Fórum

- **Sinônimos**: espaço de discussão, comunidade  
- **Descrição**: Ferramenta integrada onde usuários podem publicar dúvidas, compartilhar dicas e interagir.  
- **Impacto**: Essencial para engajamento e construção de conhecimento colaborativo.  
- **Relacionamentos**: Comunidade, Postagem, Moderação

###  Verbos

#### 🔍 Cadastrar

- **Descrição**: Ação de inserir novas informações no sistema, como dados pessoais, planta ou recomendação.  
- **Impacto**: Permite personalização do conteúdo para o usuário.  
- **Relacionamentos**: Usuário, Planta, Perfil

#### 󰳓 Acessar

- **Descrição**: Visualizar ou utilizar um recurso da plataforma.  
- **Impacto**: Garante a navegação entre seções como tutoriais, fóruns e conteúdos personalizados.  
- **Relacionamentos**: Usuário, Recomendação, Fórum

#### 💧 Regar

- **Descrição**: Ação recomendada ao usuário, conforme calendário e tipo de planta.  
- **Impacto**: Ajuda a manter a saúde das plantas e é base para geração de alertas/lembranças no sistema.  
- **Relacionamentos**: Planta, Lembrete

#### 📸 Identificar

- **Descrição**: Detectar espécie por imagem usando modelo de IA.  
- **Impacto**: Reduz barreiras de entrada para iniciantes e aumenta a precisão no cuidado.  
- **Relacionamentos**: Planta, IA, Recomendação

#### 💡 Recomendar

- **Descrição**: Oferecer sugestões automáticas para o usuário com base em suas preferências e histórico.  
- **Impacto**: Personaliza a experiência e aumenta o valor percebido.  
- **Relacionamentos**: Recomendação, IA, Usuário

###  Estados

#### ✅ Cadastrado

- **Descrição**: Status de um item já inserido no sistema.  
- **Impacto**: Permite visualização e edição de dados posteriormente.  
- **Relacionamentos**: Usuário, Planta

#### ⚠️ Esquecido

- **Descrição**: Planta ou tarefa que não recebeu atenção no período estimado.  
- **Impacto**: Dispara lembretes e alertas ao usuário.  
- **Relacionamentos**: Planta, Lembrete

#### 🌿 Saudável

- **Descrição**: Estado da planta ideal, com todos os cuidados em dia.  
- **Impacto**: Usado para avaliar boas práticas e recomendar espécies semelhantes.  
- **Relacionamentos**: Planta, Recomendação

#### ❌ Morta

- **Descrição**: Planta que não sobreviveu, possivelmente por falta de cuidados.  
- **Impacto**: Gera feedback para o sistema recomendar outras espécies mais resilientes.  
- **Relacionamentos**: Planta, Relatório, Recomendação

#### 💤 Inativo

- **Descrição**: Usuário sem interações na plataforma por determinado tempo.  
- **Impacto**: Ações de engajamento podem ser disparadas (notificações, email, etc).  
- **Relacionamentos**: Usuário, Sistema


<font size="3"><p style="text-align: center"><b>Autor:</b>  [Pedro Henrique](https://github.com/PedroHenrique061), 2025</p></font>

## Histórico de Versão
 
 | Versão | Data | Descrição | Autor | 
 | :----: | :--: | :-------: | :---: | 
 | `1.0`| 10/04 | Criação do documento | [Caio Felipe Rocha Rodrigues](https://github.com/caio-felipee) e [Arthur Ribeiro e Sousa](https://github.com/artrsousa1) |  