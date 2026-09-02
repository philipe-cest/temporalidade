# Transformações Temporais (n) & Equivalência em Matemática Financeira

Material didático de apoio para a disciplina de **Matemática Financeira** do curso de Bacharelado em Administração do **CEST — Centro Universitário Santa Terezinha**, elaborado pelo **Prof. Msc. Philipe Sampaio Lima**.

---

## 1. O Axioma da Homogeneidade Periódica

Em Matemática Financeira e Engenharia Econômica, vigora uma regra fundamental: **a taxa de juros ($i$) e o tempo ($n$) devem estar estritamente referenciados à mesma unidade periódica**.

$$\text{Montante Composto: } FV = PV \cdot (1 + i)^n$$

* Se a taxa for anual ($i \text{ a.a.}$), o período $n$ deve ser expresso em **anos**.
* Se a taxa for mensal ($i \text{ a.m.}$), o período $n$ deve ser expresso em **meses**.
* Se a taxa for diária ($i \text{ a.d.}$), o período $n$ deve ser expresso em **dias**.

---

## 2. Convenções Temporais de Mercado

O cálculo de prazos pode adotar duas premissas centrais no sistema financeiro:

* **Convenção Comercial (Ordinária):** Considera todos os meses com 30 dias e o ano com 360 dias ($12 \times 30$). É o padrão amplamente adotado em operações de crédito bancário, desconto de duplicatas e financiamentos de curto/médio prazo.
* **Convenção Exata (Civil):** Considera o calendário astronômico real, com meses de 28, 29, 30 ou 31 dias e o ano com 365 dias (ou 366 em anos bissextos). Comum em títulos da dívida pública, operações cambiais e comércio exterior.

---

## 3. Matriz de Conversão entre Unidades de Tempo

A tabela a seguir apresenta os fatores de conversão baseados no ano comercial (360 dias) e mês comercial (30 dias):

| Unidade de Entrada | Equivalência em Dias | Equivalência em Meses | Fração do Ano |
| --- | --- | --- | --- |
| **1 Dia** | $1$ | $\frac{1}{30} \approx 0{,}0333$ | $\frac{1}{360} \approx 0{,}002778$ |
| **1 Mês** | $30$ | $1$ | $\frac{1}{12} \approx 0{,}083333$ |
| **1 Bimestre** | $60$ | $2$ | $\frac{2}{12} = \frac{1}{6} \approx 0{,}1667$ |
| **1 Trimestre** | $90$ | $3$ | $\frac{3}{12} = \frac{1}{4} = 0{,}25$ |
| **1 Semestre** | $180$ | $6$ | $\frac{6}{12} = \frac{1}{2} = 0{,}50$ |
| **1 Ano** | $360$ | $12$ | $1{,}00$ |

---

## 4. O Expoente Fracionário nos Juros Compostos

Ao contrário do regime de juros simples (onde a conversão opera de forma puramente linear), no regime de juros compostos a equivalência de tempo incide sobre o expoente. O regime exponencial aceita números reais fracionários para o cálculo de juros intermediários (*pro-rata die*):

$$n = \frac{\text{Tempo total decorrido na unidade original}}{\text{Extensão temporal da unidade da taxa}}$$

### Exemplo Prático de Compatibilização:

* **Capital Inicial ($PV$):** R$ 10.000,00
* **Taxa de Juros ($i$):** 12% ao ano ($i = 0{,}12\text{ a.a.}$)
* **Prazo da Operação:** 45 dias comerciais

**Passo 1 — Conversão do prazo para anos:**


$$n = \frac{45}{360} = 0{,}125\text{ ano}$$

**Passo 2 — Resolução do montante:**


$$FV = 10.000 \cdot (1 + 0{,}12)^{0{,}125}$$

$$FV = 10.000 \cdot 1{,}014467 = \text{R\$ } 10.144{,}67$$

---

## 5. Isolamento de Prazo ($n$) via Logaritmos

Quando os valores presente ($PV$), futuro ($FV$) e a taxa periódica ($i$) são conhecidos e deseja-se encontrar a duração exata da operação, isola-se $n$ aplicando-se o logaritmo natural ($\ln$):

$$FV = PV \cdot (1 + i)^n \implies \frac{FV}{PV} = (1 + i)^n$$

$$\ln\left(\frac{FV}{PV}\right) = n \cdot \ln(1 + i)$$

$$n = \frac{\ln(FV / PV)}{\ln(1 + i)}$$

O resultado obtido para $n$ sairá rigorosamente na mesma unidade periódica em que a taxa $i$ estiver expressa.
