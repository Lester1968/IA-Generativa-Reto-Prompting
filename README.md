# ✍️ Reto 2 – Mejorando la Comunicación con un LLM mediante Prompting

**Curso:** Usos Profesionales de la IA Generativa – IBM SkillsBuild (2025)  
**Autor:** Lester Dávila

---

## 🎯 Objetivo

Explorar cómo la formulación del prompt afecta la precisión, claridad y calidad de las respuestas generadas por un Large Language Model (LLM). Se aplica la técnica **Chain of Thought Prompting** para transformar un ejemplo ambiguo en una consulta clara y lógica.

---

## 🔍 Análisis del Prompt Inicial

### ❌ Prompt Zero-Shot

> “Calcula cuántas frutas hay en total: Tengo 3 manzanas y compro 2 cajas de peras con 4 peras cada una.”

### 🔎 Posibles fallos:

- No induce razonamiento paso a paso.
- Puede omitir multiplicación implícita.
- Riesgo de alucinación por ambigüedad.

👉 Los LLMs predicen texto, no "razonan" como humanos. Si no se guía su estructura, puede fallar el cálculo.

---

## 🛠️ Técnica aplicada: Chain of Thought Prompting (CoT)

La técnica **Chain of Thought (Cadena de Pensamiento)** instruye explícitamente al modelo para **razonar paso a paso**, ideal en tareas que requieren lógica, explicación o precisión matemática.

---

## ✅ Prompt Mejorado (CoT)

> “Calcula cuántas frutas hay en total. Razona paso a paso antes de dar la respuesta final.  
Tengo 3 manzanas y compro 2 cajas de peras. Cada caja tiene 4 peras.”

---

## 📈 Comparación de enfoques

| Criterio                   | Zero-Shot Prompt                     | Prompt con CoT                        |
|---------------------------|--------------------------------------|---------------------------------------|
| Razonamiento inducido     | No                                   | Sí (paso a paso)                      |
| Interpretación numérica   | Implícita                            | Explícita                             |
| Transparencia de lógica   | Baja                                 | Alta                                  |
| Riesgo de error o invención| Alto                                 | Bajo                                  |

---

## 🧩 Resultado Esperado del LLM

```
Paso 1: Tengo 3 manzanas.  
Paso 2: Compro 2 cajas de peras.  
Paso 3: Cada caja tiene 4 peras → 2 × 4 = 8 peras.  
Paso 4: Total = 3 + 8 = **11 frutas**
```

---

## 🧠 Conclusión

Este reto demuestra que una estrategia de prompting bien aplicada puede transformar la calidad de las respuestas de un LLM. La técnica **Chain of Thought**:
- Mejora la precisión del modelo.
- Aumenta la claridad explicativa.
- Reduce alucinaciones y ambigüedad.

> En contextos profesionales, esta técnica es clave para usar la IA de forma segura, comprensible y eficiente.

---

## 👨‍💻 Autor
**Lester Dávila**  
Participante del curso "IA Generativa – IBM SkillsBuild", módulo de prompting (junio 2025).

## 📄 Licencia
Este proyecto está licenciado bajo la Licencia MIT.  
Consulta el archivo [LICENSE](LICENSE) para más detalles.
