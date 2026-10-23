# Hub de Leitura — Ambiente Docker Compose

Projeto de integração do Hub de Leitura com a suíte de testes de UI, usando Docker Compose para organizar o ambiente de execução.

## Objetivos
- Definir serviços e dependências por meio de Docker Compose.
- Preparar a aplicação e os testes de UI para execução em ambiente integrado.
- Organizar logs e artefatos de execução.

## Tecnologias
- Docker
- Docker Compose
- Hub de Leitura
- Cypress para automação de UI (consulte o projeto de testes integrado)

## Pré-requisitos
- Docker Engine e Docker Compose instalados.
- Git.
- Portas exigidas pelos serviços livres no computador.

## Como executar
1. Clone o repositório e entre na pasta.
2. Revise os serviços, portas, volumes e variáveis em `docker-compose.yml`.
3. Inicie o ambiente:
```bash
docker compose up --build
```
4. Consulte os logs dos serviços e confirme que a aplicação está pronta antes de iniciar os testes.
5. Para encerrar:
```bash
docker compose down
```
A forma de disparar os testes depende dos comandos e serviços definidos no Compose; verifique o arquivo antes de executar.

## Estrutura do projeto
```text
atividade-docker-hub-de-leitura/
├── docker-compose.yml
├── hub-de-leitura-integrado/
├── hub-de-leitura-teste-ui/
├── logs/
└── README.md
```

## Desafios práticos
Integrar aplicação e suíte de testes, configurar a comunicação entre containers e diagnosticar problemas com auxílio dos logs.

## Boas práticas adotadas
- Descrição do ambiente como código.
- Separação entre aplicação integrada e testes de UI.
- Diretório dedicado para logs.

## 📚 Aprendizados
A atividade permite praticar Docker Compose para coordenar serviços e preparar um ambiente integrado para automação. Também reforça a importância de conferir a inicialização da aplicação e consultar logs ao investigar falhas.

## Considerações finais
A estrutura exata dos serviços e o comando para executar os testes dependem do conteúdo de `docker-compose.yml`. Revise as configurações antes da primeira execução.

---

## 🎓 Formação
Atividade desenvolvida durante a formação profissionalizante em **Quality Assurance (QA) pela EBAC — Escola Britânica de Artes Criativas e Tecnologia**.