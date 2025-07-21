# Modelo-predictivo-GRD
Predicción de GRD código equivalente al gold standar con el que se creó la base de datos de un hospital 

Manual de Usuario - Proyecto GRD (Grupo Relacionado por Diagnóstico)

Este manual tiene como propósito guiar paso a paso la descarga, instalación y ejecución del sistema de predicción de GRD desarrollado en Django y TensorFlow.

# 1. Requisitos previos

Antes de iniciar, asegúrate de tener instalado en tu equipo:

Python 3.8 y 3.11

Git (opcional, para clonar el repositorio)

Visual Studio Code o cualquier editor de código

# 2. Descarga del proyecto

Puedes obtener los archivos del proyecto desde el repositorio o mediante un archivo comprimido. Una vez descargado:

Extrae el contenido en una carpeta local.

Abre una terminal de PowerShell (o VSCode) y navega hasta la carpeta del proyecto.

# 3. Activación del entorno y ejecución

a) Activar entorno:
.\venv\Scripts\Activate.ps1

b) Ir al proyecto Django:
cd proyecto_grd

c) Activar entorno de TensorFlow:
.\venv_tf\Scripts\activate

d) Ejecutar el servidor:
python manage.py runserver

Esto inicia el servidor local de desarrollo, la dirección se encuentra en el terminar tras ejecutar el servidor, le puedes dar click y se abrirá una pestaña en tu navegador predeterminado.

# 4. Interfaz de usuario

La aplicación web cuenta con un formulario intuitivo para el ingreso de datos clínicos del paciente.

Características:

Soporte para valores vacíos (NaN): el sistema admite campos sin valor sin generar error.

Listas desplegables dinámicas: para campos categóricos se ofrecen opciones sugeridas para reducir errores de digitación y mejorar la experiencia de usuario.

Botón 'Predecir': al presionar este botón se refresca la página. Si vas al final de esta, verás desplegado el código GRD asignado con su descripción correspondiente.

# 5. Resultado

Una vez enviados los datos y procesados, el sistema mostrará al final de la página el GRD correspondiente a la ruta de atención del paciente. Este resultado se basa en un modelo previamente entrenado en TensorFlow, y considera múltiples variables del ingreso, estada y egreso hospitalario.

# 6. Contacto y soporte

Para soporte técnico o dudas adicionales, contacta al equipo desarrollador o revisa la documentación técnica interna del proyecto.

© Proyecto GRD - Predicción basada en IA

