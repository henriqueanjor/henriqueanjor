<h1 align="center">Luiz Henrique dos Anjos Rodrigues</h1>

<p align="center">
  <b>Desenvolvedor Back-end · Java · AWS · Infraestrutura e Redes</b><br/>
  3 anos de experiência em tecnologia no geral, tanto em desenvolvimento como assistencia de TI · Recife, PE
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/luiz-henrique-409604225/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="mailto:ldl.anjos228.lha@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
</p>

---

## Sobre

A maioria dos desenvolvedores nunca configurou uma rota. Eu passei um ano configurando PPPoE, endereçamento IP e diagnosticando falhas de conexão de assinantes reais — e dois anos antes disso escrevendo código que rodava em produção.

**Connect (2023–2025), desenvolvedor CLT.** Equipe de 3 pessoas responsável pelo aplicativo iOS e pelo site da empresa: telas em Swift/UIKit, integração com APIs REST internas, correção de bugs reportados por usuários e apoio à operação em AWS (EC2 e S3).

**Suporte técnico N1/N2 (jun/2025–jun/2026), remoto.** Assinantes de banda larga sob metas de SLA: configuração de CPE, PPPoE, Wi-Fi, diagnóstico de conectividade e abertura de ordens de serviço.

Hoje meu foco é **back-end em Java com Spring Boot**. Em paralelo, trabalho com visão computacional — e com um tipo de problema que aparece bastante nos meus projetos: fazer software rodar em hardware que não foi feito pra ele.

📫 ldl.anjos228.lha@gmail.com

---

## Stack

**Uso no dia a dia**

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,python,mysql,git,github,linux" />
</p>

`Java` · `Python` · `API REST` · `SQL / MySQL` · `AWS (EC2, S3)` · `Linux` · `Git`

**Também trabalhei com**

`Swift / UIKit` · `PHP` · `JavaScript` · `C++` · `SQLite`

**Estudando agora**

`Spring Boot` · `Docker` · `PostgreSQL`

---

# Projetos

## Inferência YOLO acelerada por GPU em hardware AMD

Detecção de objetos em tempo real rodando com aceleração por GPU em placa AMD.

**O problema:** praticamente todo o ecossistema de deep learning assume NVIDIA e CUDA. Em hardware AMD o caminho padrão não funciona, e a alternativa comum é cair para CPU, com perda severa de desempenho.

**A solução:** exportar o modelo YOLO para o formato ONNX e executá-lo via ONNX Runtime com o *execution provider* DirectML, que expõe a GPU AMD através da API do DirectX.

- Exportação e validação do grafo ONNX, verificando compatibilidade de operadores com o execution provider
- Pipeline de inferência mantendo os tensores residentes em VRAM entre frames, evitando cópias entre memória de sistema e GPU
- Pré-processamento próprio: letterbox resize e normalização, alinhados ao formato de entrada do modelo exportado
- Pós-processamento com decodificação das saídas e non-maximum suppression (NMS)
- Captura e exibição em tempo real com OpenCV

`Python` · `ONNX Runtime` · `DirectML` · `OpenCV` · `YOLO`

---

## API REST de Ordens de Serviço — *em construção*

API para gestão de chamados técnicos de provedor de internet, modelada a partir do fluxo que eu operava no suporte: cliente, chamado, prioridade, status e técnico responsável.

- Arquitetura em camadas: controller, service e repositório
- Persistência relacional com JPA
- Injeção de dependência e validação de entrada
- Tratamento centralizado de erros com respostas HTTP consistentes

`Java` · `Spring Boot` · `MySQL`

---

## Ryzentosh — macOS em hardware AMD Ryzen

Instalação e configuração completa do macOS em hardware não suportado, via OpenCore.

- Configuração do bootloader e da ACPI, com patches para compatibilidade da plataforma AMD
- Resolução de incompatibilidades de kernel e drivers
- Diagnóstico de falhas de inicialização a partir de logs de boot

`OpenCore` · `macOS` · `ACPI` · `Hardware`

---

## Motor de Xadrez com integração ao Stockfish

Cliente de xadrez com análise de partidas em tempo real.

- Comunicação bidirecional via subprocesso com o Stockfish usando o protocolo UCI
- Envio assíncrono de comandos, mantendo a interface responsiva durante a análise
- Validação de jogadas incluindo casos especiais: roque, en passant e promoção de peão
- Controle de nível de dificuldade

`Python` · `Stockfish` · `UCI`

---

## Open Finance — Agregação de APIs Financeiras

Camada de agregação que consome múltiplas APIs públicas e unifica os dados.

- Normalização de esquemas heterogêneos em um único modelo de dados
- Tratamento de erros com retry e fallback para timeouts e indisponibilidade de serviço
- Autenticação e organização modular

`Java` · `PHP` · `APIs REST` · `MySQL`

---

## Sistema Web de Adoção de Pets

Sistema full-stack desenvolvido em equipe, com controle de acesso por perfil.

- Autenticação separada para usuário e administrador
- CRUD completo com consultas parametrizadas, prevenindo SQL injection
- Filtros por espécie, porte e gênero

`PHP` · `MySQL` · `HTML` · `CSS` · `JavaScript`

---

## Formação

**Bacharelado em Ciência da Computação** — Universidade Católica de Pernambuco (UNICAP)  
Previsão de conclusão: 2029

**Certificações**
- CS50x: Introduction to Computer Science — Harvard University (edX)
- CS50 AI: Introduction to Artificial Intelligence with Python — Harvard University (edX)
- Especialização em Inteligência Artificial Generativa
