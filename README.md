<div align="center">

# Modelo Relacional y Constraints — Car Dealership & Human Resources DB

![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Database](https://img.shields.io/badge/Base_de-Datos_Relacional-FF6B35?style=for-the-badge)
![Normalization](https://img.shields.io/badge/Normalización-3FN-8E24AA?style=for-the-badge)

> Diseño e implementación propios de bases de datos relacionales para dos dominios de negocio: concesionario automotriz y recursos humanos.

## Descripción

</div>

---

Proyecto desarrollado por **Alejandro De Mendoza** que aplica el modelo relacional sobre dos dominios de negocio reales: un **concesionario de automóviles** y un sistema de **recursos humanos**. Se implementa el diseño completo desde el DER hasta el DDL en SQL, con normalización a 3FN, restricciones de integridad referencial y optimización de consultas para reportes de negocio.

## Dominios modelados

### Concesionario automotriz
- Entidades: Vehículo, Marca, Modelo, Cliente, Venta, Vendedor
- Relaciones: Cliente compra Vehículo a través de Venta, Vendedor gestiona Venta

### Recursos Humanos
- Entidades: Empleado, Departamento, Cargo, Historial Salarial, Ubicación

## Arquitectura

```mermaid
flowchart TD
    A[Concesionario Automotriz] --> B[Vehiculo / Marca / Modelo / Cliente / Venta / Vendedor]
    C[Recursos Humanos] --> D[Empleado / Departamento / Cargo / Historial Salarial]
    B --> E[HR_Database_Create_Tables_Script.sql - DDL]
    D --> E
    E --> F[Normalizacion 3FN - 1FN / 2FN / 3FN]
    F --> G[Datos CSV - Employees / Departments / Jobs / Locations]
    G --> H[Consultas y Reportes SQL]
```

## Normalización aplicada

| Forma Normal | Condición satisfecha |
|---|---|
| 1FN | Atributos atómicos, clave primaria definida |
| 2FN | Dependencias totales sobre la clave primaria |
| 3FN | Sin dependencias transitivas entre atributos no clave |

## Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `HR_Database_Create_Tables_Script.sql` | DDL completo del esquema HR |
| `*.csv` | Datos de prueba: Employees, Departments, Jobs, Locations |
| `Activity.docx` | Enunciado y desarrollo de las actividades |

## Contexto académico

**Asignatura:** Bases de Datos · **Institución:** Ingeniería Informática
**Autor:** Alejandro De Mendoza — Ingeniero Informático · Especialista en Ingeniería de Software · Máster en Arquitectura de Software

---

## Autor

**Alejandro De Mendoza**  
Ingeniero Informático · Especialista en IA · Especialista en Ingeniería de Software · Máster en Arquitectura de Software

[![GitHub](https://img.shields.io/badge/GitHub-AlejoTechEngineer-181717?style=for-the-badge&logo=github)](https://github.com/AlejoTechEngineer)
