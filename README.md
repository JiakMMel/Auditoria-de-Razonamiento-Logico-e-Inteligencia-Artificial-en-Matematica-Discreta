# Auditoría de Razonamiento Lógico e Inteligencia Artificial en Matemática Discreta

Proyecto integrador de Matemática Discreta para CC. Se revisan las respuestas de tres modelos de IA (Gemini, ChatGPT y Qwen) a cinco problemas de demostración, funciones y relaciones, y a un problema bonus de combinatoria, y se analizan sus errores.

## Contenido

- `informe/`: reporte final en LaTeX (`reporte.tex`) y su PDF.
- `logs/`: transcripciones de los chats con los modelos y capturas de pantalla de las repreguntas.
- `assets/`: archivos de apoyo del proyecto.
- `registro_auditoria.md`: registro de cada interacción con los modelos (prompt, resultado, categoría y observaciones) y métricas resumen.

## Resultado principal

Los modelos resolvieron bien los ejercicios típicos y se corrigieron cuando se les señaló el error exacto, pero cometieron pasos circulares, omitieron condiciones del dominio y, en un caso, llegaron a la respuesta correcta con un razonamiento inválido. Un mismo modelo (Qwen) dio resultados distintos en dos ejecuciones del mismo problema.

## Compilar el reporte

`reporte.tex` usa la clase `IEEEtran`. La forma más simple es subirlo a Overleaf y compilar. En local: `pdflatex reporte.tex` dos veces, con `IEEEtran` (`texlive-publishers` en Arch Linux) y `babel` en español (`texlive-langextra`).
