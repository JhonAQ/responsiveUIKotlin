# Laboratorio 04: Diseño Adaptativo en Pantallas Móviles

**Universidad Nacional de San Agustín de Arequipa (UNSA)**  
**Facultad de Ingeniería de Producción y Servicios**  
**Escuela Profesional de Ingeniería de Sistemas (EPIS)**  
**Curso:** Introducción al Desarrollo de Nuevas Plataformas (E) - Semestre 2026-B  
**Docente:** Mg. Christian Alain Revilla Arroyo  

---

## 👥 Integrantes
- **Johann Andre Caceres Ruiz**
- **Paul Adree Cari Lipe**
- **Jhonatan David Arias Quispe**

---

## 📱 Descripción del Proyecto

Aplicación Android desarrollada en **Kotlin** utilizando **Jetpack Compose** y **Material Design 3 (M3)**, implementando patrones de arquitectura responsiva y adaptativa para múltiples factores de forma:

- **Estrategia Adaptativa:** Uso de `BoxWithConstraints` con umbral de corte de `600.dp`.
  - **Factor Compacto (`< 600.dp`):** Disposición en columna única vertical con `verticalScroll` asistido para smartphones.
  - **Factor Expandido (`>= 600.dp`):** Reestructuración a dos paneles simultáneos (`Row`), manteniendo fija la cabecera y el botón de acción a la izquierda, y el temario/métricas con scroll independiente a la derecha.
- **Soporte de Temas:** Paletas semánticas completas para **Modo Claro** y **Modo Oscuro** con altos ratios de contraste WCAG.
- **Accesibilidad Tipográfica:** Empleo estricto de unidades `sp` y modificadores flexibles (`wrapContentHeight`) para tolerar escalados del sistema de hasta **200%** sin truncamiento ni recortes.

---

## 🛠️ Tecnologías Empleadas
- **Lenguaje:** Kotlin 2.2+
- **Framework UI:** Jetpack Compose (BOM 2026.02.01)
- **Design System:** Material Design 3 (M3)
- **Build System:** Gradle 9.6 con Kotlin DSL (`build.gradle.kts`)
- **Compatibilidad:** Android 7.0+ (API 24 a API 37)

