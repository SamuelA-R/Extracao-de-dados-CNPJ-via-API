# Extração de dados CNPJ via API
Esse código irá extrair informações da API da receita federal brasileira, informações como Nome, localização e outras informações.
A versão do Python utilizado foi 3.11.7

**Informações possíveis de serem extraídas:**

- **Status**:
  - `status`: Status da resposta (ex: "OK").

- **Última Atualização**:
  - `ultima_atualizacao`: Data e hora da última atualização.

- **Informações da Empresa**:
  - `cnpj`: Número do CNPJ.
  - `tipo`: Tipo da empresa (ex: MATRIZ).
  - `porte`: Porte da empresa.
  - `nome`: Nome da empresa.
  - `fantasia`: Nome fantasia da empresa.
  - `abertura`: Data de abertura da empresa.

- **Atividades**:
  - `atividade_principal`: Atividade principal da empresa (código e descrição).
  - `atividades_secundarias`: Atividades secundárias da empresa (código e descrição).

- **Informações Jurídicas**:
  - `natureza_juridica`: Natureza jurídica da empresa.

- **Endereço**:
  - `logradouro`: Logradouro da empresa.
  - `numero`: Número do endereço.
  - `complemento`: Complemento do endereço.
  - `cep`: Código postal (CEP).
  - `bairro`: Bairro.
  - `municipio`: Município.
  - `uf`: Unidade Federativa (Estado).

- **Contato**:
  - `email`: Endereço de e-mail.
  - `telefone`: Número de telefone.

- **Situação da Empresa**:
  - `efr`: Informações sobre o EFR (não especificado).
  - `situacao`: Situação atual da empresa.
  - `data_situacao`: Data da situação atual.
  - `motivo_situacao`: Motivo da situação.
  - `situacao_especial`: Situação especial (se houver).
  - `data_situacao_especial`: Data da situação especial.

- **Informações Financeiras**:
  - `capital_social`: Capital social da empresa.

- **Quadro de Sócios e Administradores (QSA)**:
  - `qsa`: Nome, qualificação e país de origem dos sócios ou administradores, e nome e qualificação do representante legal.

- **Optantes pelo Simples Nacional**:
  - `simples`: Se a empresa é optante pelo Simples Nacional, e as datas relacionadas.

- **Optantes pelo MEI (SIMEI)**:
  - `simei`: Se a empresa é optante pelo MEI, e as datas relacionadas.

- **Informações de Faturamento**:
  - `billing`: Se a empresa possui acesso gratuito e está registrada na base de dados.

# Pré-requisitos
Antes de rodas o código, você vai precisar instalar as seguintes bibliotecas: `requests`, `json` e `pandas`.  
Você pode instalar as bibliotecas necessárias utilizando o código **`pip install requests pandas`**.

# Comentário
Esse projeto foi essencial para uma demanda em que precisei corrigir dados inconsistentes, como nomes, nomes fantasia e razão social digitados incorretamente.  
Além disso, ajudou a preencher e corrigir endereços ausentes ou errados, garantindo maior precisão nas análises geoespaciais e melhorando a confiabilidade das informações.  
Espero que também seja útil para você!

---

📌 **Para eventuais dúvidas, conecte-se comigo no LinkedIn:**  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/samuel-alves-ribeiro-017960246/)
