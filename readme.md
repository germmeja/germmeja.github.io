# PaquilandiaCRM 🌱

Sistema de administración rural sin servidor para el manejo de cultivos, actividades, equipos y mantenimientos. Diseñado para operar directamente en el navegador usando SQLite vía WebAssembly (`sql.js`).

## 🧩 Componentes

- `index.html` → Interfaz principal con formularios, trazabilidad y exportación.
- `sql-wasm.js` / `sql-wasm.wasm` → Motor SQLite para navegador.
- `DBPaquilandia.db` → Base SQLite local con 4 tablas definidas:
  - `Cultivo_Nombre`
  - `Cultivo_Nombre_Actividades`
  - `Equipos_Nombre`
  - `Equipos_Nombre_Tipo_Mtto`

## 🚀 Funcionalidades

- 📂 Carga de base local
- ➕ Inserción de nuevos registros
- ✏️ Modificación trazable por campos indexados
- 🗑️ Eliminación sin borrar (marcado como retirado)
- 🔍 Filtros inteligentes por combinación de índices
- 💾 Exportación de base `.db` actualizada desde navegador
- 🚪 Cierre de sesión local

## 📦 Requisitos

- Navegador moderno (Edge, Chrome, Firefox)
- Archivos `sql-wasm.js` y `sql-wasm.wasm` en la misma carpeta
- Archivo `DBPaquilandia.db` con estructura compatible

## 📄 Uso

1. Abre `index.html` en tu navegador
2. Carga la base local (`DBPaquilandia.db`)
3. Usa las pestañas para registrar o modificar
4. Exporta los cambios con el botón “💾 Descargar BD”

## ⚙️ Futuras mejoras

- Diseño visual rural minimalista
- Registro de responsables por actividad
- Resumen exportable en PDF o JSON
- Integración con sensores o APIs externas

---
Desarrollado con trazabilidad y cariño para Paquilandia 🧤📊☕