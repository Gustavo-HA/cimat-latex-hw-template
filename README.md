# 📋 Plantilla para Tareas de Cómputo Estadístico - CIMAT

Esta es una plantilla completa para trabajos académicos con R y LaTeX, optimizada para el Centro de Investigación en Matemáticas (CIMAT).

## 📁 Archivos Esenciales para la Plantilla

### 🔴 Criticos
```
tarea_plantilla.Rtex       # Documento principal (LaTeX + R)
cimat-logo.png            # Logo institucional
compile_fast.sh           # Script de compilación optimizada
bib.bib                   # Referencias bibliográficas
```

### 🟡 Recomendados
```
latexmkrc                 # Configuración para latexmk
```

### 🟢 Opcionales
```
algorithm.sty             # Para algoritmos (si se usan)
algorithmic.sty           # Para pseudocódigo (si se usa)
IEEEtran.cls             # Clase IEEE (si se necesita)
```

## **Personalización**
Editar en `mi-documento.Rtex`:
- **Título**: Líneas 133-138
- **Autor**: Línea 142
- **Fecha**: Línea 144
- **Contenido**: Reemplazar problemas existentes


## 🛠️ Estructura de un Problema

```latex
%%%%%%%%%%% PROBLEMA X %%%%%%%%%%%
\begin{problem}{Título del Problema}
Enunciado del problema...
\end{problem}

\subsection{\textbf{Solución:}}

Explicación teórica...

<<chunk-name>>=
# Código R
datos <- c(1, 2, 3)
modelo <- lm(y ~ x, data = datos)
summary(modelo)
@

Interpretación de resultados...

\newpage
```

## 🔧 Configuraciones Importantes

### En el documento `.Rtex`:
```latex
cache = TRUE                    # Acelera recompilación
fig.path = 'figure/'           # Organiza figuras
spanish babel                  # Idioma español
CIMAT styling                  # Colores y formato institucional
```


## 📚 Recursos Adicionales

- [Chunck options](https://yihui.org/knitr/](https://yihui.org/knitr/options/): Importantes para obtener el resultado deseado en cada celda de código.

---
*Plantilla creada para CIMAT - Cómputo Estadístico*
