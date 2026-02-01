# 💈 CitaStudio - Sistema de Gestión para Salones y Barberías

Sistema de gestión profesional todo-en-uno para salones de belleza y barberías. Controla tu negocio completamente desde el navegador sin necesidad de backend o conexión a internet después de la carga inicial.

![GitHub](https://img.shields.io/github/license/tuusuario/citastudio)
![GitHub last commit](https://img.shields.io/github/last-commit/tuusuario/citastudio)

## 🎯 Características Principales

### 📅 Gestión de Agenda
- Vista de todas las citas futuras agrupadas por fecha
- Cancelación automática de citas no confirmadas
- Estados: Pendiente, En Proceso, Completada, Cancelada

### 👥 Gestión de Clientes
- Base de datos completa de clientes
- Historial de visitas y gastos
- Búsqueda rápida
- Notas personalizadas

### 💇 Gestión de Equipo
- Administra tus estilistas/barberos
- Asignación de colores personalizados
- Control de citas por profesional

### 💰 Control de Caja
- Registro de ingresos y egresos
- Balance automático
- Historial de movimientos
- Integración con citas completadas

### 📊 Reportes Profesionales
- Exportación a PDF con diseño profesional
- Backup completo en Excel
- Exportación de datos en JSON
- Reportes por rango de fechas

### 📱 Recordatorios WhatsApp
- Envía recordatorios de citas con un click
- Mensaje personalizado automático
- Integración directa con WhatsApp

### 🎨 Diseño Moderno
- Interfaz elegante en negro y dorado
- 100% responsive (móvil, tablet, PC)
- Menú hamburguesa en dispositivos móviles
- PWA-ready (se puede instalar como app)

## 🚀 Instalación

### Opción 1: Netlify (Recomendado)
1. Crea una cuenta en [Netlify](https://netlify.com)
2. Arrastra la carpeta del proyecto
3. ¡Listo! Obtienes una URL pública

### Opción 2: GitHub Pages
1. Sube el proyecto a un repositorio de GitHub
2. Ve a Settings → Pages
3. Selecciona la rama `main` y carpeta `root`
4. Guarda y obtendrás una URL

### Opción 3: Hosting Propio
1. Sube todos los archivos a tu servidor
2. Apunta tu dominio a la carpeta
3. Abre en el navegador

## 🔐 Configuración Inicial

### Credenciales por Defecto
```
Usuario: admin
Contraseña: admin
```

### Cambiar Credenciales
Edita el archivo `app.js` en la línea **~51**:
```javascript
cargarCredenciales() {
    return [
        { 
            usuario: 'tu_usuario',    // ← Cambia aquí
            password: 'tu_contraseña', // ← Cambia aquí
            tipoNegocio: 'salon',      // 'salon' o 'barberia'
            nombreNegocio: 'TU NOMBRE'
        }
    ];
}
```

## 📱 Instalación como App (PWA)

### En iOS (iPhone/iPad)
1. Abre el sitio en Safari
2. Toca el botón compartir
3. "Agregar a pantalla de inicio"
4. ¡Listo! Ahora funciona como una app

### En Android
1. Abre el sitio en Chrome
2. Menú → "Agregar a pantalla de inicio"
3. ¡Listo! Ahora funciona como una app

## 🛠️ Tecnologías Utilizadas

- **HTML5** - Estructura semántica
- **CSS3** - Diseño moderno con variables CSS
- **JavaScript (Vanilla)** - Sin frameworks, código limpio
- **LocalStorage API** - Persistencia de datos local
- **jsPDF** - Generación de reportes PDF
- **SheetJS (XLSX)** - Exportación a Excel
- **PWA** - Instalable como aplicación

## 📦 Sin Dependencias de Backend

- ✅ No necesita servidor
- ✅ No necesita base de datos
- ✅ No requiere instalación
- ✅ Funciona 100% offline
- ✅ Datos almacenados localmente en el navegador

## 🎯 Casos de Uso

- Salones de belleza pequeños y medianos
- Barberías independientes
- Estilistas freelance
- Peluquerías familiares
- Emprendedores del sector belleza

## ⚠️ Importante

- Los datos se guardan en el navegador (localStorage)
- Hacer backups regularmente usando "Backup Excel"
- Si borras los datos del navegador, pierdes la información
- Recomendado para un máximo de 500 citas simultáneas

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Para cambios importantes:

1. Fork el proyecto
2. Crea una rama (`git checkout -b feature/nueva-funcionalidad`)
3. Commit tus cambios (`git commit -m 'Agrega nueva funcionalidad'`)
4. Push a la rama (`git push origin feature/nueva-funcionalidad`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.

## 👨‍💻 Autor

**Steven** - [GitHub](https://github.com/tuusuario)

## 🙏 Agradecimientos

- Diseñado para pequeños negocios que buscan profesionalidad sin costos mensuales
- Inspirado en la necesidad de herramientas accesibles para emprendedores

## 📞 Soporte

Para reportar bugs o sugerir funcionalidades, abre un [Issue](https://github.com/sdtechsolutionsdev/citastudio/issues)

---

⭐ Si te gusta el proyecto, dale una estrella en GitHub!
```

---

```
# No subir archivos de sistema
.DS_Store
Thumbs.db

# No subir archivos de IDE
.vscode/
.idea/
*.swp
*.swo

# No subir archivos temporales
*~
*.tmp
