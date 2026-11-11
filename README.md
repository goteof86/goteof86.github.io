# Blog Django con predictor de Machine Learning

Aplicación web hecha con Django: un blog con usuarios y un modelo de Machine Learning integrado que se puede probar desde el navegador.

🔗 **Demo en vivo:** https://goteof86.pythonanywhere.com

## Qué hace

- Registro e inicio de sesión de usuarios
- Crear, editar y eliminar artículos (solo su autor puede modificarlos)
- Formulario de contacto y bandeja de mensajes
- Modo oscuro / claro
- **Predictor de clientes con ML:** a partir de la edad y el tiempo que el visitante pasa en la página, un modelo de clasificación predice si comprará o no

## Tecnologías

Python · Django · scikit-learn · joblib · SQLite · HTML / CSS / JavaScript

## Estructura del proyecto

- `core/`: configuración de Django
- `hola/`: app principal (modelos, vistas, plantillas y lógica de ML)
- `modelo_clientes.pkl`: modelo entrenado
- `redes_neuronales/`: ejercicios con TensorFlow (Celsius a Fahrenheit y XOR)

## Cómo ejecutarlo en local

1. Clona el repositorio e instala las dependencias:

        git clone https://github.com/goteof86/blog-django-predictor.git
        cd blog-django-predictor
        pip install -r requirements.txt

2. Crea un archivo `.env` en la raíz del proyecto con tu propia clave:

        SECRET_KEY=pon-aqui-una-clave-propia

3. Prepara la base de datos y arranca el servidor:

        python manage.py migrate
        python manage.py runserver

## Autor

Leo · goteof86@gmail.com
