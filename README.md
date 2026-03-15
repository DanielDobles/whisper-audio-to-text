# Whisper Audio to Text (Kaggle Pro Edition)

Este proyecto contiene un cuaderno de Jupyter diseñado para el procesamiento masivo y robusto de audio en Kaggle, utilizando el modelo **Whisper large-v3**.

## Características Principales
- **Modelo Robustos**: Utiliza `large-v3` para máxima precisión en audios de 3+ horas.
- **Escaneo Recursivo**: Busca automáticamente audios en subcarpetas de `/kaggle/input/datasets/danieldobles/test-whisper`.
- **Lógica Inteligente**: Salta archivos que ya han sido transcritos para ahorrar tiempo en ejecuciones interrumpidas.
- **Formatos Soportados**: `.mp3`, `.wav`, `.m4a`, `.flac`, `.ogg`, `.mp4`.
- **Exportación Dual**: Genera archivos `.txt` y `.md` por cada audio.

## Estructura en Kaggle
- **Entrada**: `/kaggle/input/datasets/danieldobles/test-whisper` (Dataset recursivo).
- **Salida**: `/kaggle/working/transcriptions/` (Aquí aparecerán tus resultados).

## Cómo Usar
1. Sube el archivo `.ipynb` a un Notebook en Kaggle.
2. Ve a **Settings** -> **Accelerator** y selecciona **GPU T4 x2** (o P100).
3. Asegúrate de que el Dataset esté montado en la ruta especificada.
4. Ejecuta todas las celdas.
5. Al finalizar, podrás descargar los archivos desde el panel de **Output** en `/kaggle/working/`.

## Licencia
MIT
