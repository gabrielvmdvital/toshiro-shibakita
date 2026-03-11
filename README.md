Docker: Utilização prática no cenário de Microsserviços
Denilson Bonatti, Instrutor - Digital Innovation One

Muito se tem falado de containers e consequentemente do Docker no ambiente de desenvolvimento. Mas qual a real função de um container no cenários de microsserviços? Qual a real função e quais exemplos práticos podem ser aplicados no dia a dia? Essas são algumas das questões que serão abordadas de forma prática pelo Expert Instructor Denilson Bonatti nesta Live Coding. IMPORTANTE: Agora nossas Live Codings acontecerão no canal oficial da dio._ no YouTube. Então, já corre lá e ative o lembrete! Pré-requisitos: Conhecimentos básicos em Linux, Docker e AWS.

## Como rodar o projeto localmente com Docker Compose

Para subir a infraestrutura completa contendo banco de dados (MySQL), as 3 instâncias da aplicação PHP e o Load Balancer (Nginx), basta executar o seguinte comando a partir da raiz do projeto:

```bash
docker-compose up -d --build
```

A aplicação estará acessível através do endereço `http://localhost:4500`. Você pode verificar no navegador ou fazendo múltiplas chamadas com comando `curl` para conferir o balanceamento de carga entre as máquinas (o registro do `host` mudará entre `app1`, `app2` e `app3`).
