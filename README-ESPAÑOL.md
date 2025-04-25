¡Claro! Aquí tienes la traducción al español del `README.md` original de ZapZap:

```markdown
# [ZapZap](https://rtosta.com/zapzap-web/) - WhatsApp de Escritorio para Linux
![ZapZap para WhatsApp](share/screenshot/default.png)

## Acerca de

ZapZap acerca la experiencia de WhatsApp en Linux a la de una aplicación nativa. Dado que Meta no proporciona una API pública para aplicaciones de terceros, ZapZap se desarrolla como una [Aplicación Web Progresiva](https://es.wikipedia.org/wiki/Progressive_Web_Apps) (PWA).

## Descarga

**Flathub:** [Descargar a través de Flathub](https://flathub.org/apps/details/com.rtosta.zapzap)
**Fedora Copr:** [Descargar a través de Fedora Copr](https://copr.fedorainfracloud.org/coprs/rafatosta/zapzap/)

## Características

ZapZap extiende WhatsApp Web con funcionalidades adicionales:

### **Apariencia**

- Modo claro y oscuro adaptativo
- Modo de pantalla completa
- Decoraciones de ventana personalizadas
- Ajuste de la escala de la interfaz (ideal para pantallas 2K/4K)

### **Usabilidad**

- Atajos de teclado para las opciones principales
- Icono adaptativo en la bandeja del sistema (notifica nuevos mensajes)
- Soporte para proceso en segundo plano
- Funcionalidad de arrastrar y soltar
- Posibilidad de seleccionar una carpeta personalizada para descargas
- Carpeta temporal para abrir archivos

### **Extras**

- Corrector ortográfico con selección de idioma a través del menú contextual
- Iconos personalizables para la bandeja del sistema
- Opción para elegir una carpeta para diccionarios personalizados
- Ajuste para deshabilitar el diálogo de selección de archivos nativo (Hyprland)
- Panel de Configuración reorganizado
- Sección de Rendimiento añadida

## Desarrollo

ZapZap está construido utilizando PyQt6 y PyQt6-WebEngine.

### **Construir y Ejecutar Localmente**

- [Instrucciones](/_run/README.md)

### **Empaquetado**

- [Fedora Copr](/_packaging/fedora/zapzap.spec)
- [Flatpak](/_packaging/flatpak/README.md)

### **Traducción**

ZapZap soporta traducciones. Si falta el archivo de tu idioma en la carpeta [po](/po), envía una solicitud de extracción (pull request) o abre un [incidente](https://github.com/rafatosta/zapzap/issues).

## Ejecución

### **Descripción**

Esta es una aplicación de Python que se puede ejecutar en tres modos diferentes:

- **dev**: Modo de desarrollo
- **preview**: Modo de vista previa
- **build**: Genera un ejecutable para producción (`zapzap.flatpak`)

El proyecto utiliza `zapzap.toml` para gestionar las dependencias y un script de Python (`run.py`) para ejecutar comandos.

### **Requisitos**

- Python 3.9 o superior

### **Instalación**

1. **Clonar el repositorio**

```bash
git clone [https://github.com/rafatosta/zapzap.git](https://github.com/rafatosta/zapzap.git)
cd zapzap
```

2. **Instalar las dependencias**

Asegúrate de que Poetry esté instalado. Si no lo está, sigue [esta guía](https://python-poetry.org/docs/#installation).

Luego, instala las dependencias del proyecto:

```bash
poetry install
```

3. **Activar el entorno virtual**

Poetry crea un entorno virtual para el proyecto. Para activarlo, ejecuta:

```bash
poetry shell
```

### **Uso**

#### Ejecutar en modo de desarrollo

```bash
python run.py dev
```

#### Ejecutar en modo de vista previa

```bash
python run.py preview
```

Construye y ejecuta directamente en Flatpak

#### Generar el ejecutable para producción

```bash
python run.py build
```

El ejecutable se generará en la carpeta `dist/` como `zapzap.flatpak`.

### **Estructura del Proyecto (En Construcción)**

```plaintext
zapzap/
├── zapzap.toml        # Archivo de configuración del proyecto
├── run.py             # Script para gestionar los modos de ejecución
├── zapzap/
│   └── main.py        # Archivo principal de la aplicación
├── dist/              # (Generado) Carpeta donde se creará el ejecutable
└── README.md          # Documentación del proyecto
```

## Contribuciones

¡Las contribuciones son bienvenidas! Por favor, envía una solicitud de extracción con cualquier mejora o cambio que desees proponer.

## Licencia

Este proyecto está licenciado bajo la GPL. Consulta el archivo LICENSE para obtener más información.

## Donaciones

**PayPal:** [Donar a través de PayPal](https://www.paypal.com/donate/?business=E7R4BVR45GRC2&no_recurring=0&item_name=ZapZap+-+Whatsapp+Desktop+for+linux%0AAn+unofficial+WhatsApp+desktop+application+written+in+Pyqt6+%2B+PyQt6-WebEngine.&currency_code=USD)
**Pix:** [Donar a través de Pix](https://nubank.com.br/pagar/3c3r2/LS2hiJJKzv)
**Ko-fi:** [Donar a través de Ko-fi](https://ko-fi.com/X8X2E1OLG)

## Contacto

**Mantenedor:** Rafael Tosta
**Correo Electrónico:** [rafa.ecomp@gmail.com](mailto:rafa.ecomp@gmail.com)
```

Espero que esta traducción te sea útil para entender mejor el proyecto ZapZap. ¿Hay algo más en lo que te pueda ayudar?
