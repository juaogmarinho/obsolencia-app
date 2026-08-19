# Controle de Notebooks

Aplicação web para gestão de notebooks corporativos, controle de substituição, acompanhamento de status e visualização de indicadores operacionais.

## Visão geral

Este projeto foi desenvolvido para facilitar o controle de ativos de TI em empresas, permitindo registrar notebooks por colaborador, acompanhar status de troca, visualizar prioridade, importar/exportar dados e monitorar o cenário por dashboard.

A aplicação funciona em navegador, sem necessidade de backend, armazenando os dados localmente no navegador via `localStorage` para uso rápido e prático.

## Funcionalidades

- Cadastro de notebooks com dados do colaborador, patrimônio, modelo, hostname, empresa, departamento e observações
- Controle de status de notebook:
  - Ativo
  - Aguardando substituição
  - Compra aprovada
  - Novo notebook enviado
  - Troca concluída
- Classificação por prioridade:
  - Alta
  - Média
  - Baixa
- Busca por colaborador, patrimônio, modelo, hostname e empresa
- Filtros por status e prioridade
- Ordenação por colunas da tabela
- Paginação configurável
- Dashboard com estatísticas por departamento, empresa e status
- Importação de dados em Excel (`.xlsx` / `.xls`)
- Importação de backup em JSON
- Exportação para CSV
- Exportação para backup em JSON
- Download de template de Excel
- Persistência de dados no navegador

## Stack tecnológico

- HTML5
- CSS3
- JavaScript puro
- Chart.js
- SheetJS (`xlsx.full.min.js`)

## Estrutura do projeto

```text
obsolencia-app/
├── notebooks-app.html   # Aplicação principal
├── xlsx.full.min.js     # Biblioteca responsável pela leitura/exportação de Excel
├── README.md            # Documentação do projeto
└── .git                 # Git do repositório
```

## Como executar

1. Faça o download ou clone este repositório.
2. Abra o arquivo `notebooks-app.html` em um navegador.
3. A aplicação já estará disponível para uso.

> Como a solução foi construída em front-end puro, não há necessidade de instalar dependências ou subir um servidor local.

## Como usar

### Cadastro

- Clique em `+ Novo notebook`.
- Preencha os dados do colaborador e do equipamento.
- Salve o registro.

### Filtros e busca

- Use o campo de busca para localizar notebooks por colaborador, patrimônio, modelo ou hostname.
- Filtre por status e prioridade.
- Ajuste a quantidade de registros por página conforme sua necessidade.

### Importação e exportação

- `Importar Excel`: carrega dados em planilha para inserir registros no sistema.
- `Importar JSON`: restaura um backup feito anteriormente.
- `CSV`: exporta os dados em formato CSV.
- `Backup`: exporta os dados em JSON.
- `Template`: baixa um modelo para preenchimento.

### Dashboard

- Acesse o painel de indicadores para verificar:
  - notebooks por departamento
  - status atual da frota
  - distribuição por empresa/vínculo

## Observações importantes

- Os dados são armazenados no `localStorage` do navegador.
- Se o histórico do navegador for limpo, os registros podem ser apagados.
- Para manter uma cópia segura, utilize a função de exportação em JSON ou CSV.

## Status do projeto

Projeto em funcionamento e com interface voltada para uso interno de gestão de TI e ativos corporativos.

## Possíveis evoluções futuras

- autenticação de usuários
- integração com banco de dados
- sincronização entre múltiplos usuários
- geração de relatórios PDF
- paginação avançada e filtros mais robustos
- histórico de alterações por registro

## Licença

Este projeto foi desenvolvido para uso interno e apresentação de portfólio/projeto pessoal. Caso queira reutilizar, fique à vontade para adaptar conforme a necessidade.

## Autor

Desenvolvido para gestão operacional de notebooks e ativos de TI.
