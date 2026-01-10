# Roteiro para Calcular Limites de Sequências

---

### Passo 1: Identifique o tipo da sequência
Observe a forma de aₙ:

1. **Frações de polinômios:** aₙ = P(n) / Q(n)
2. **Com raízes ou radicais:** aₙ = ⁿ√(f(n)) ou aₙ = √(n² + ...) - n
3. **Alternantes:** aₙ = (-1)ⁿ × f(n)
4. **Exponenciais / logaritmos / fatoriais:** (1 + 1/n)ⁿ, ln(n)/n, etc.

---

### Passo 2: Observe o comportamento quando n → ∞

- **Frações de polinômios:** compare os graus do numerador e denominador:

| Grau do numerador < grau do denominador | Limite |
|---------------------------------------|-------|
| menor                                 | 0     |
| igual                                 | razão dos coeficientes principais |
| maior                                 | +∞ ou -∞ |

- **Sequências com raiz:** tente fatorar ou racionalizar.
  - Ex.: √(n² + 1) - n = 1 / (√(n² + 1) + n) → 0

- **Sequências alternantes:** observe |aₙ|. Se |aₙ| → 0, a sequência converge; caso contrário, pode divergir oscilando.

- **Exponenciais / logaritmos:** use limites conhecidos, regra de l’Hôpital ou propriedades de e.

---

### Passo 3: Simplifique a expressão, se necessário

- Divida numerador e denominador pelo maior grau de n
- Racionalize raízes
- Separe módulo e sinal em alternantes

---

### Passo 4: Determine N(ε) se quiser formalizar

- Dado ε > 0, encontre N tal que, para todo n ≥ N:

|aₙ - L| < ε

- Isso serve para provar formalmente a convergência da sequência.

---

### Passo 5: Conclua o limite

- Se todos os passos mostram que |aₙ - L| pode ser tornado arbitrariamente pequeno: **sequência convergente** → limite L
- Caso contrário: **sequência divergente** (pode ser infinita ou oscilante)

---

💡 **Exemplo rápido:**

aₙ = (3n² + 5) / (6n² - 4n + 1)

1. Tipo: fração de polinômios
2. Grau numerador = 2, grau denominador = 2 → igual grau
3. Limite = razão dos coeficientes principais → 3/6 = 1/2
4. Sequência convergente: limite = 1/2