# � Salvador de Similitud - Versión Web

Herramienta web para modificar documentos Word insertando caracteres invisibles que alteran la similitud del texto.

## 🚀 Uso Rápido

1. **Abre:** `index.html` en tu navegador
2. **Arrastra:** tu archivo .docx a la zona de carga
3. **Configura:** el número de modificaciones (1-10)
4. **Procesa:** y descarga el archivo modificado

## ✅ Características

- **100% JavaScript** - No requiere servidor ni instalación
- **Ultra seguro** - Modificaciones mínimas que no corrompen el archivo
- **Compatible** - Funciona con cualquier documento Word (.docx)
- **Invisible** - Las modificaciones son completamente invisibles al usuario
- **GitHub Pages** - Funciona directamente desde el navegador

## 🔧 Cómo Funciona

La herramienta:
1. Lee el archivo Word (.docx) 
2. Localiza párrafos con texto
3. Inserta espacios invisibles al final de algunos párrafos
4. Genera un nuevo archivo que se abre perfectamente en Word

## 📁 Archivos del Proyecto

- `index.html` - Aplicación web principal
- `SALVADOR DE SIMILITUD.py` - Versión original de escritorio  
- `web_app/` - Versión Flask (servidor Python)
- `_config.yml` - Configuración de GitHub Pages

## 🌐 Acceso Online

La aplicación está disponible en: `https://francisco-campos-s.github.io/SALVADOR_DE_SIMILITUD.git.io/`

## 💡 Uso Recomendado

- **Configuración:** 3-5 modificaciones es suficiente para la mayoría de casos
- **Archivos:** Máximo 10MB por limitaciones del navegador
- **Formato:** Solo archivos .docx (Word 2007+)

---

**Versión Ultra-Segura** - Diseñada para garantizar que los archivos procesados se abran correctamente en Microsoft Word.

Una aplicación web profesional para procesar documentos de Word insertando caracteres invisibles que ayudan a modificar la similitud del texto, diseñada específicamente para uso académico y profesional.

## 🌟 Características

- **Versión Flask Local**: Aplicación web completa con backend Python
- **Versión GitHub Pages**: Procesamiento 100% en el navegador, sin servidor
- **Interfaz Moderna**: Diseño responsive con drag & drop
- **Privacidad**: Los archivos se procesan localmente
- **Compatibilidad**: Soporte para archivos .docx y .docm

## 🚀 Versiones Disponibles

### 1. GitHub Pages (Recomendado para uso público)
**URL:** https://francisco-campos-s.github.io/SALVADOR_DE_SIMILITUD.git.io/

**Características:**
- ✅ Sin instalación requerida
- ✅ Funciona 100% en el navegador
- ✅ Máxima privacidad (archivos no salen de tu computadora)
- ✅ Compatible con todos los sistemas operativos
- ✅ Acceso desde cualquier dispositivo

### 2. Aplicación Flask Local (Para uso avanzado)

**Instalación:**
```bash
# Clonar repositorio
git clone https://github.com/Francisco-Campos-S/SALVADOR_DE_SIMILITUD.git.io.git
cd SALVADOR_DE_SIMILITUD.git.io/web_app

# Crear entorno virtual
python -m venv venv

# Activar entorno virtual
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate

# Instalar dependencias
pip install -r requirements.txt

# Ejecutar aplicación
python app.py
```

**Uso:**
1. Abrir navegador en `http://localhost:5000`
2. Subir archivo .docx o .docm
3. Configurar parámetros
4. Procesar y descargar

## 📋 Instrucciones de Uso

### Paso a Paso:

1. **Seleccionar Archivo**
   - Haz clic en el área de subida o arrastra tu archivo
   - Archivos soportados: `.docx`, `.docm`
   - Tamaño máximo: 16MB (Flask) / 10MB (GitHub Pages)

2. **Configurar Parámetros**
   - **Paso**: Número de caracteres entre inserciones (recomendado: 70)
   - Valores válidos: 10-200 caracteres

3. **Procesar Documento**
   - Haz clic en "Procesar Documento"
   - El sistema insertará '0' blancos en posiciones estratégicas
   - Se saltará automáticamente la primera página

4. **Descargar Resultado**
   - El archivo se descarga automáticamente con sufijo "_modificado"
   - Mantiene el formato original del documento

## 🔧 Tecnologías Utilizadas

### Versión Flask:
- **Backend**: Python 3.8+ con Flask
- **Procesamiento**: python-docx para manipulación de documentos
- **Frontend**: HTML5, CSS3, JavaScript ES6
- **Seguridad**: Validación de archivos, límites de tamaño

### Versión GitHub Pages:
- **Frontend**: HTML5, CSS3, JavaScript ES6
- **Procesamiento**: JSZip para manipular archivos Office
- **Compatibilidad**: Funciona en todos los navegadores modernos

## 🛡️ Funcionamiento del Algoritmo

El algoritmo procesa documentos de Word de la siguiente manera:

1. **Análisis del Documento**
   - Lee todos los párrafos del documento
   - Omite la primera página para preservar encabezados
   - Identifica texto con longitud suficiente

2. **Inserción Estratégica**
   - Calcula posiciones cada X caracteres (paso configurado)
   - Busca espacios cercanos a estas posiciones
   - Reemplaza espacios con '0' de color blanco

3. **Preservación del Formato**
   - Mantiene la estructura original del documento
   - Los '0' blancos son invisibles al ojo humano
   - No afecta la legibilidad del contenido

## 📁 Estructura del Proyecto

```
SALVADOR_DE_SIMILITUD.git.io/
├── index.html                 # Versión GitHub Pages
├── web_app/                   # Aplicación Flask
│   ├── app.py                # Servidor Flask
│   ├── requirements.txt      # Dependencias Python
│   ├── templates/
│   │   └── index.html       # Template Flask
│   └── uploads/             # Archivos temporales
├── SALVADOR DE SIMILITUD.py  # Versión original (Tkinter)
└── README.md                 # Este archivo
```

## 🔒 Privacidad y Seguridad

- **Procesamiento Local**: En ambas versiones, el procesamiento es local
- **Sin Almacenamiento**: No se guardan archivos en servidores
- **Validación Estricta**: Solo archivos Word válidos
- **Límites de Tamaño**: Protección contra archivos excesivamente grandes

## 🌐 Despliegue en GitHub Pages

El archivo `index.html` en la raíz está configurado para GitHub Pages:

1. El repositorio debe ser público
2. GitHub Pages debe estar habilitado en la configuración
3. La página estará disponible en: `https://[usuario].github.io/[repositorio]/`

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork del repositorio
2. Crear rama para nueva funcionalidad
3. Commit de cambios
4. Push a la rama
5. Crear Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver archivo `LICENSE` para más detalles.

## 🆘 Soporte

Si encuentras algún problema:

1. Revisa que el archivo sea un .docx válido
2. Verifica el tamaño del archivo (máximo 16MB/10MB)
3. Usa un navegador moderno y actualizado
4. Para la versión Flask, asegúrate de tener Python 3.8+

## 📊 Compatibilidad

### Navegadores Soportados (GitHub Pages):
- ✅ Chrome 80+
- ✅ Firefox 75+
- ✅ Safari 13+
- ✅ Edge 80+

### Sistemas Operativos (Flask):
- ✅ Windows 10/11
- ✅ macOS 10.15+
- ✅ Ubuntu 20.04+
- ✅ Otras distribuciones Linux

---

**Desarrollado con ❤️ para la comunidad académica y profesional**