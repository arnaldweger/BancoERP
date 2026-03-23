🏦 BancoERP — Conciliação Bancária Automatizada

Aplicação desktop desenvolvida em Python para automatizar a conciliação entre extratos bancários e lançamentos do sistema ERP, eliminando o trabalho manual de conferência planilha por planilha.


🎯 Problema que resolve
Em ambientes hospitalares e empresariais, a conciliação bancária é feita manualmente: o analista financeiro baixa o extrato do banco, abre o ERP, e compara linha a linha os lançamentos. Esse processo consome horas por semana e está sujeito a erros humanos.
O BancoERP automatiza essa comparação em segundos.

⚙️ Como funciona

O usuário importa o extrato bancário (CSV ou XLSX)
O usuário importa o relatório de lançamentos do ERP (Tasy ou similar)
A aplicação cruza os dados automaticamente por valor, data e histórico
O resultado é exibido em um dashboard interativo com:

✅ Itens conciliados
⚠️ Itens pendentes / divergências
📊 Resumo por período




🛠️ Tecnologias utilizadas
TecnologiaUsoPython 3.xLinguagem principalPandasLeitura, tratamento e cruzamento de dadosStreamlitInterface web interativaOpenPyXLLeitura e escrita de arquivos ExcelMatplotlib / PlotlyVisualização dos resultadosNuitkaEmpacotamento em .exe para uso corporativo

🚀 Como executar
Pré-requisitos
bashpip install -r requirements.txt
Rodar a aplicação
bashstreamlit run app.py
Acesse em http://localhost:8501

📁 Estrutura do projeto
BancoERP/
├── app.py                  # Interface Streamlit (ponto de entrada)
├── conciliacao.py          # Lógica de cruzamento de dados
├── utils/
│   ├── leitura_banco.py    # Leitura e padronização do extrato bancário
│   └── leitura_erp.py      # Leitura e padronização do relatório ERP
├── data/
│   └── exemplos/           # Arquivos de exemplo para testes
├── requirements.txt
└── README.md

📸 Screenshots

Interface do dashboard com resultado da conciliação e indicadores de pendências.

(Em breve — adicionar prints da aplicação em uso)

💡 Contexto real de aplicação
Este projeto foi desenvolvido a partir de uma necessidade real identificada durante a atuação como Auxiliar de Operações Financeiras no Hospital São Camilo SP, onde o processo de conciliação de recebimentos de cartão era 100% manual.
A ferramenta foi implementada internamente e passou a ser utilizada pela equipe de tesouraria, reduzindo significativamente o tempo dedicado a essa atividade.

🔗 Outros projetos de automação do mesmo contexto
Este projeto faz parte de um conjunto de automações desenvolvidas para o setor de planejamento hospitalar:
ProjetoDescriçãoBancoERP (este)Conciliação bancária entre extrato do banco e ERPPedidosGTPlanConverte planilha de planejamento em CSV integrado ao GTPlan para pedidos em massaFollowUp FornecedoresEnvio automático de e-mails de cobrança para pendências com fornecedores

📬 Contato
Arnald Weger
🔗 LinkedIn
📧 arnaldweger@gmail.com
📍 São Paulo, SP — Disponível para trabalho remoto
