
DVH Web – Instrucciones rápidas

1) Requisitos
- Tener Python 3.9+ instalado.

2) Crear entorno e instalar dependencias
Windows (PowerShell):
  python -m venv dvhenv
  .\dvhenv\Scripts\Activate.ps1
  pip install -r requirements.txt

Linux/Mac:
  python -m venv dvhenv
  source dvhenv/bin/activate
  pip install -r requirements.txt

3) Ejecutar
  python app.py

4) Abrir en el navegador
  - En tu PC: http://localhost:5000
  - En otra PC de la misma red: http://IP_DE_TU_PC:5000
    (si no abre, permitir el puerto 5000 en el firewall).

Formato DVH esperado
- Columnas típicas: "Dose (Gy)" y "Volume (cc)" o "Volume (%)".
- Si los nombres difieren, podés mapearlos en el formulario.

Notas
- Si tu DVH está en %, para D2cc indicá el volumen total (cc) del ROI.
- El archivo de salida se descarga en CSV con las métricas calculadas.
