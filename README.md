# 🥚 EggMinder Pro - Dashboard IoT

> Sistema de gestión centralizada para bandejas de huevos inteligentes (IoT), permitiendo el monitoreo de inventario y control de frescura en tiempo real.

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![Bootstrap](https://img.shields.io/badge/bootstrap-%23563D7C.svg?style=for-the-badge&logo=bootstrap&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=F7DF1E)

## 📖 Descripción

Este proyecto es una aplicación web **SPA (Single Page Application)** diseñada para administrar múltiples dispositivos **Quirky Egg Minder**. Simula un entorno IoT donde las bandejas inteligentes envían datos sobre la cantidad de huevos restantes y permiten al usuario activar indicadores LED para identificar los productos más antiguos.

El sistema consume una **API REST simulada (MockAPI)** para realizar operaciones CRUD, control de estado y monitoreo en vivo.

## 🚀 Características Principales

* **Administración (CRUD):** Registro, visualización y eliminación de bandejas conectadas.
* **Control Remoto:** Interruptores para activar/desactivar los LEDs de cada dispositivo (Simulación de función "Find Oldest Egg").
* **Monitoreo en Tiempo Real:**
    * Dashboard visual que representa gráficamente los espacios ocupados en la bandeja.
    * Tabla de historial de eventos con actualización automática cada **2 segundos**.
    * Indicadores de estado (Online/Offline) y alertas visuales.
* **Diseño Responsivo:** Interfaz moderna construida con **Bootstrap 5**.

## 🛠️ Tecnologías Utilizadas

* **Frontend:** HTML5, CSS3, Bootstrap 5.3.
* **Lógica:** Vanilla JavaScript (ES6+), Fetch API.
* **Backend (Simulado):** MockAPI.io.
* **Control de Versiones:** Git & GitHub.

## ⚙️ Configuración y Instalación

Para ejecutar este proyecto en tu máquina local:

1.  **Clonar el repositorio:**
    ```bash
    git clone [https://github.com/elsundress/EggMinder.git](https://github.com/elsundress/EggMinder.git)
    ```

2.  **Configurar la API:**
    El proyecto utiliza MockAPI. Para que funcione correctamente, debes tener tu propio endpoint o usar el configurado en `index.html`.
    
    Si configuras tu propio MockAPI, el recurso `trays` debe tener esta estructura JSON:
    ```json
    {
      "id": "1",
      "name": "Refrigerador Cocina",
      "location": "Planta Baja",
      "led_active": false,  // (boolean)
      "egg_count": 12       // (number)
    }
    ```

3.  **Ejecutar:**
    Simplemente abre el archivo `index.html` en tu navegador web favorito (Chrome, Edge, Firefox). No requiere servidor Node.js ni instalaciones adicionales.

## 📸 Capturas de Pantalla

### Panel de Administración
_(Puedes agregar aquí tus capturas de pantalla, ej: ![Admin](./img/admin.png))_

### Monitoreo en Vivo
_(Espacio para captura del monitor)_

## ✒️ Autor

**Misael** - *Desarrollo y