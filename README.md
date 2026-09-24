# Aula-1---COMP.NUV

## Aula-1---Computação-em-Nuvem-Conceitos-Básicos
Este repositório tem como objetivo documentar as atividades práticas e reflexões propostas na disciplina de Computação em Nuvem, servindo como registro de aprendizado e evidência das práticas realizadas em laboratório. Sinta-se à vontade para explorar os arquivos e acompanhar a evolução dos conceitos ao longo do semestre.

O que foi proposto em aula
A primeira aula teve como foco apresentar a disciplina e introduzir os Conceitos Básicos em Computação em Nuvem, mostrando como a migração para a nuvem está transformando a forma como trabalhamos, nos comunicamos e colaboramos.

Atividade Prática — Nosso Primeiro Ambiente Remoto
Vamos utilizar um computador que não está no nosso computador! Nesta atividade utilizaremos o Killercoda, uma plataforma que disponibiliza ambientes Linux interativos diretamente pelo navegador.

Objetivo da atividade: compreender, na prática, como podemos utilizar recursos computacionais remotos por meio da Internet.

Ambiente: Killercoda
Plataforma: Killercoda (gratuito, navegador, sem instalação local)

Sistema Operacional do ambiente: Ubuntu 24.04

Acesso: https://killercoda.com/learn

Ambiente Ubuntu Linux Playground: https://killercoda.com/playgrounds/scenario/ubuntu

⚠️ Importante: O ambiente do Killercoda utilizado nesta prática é baseado no Ubuntu 24.04. O ambiente é temporário e executado remotamente. Na modalidade gratuita, uma sessão pode durar no máximo 1 hora; ao final, o ambiente é eliminado.

Passo 1: Acessar o Killercoda
Abra o navegador

Acesse https://killercoda.com/learn

Clique em Login / Sign Up

Caso ainda não possua uma conta, faça o cadastro gratuito

Após entrar, acesse o ambiente Ubuntu Linux Playground

Utilizaremos somente os recursos gratuitos da plataforma

Passo 2: Abrir o Ubuntu Linux
Acesse diretamente: https://killercoda.com/playgrounds/scenario/ubuntu

Abra o link

Caso solicitado, faça login

Inicie o ambiente

Aguarde alguns segundos enquanto o ambiente Linux é preparado

Um terminal aparecerá no navegador

O que acabou de acontecer? Seu computador → Internet → Killercoda → disponibiliza um ambiente computacional Linux Ubuntu remoto. O terminal no navegador permite executar comandos em um ambiente Linux sem instalar esse sistema operacional no computador utilizado na aula.

Passo 3: Quem sou eu?
bash
whoami
Mostra qual usuário está executando os comandos naquele ambiente Linux.

bash
hostname
Mostra o nome atribuído à máquina.

Passo 4: Qual sistema estamos utilizando?
bash
uname -a
Apresenta informações sobre o sistema Linux em execução.

bash
cat /etc/os-release
Mostra informações relacionadas ao sistema operacional utilizado pelo ambiente.

Pergunta: O Ubuntu está instalado no computador do laboratório? → Não. Estamos interagindo com um ambiente Linux disponibilizado remotamente pelo Killercoda.

Passo 5: Onde estamos?
bash
pwd
Print Working Directory — mostra em qual diretório do sistema estamos.

bash
ls
Mostra os arquivos e diretórios existentes no local atual.

Até agora conseguimos:

Identificar o usuário

Identificar a máquina

Verificar o sistema operacional

Descobrir onde estamos

Visualizar arquivos

Tudo utilizando um ambiente remoto acessado pelo navegador.

Passo 6: Vamos criar nosso espaço de trabalho
bash
mkdir computacao-nuvem
cd computacao-nuvem
pwd
mkdir criou um novo diretório

cd permitiu entrar nesse diretório

bash
ls
A pasta ainda deverá estar vazia.

Passo 7: Criando nosso primeiro arquivo
bash
echo "Minha primeira atividade de Computacao em Nuvem" > mensagem.txt
ls
Deverá existir: mensagem.txt. Acabamos de criar um arquivo dentro do ambiente Linux que estamos utilizando remotamente.

Passo 8: Lendo o arquivo
bash
cat mensagem.txt
O terminal deverá apresentar:

text
Minha primeira atividade de Computacao em Nuvem
O arquivo foi criado no ambiente remoto — não em uma pasta comum do computador que você está usando.

Passo 9: Vamos adicionar informações
bash
echo "Estou utilizando um ambiente Linux remoto." >> mensagem.txt
echo "O acesso esta sendo realizado pelo navegador." >> mensagem.txt
cat mensagem.txt
O arquivo deverá apresentar três linhas.

Atenção aos operadores:

> cria/substitui o conteúdo

>> acrescenta conteúdo ao final do arquivo

Passo 10: Vamos investigar a máquina
bash
hostname    # identificação da máquina
nproc       # quantidade de CPUs disponíveis
free -h     # memória disponível
df -h       # espaço de armazenamento
Agora temos evidências de que o ambiente remoto possui recursos computacionais.
