# Testes-C2
Testes Para estudar Convergência de Séries e sequencias 
# 📌 Teste da Série Alternada  

Considere uma série da forma:

\[
\sum_{n=1}^{\infty} (-1)^{n-1} b_n = b_1 - b_2 + b_3 - b_4 + b_5 - \dots
\]

onde  

\[
b_n > 0 \quad \text{para todo } n.
\]

Essa série é chamada de *série alternada, pois seus termos mudam de sinal sucessivamente (positivo, negativo, positivo, negativo...*).

---

## ✅ Condições do Teste da Série Alternada  

A série 

\[
\sum_{n=1}^{\infty} (-1)^{n-1} b_n
\]

*converge* se forem satisfeitas as duas condições:

1. *Decrescimento dos termos*  
   \[
   b_{n} \geq b_{n+1}, \quad \forall n \in \mathbb{N}
   \]  
   A sequência \((b_n)\) deve ser *monótona decrescente*.

2. *Limite dos termos nulos*  
   \[
   \lim_{n \to \infty} b_n = 0
   \]

---

## 💡 Observações Importantes  

- O teste *não exige convergência absoluta*.  
- Se a série alternada converge, mas \(\sum b_n\) diverge, então a série é chamada de *condicionalmente convergente*.  
- Se também \(\sum b_n\) converge, a série é *absolutamente convergente*.  

---

## 📘 Exemplo Clássico  

A série harmônica alternada:  

\[
\sum_{n=1}^{\infty} \frac{(-1)^{n-1}}{n} = 1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \dots
\]

- Atende às condições do teste:  
  - \( \frac{1}{n} \) é decrescente.  
  - \( \lim_{n \to \infty} \frac{1}{n} = 0 \).  

✅ Logo, a série *converge*.

---

## 🔎 Resumo Visual  

```mermaid
graph TD
    A["Série Alternada ∑ (-1)^(n-1) bₙ"] --> B["1. bₙ decrescente? (bₙ ≥ bₙ₊₁)"]
    B -->|Não| D["❌ Diverge ou não é garantido"]
    B -->|Sim| C["2. lim (n→∞) bₙ = 0?"]
    C -->|Não| D
    C -->|Sim| E["✅ Converge (pelo Teste da Série Alternada)"]
