# WebScraping - Cotação

### Resumo:
Um projeto desenvolvimento com o Python que visa a coleta da cotação atual do dólar, euro e ouro e atualiza uma base de dados com a nova cotação.

---

## Desafio inspirado:

Uma empresa que atua no setor de importação tem como os preços dos produtos vinculado à cotação do:
- Dólar;
- Euro;
- Ouro.

É necessário coletar na internet de forma automática a cotação desses 3 itens e saber quanto devemos cobrar pelo nossos produtos, considerando uma margem de contribuição que temos na nossa base de dados.

---

### Funcionamento:

1. Realiza a coleta das três cotações e salva cada individualmente em uma variável

2. Importa a base de dados

 Produtos | Preço Original | Moeda | Cotação | Preço de Compra | Margem | Preço de Venda
  --- | --- | --- | --- | --- | ---| ---
 Câmera Canon | 999,99 | Dólar | 5 | 4999,95 | 1,4 | 6999,93
 Carro Renault | 4500 | Euro | 6 | 27000 | 2 | 54000
Notebook Dell | 899,99 | Dólar | 5 | 4499,95 | 1,7 | 7649,915
IPhone | 799 | Dólar | 5 | 3995 | 1,7 | 6791,5
Joia 20g | 20 | Ouro | 350 | 7000 | 1,15 | 8050
  --- | --- | --- | --- | --- | ---| ---


3. Atualiza as colunas **Cotação**, **Preço de Compra**, **Margem** e **Preço de Venda**:

    Data das cotações: **20/01/2023 14:00:13**

Produtos | Preço Original | Moeda | Cotação | Preço de Compra | Margem | Preço de Venda
  --- | --- | --- | --- | --- | ---| ---
Câmera Canon | 999,99 | Dólar | 5,2103 | 5210,247897 | 1,4 | 7294,347056
Carro Renault | 4500 | Euro | 5,64327593 | 25394,74169 | 2 | 50789,48337
Notebook Dell | 899,99 | Dólar | 5,2103 | 4689,217897 | 1,7 | 7971,670425
IPhone | 799 | Dólar | 5,2103 | 4163,0297 | 1,7 | 7077,15049
Joia 20g | 20 | Ouro | 322,63 | 6452,6 | 1,15 | 7420,49
--- | --- | --- | --- | --- | ---| ---

4. Exporta a planilha (nomeada com a data atual)

    Exemplo: `Produtos_atualizados_20-1-2023-14-0-13.xlsx`

---

## Utilização do programa

### 1. Instalamento dos requisitos

```
pip install -r requirements.txt
```

### 2. Execute o arquivo `main.ipynb`
Obs: preferencialmente com o Jupyter Notebook.


## Aviso:

É necessário que os arquivos `main.ipynb` e `Produtos.xlsx` estejam no mesmo diretório.

