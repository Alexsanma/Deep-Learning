# Curso IA y Deep Learning

Notebooks y proyectos del curso de Inteligencia Artificial y Deep Learning.

## Requisitos

- Python 3.13

## Crear el entorno

Desde la raíz del proyecto:

```powershell
python -m venv venv
```

### Activar el entorno

```powershell
.\venv\Scripts\Activate.ps1
```

Si PowerShell bloquea la ejecución del script, corre una vez:

```powershell
Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
```

### Instalar las dependencias

```powershell
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### Registrar el kernel en Jupyter (opcional)

```powershell
python -m ipykernel install --user --name=venv-iadl --display-name "Python (IA y DL)"
```

### Abrir los notebooks

```powershell
jupyter lab
```

Selecciona el kernel "Python (IA y DL)" al abrir cualquier `.ipynb`.

## Notas

- `tensorflow` y `opencv-python` son paquetes pesados; la primera instalación puede tardar varios minutos.
- Si tienes GPU NVIDIA y quieres aceleración en Linux/WSL, instala `tensorflow[and-cuda]` en vez de `tensorflow`. En Windows nativo, TensorFlow 2.11+ ya no soporta GPU directamente; usa WSL2 para eso.
