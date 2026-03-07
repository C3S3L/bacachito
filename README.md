# 🕷️ Cuadrúpedo Robótico - Proyecto Innovabots
**Desarrollo de un robot cuadrúpedo basado en ESP32 con Cinematica Inversa y control PWM.**

---

## 📝 Descripción
Este proyecto consiste en el diseño, impresión 3D y programación de un robot cuadrúpedo (comúnmente llamado "araña"). Utiliza un microcontrolador **ESP32** para procesar la lógica de movimiento y un controlador **PCA9685** para gestionar 12 servos **MG90S**.

El robot es capaz de realizar movimientos fluidos gracias a la implementación de **Cinemática Inversa (IK)**, permitiendo el control mediante coordenadas cartesianas $(X, Y, Z)$.

## 🚀 Características Técnicas
*   **Cerebro:** ESP32 CH340 Lolin (Wi-Fi/Bluetooth).
*   **Control de Motores:** PCA9685 de 16 canales vía I2C.
*   **Actuadores:** 12x Servos TowerPro MG90S.
*   **Alimentación:** Batería LiPo 7.4V con reguladores Step-Down (MP1584) y Step-Up (XL6009).
*   **Lenguaje:** Python (MicroPython) / C++ (Arduino IDE).

## 📐 Dimensiones y Diseño
El diseño fue optimizado para impresión en 3D con las siguientes medidas de eslabones:
- **Coxa (L1):** 55.0 mm
- **Fémur (L2):** 77.5 mm
- **Tibia (L3):** 27.5 mm

## 🔌 Diagrama de Conexión
El sistema utiliza un bus I2C para la comunicación entre el ESP32 y el controlador de servos:
- **SDA:** Pin 4
- **SCL:** Pin 5

> [!TIP]
> Asegúrate de ajustar el regulador de voltaje a **6V** para los servos para evitar daños y maximizar el torque.

## 💻 Instalación y Uso

1.  **Clonar el repositorio:**
    ```bash
    git clone [https://github.com/tu-usuario/nombre-del-repo.git](https://github.com/tu-usuario/nombre-del-repo.git)
    ```
2.  **Cargar MicroPython:** Asegúrate de tener el firmware de MicroPython en tu ESP32.
3.  **Subir librerías:** Sube el archivo `pca9685.py` a la raíz del ESP32.
4.  **Ejecutar:** Carga `main.py` para iniciar la secuencia de caminado.

## 🛠️ Roadmap (Próximas Mejoras)
- [ ] Integración de sensores ultrasónicos para evasión de obstáculos.
- [ ] Control remoto vía App móvil mediante Bluetooth.
- [ ] Implementación de marcha dinámica (Gait control) avanzada.
- [ ] Reconocimiento visual con cámara ESP32-CAM.

## 🤝 Contribuciones
¡Las contribuciones son bienvenidas! Si tienes ideas para mejorar la cinemática o el diseño 3D, siéntete libre de abrir un *Pull Request*.

---
**Desarrollado por Abi - Mecatrónica TecNM**  
*Impulsando la robótica *
