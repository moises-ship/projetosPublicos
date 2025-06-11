📊 Projeto: Extração Automatizada de Dados CNES + Integração com SharePoint
Este projeto realiza a coleta automatizada de dados públicos de estabelecimentos de saúde registrados no CNES (Cadastro Nacional de Estabelecimentos de Saúde), através da API oficial do Ministério da Saúde. A solução foi desenvolvida em Python, com automação de execução e integração via Power Automate Desktop.

🧪 Objetivo
Criar uma rotina automatizada para:

Coletar os dados brutos da API CNES (em formato JSON),

Converter os dados para CSV,

Salvar o arquivo na pasta de Downloads do usuário,

Indexar automaticamente o arquivo em uma biblioteca do SharePoint.

⚙️ Tecnologias utilizadas
🐍 Python (v3.13+)

requests

csv

os

💼 Power Automate Desktop (execução automatizada do script + envio ao SharePoint)

☁️ SharePoint Online (armazenamento do CSV)

🏛️ Fonte dos dados: API pública do CNES - Dados Abertos

📝 Como usar
Instale os requisitos Python:

bash
Copiar
Editar
pip install requests
Execute o script cnes_scraper.py ou configure o Power Automate Desktop para chamá-lo automaticamente.

O arquivo cnes_pad_output.csv será salvo na sua pasta de Downloads.

📌 Observações
O script usa paginação (limit e offset) para coletar todos os registros de forma segura.

A integração com SharePoint foi feita por meio de um fluxo no Power Automate Desktop (não incluído neste repositório por conter configurações locais).

O projeto foi desenvolvido como parte da proposta de participação no edital IPEA/PIPA 032/2025.

