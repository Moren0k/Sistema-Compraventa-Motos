# Especificación de Requisitos de Software (SRS)

## Sistema de Gestión para Compraventa de Motos

---

## 1. Introducción

### 1.1 Propósito

Este documento describe los requisitos funcionales y no funcionales para el desarrollo de un sistema web que permita gestionar de forma integral un negocio de compraventa de motos en Colombia.

### 1.2 Alcance

El sistema centralizará inventario, ventas, compras, gestión documental, finanzas, clientes y mantenimiento. Estará orientado a negocios que manejan entre 5 y 20 motos de forma rotativa.

### 1.3 Definiciones

- **SOAT**: Seguro Obligatorio de Accidentes de Tránsito  
- **RUNT**: Registro Único Nacional de Tránsito  
- **SRS**: Software Requirements Specification  
- **Admin**: Usuario con permisos totales (dueño)  
- **Empleado**: Usuario con permisos limitados  

---

## 2. Descripción General

### 2.1 Perspectiva del Producto

Aplicación web responsiva, accesible desde PC, tablet y móvil, con interfaz intuitiva en español.

### 2.2 Funcionalidades Principales

- Gestión de motos (inventario, fotos, estado)
- Registro de compras, ventas, permutas con excedentes
- Control documental (SOAT, revisión, traspasos)
- Finanzas (ingresos, egresos, comisiones, ganancias)
- Seguimiento de clientes e interesados
- Registro de mantenimiento
- Accesos multiusuario

### 2.3 Usuarios del Sistema

- Dueño/Administrador  
- Empleado

---

## 3. Requisitos Específicos

### 3.1 Requisitos Funcionales

| ID     | Descripción                                                                 | Prioridad |
|--------|------------------------------------------------------------------------------|-----------|
| RF-01  | Registrar motos con todos sus datos                                          | Alta      |
| RF-02  | Marcar estado de cada moto (vendida, disponible, consignación, etc.)        | Alta      |
| RF-03  | Subir documentos (SOAT, técnico, tarjeta, contrato)                         | Alta      |
| RF-04  | Registrar ventas con moto en parte de pago y cálculo de excedente           | Alta      |
| RF-05  | Alertas de vencimiento (SOAT, técnico)                                       | Alta      |
| RF-06  | Control de caja: ingresos, egresos, comisiones                              | Alta      |
| RF-07  | Gestión de clientes y seguimiento                                            | Media     |
| RF-08  | Subida de fotos de las motos                                                 | Alta      |
| RF-09  | Acceso con roles diferenciados (admin, empleado)                            | Alta      |
| RF-10  | Responsive (móvil, tablet, PC)                                               | Alta      |
| RF-11  | Buscador avanzado por datos clave                                            | Media     |
| RF-12  | Registro de mantenimiento y costos                                           | Media     |
| RF-13  | Gestión de comisiones para motos en consignación                            | Media     |

### 3.2 Requisitos No Funcionales

| ID     | Descripción                                                  | Prioridad |
|--------|--------------------------------------------------------------|-----------|
| RNF-01 | Accesible vía navegador (web)                                | Alta      |
| RNF-02 | Tiempo de respuesta rápido (<3 segundos)                     | Media     |
| RNF-03 | Base de datos con respaldo automático                        | Alta      |
| RNF-04 | Interfaz simple y en español                                 | Alta      |
| RNF-05 | Compatible con dispositivos móviles                          | Alta      |
| RNF-06 | Seguridad en autenticación                                   | Alta      |

---

## 4. Casos de Uso Principales

- **CU-01**: Registrar moto  
- **CU-02**: Venta con permuta y excedente  
- **CU-03**: Control de vencimientos  
- **CU-04**: Gestión de clientes  
- **CU-05**: Registro de ingresos, egresos y comisiones

---

## 5. Restricciones

- Funciona solo con conexión a internet.  
- Compatible con Chrome, Firefox y Edge.  
- Cumple normativas colombianas de protección de datos (Habeas Data).

---

## 6. Cronograma Estimado

| Fase                                | Duración Estimada |
|-------------------------------------|--------------------|
| Levantamiento de requisitos         | 1-2 semanas        |
| Diseño de arquitectura e interfaz   | 2-3 semanas        |
| Desarrollo backend/frontend         | 6-8 semanas        |
| Pruebas y ajustes                   | 2 semanas          |
| Implementación y capacitación       | 1 semana           |

---

## 7. Tecnologías Propuestas

- **Frontend**: React.js / Vue.js  
- **Backend**: Node.js / Django  
- **Base de datos**: PostgreSQL / MySQL  
- **Hosting**: AWS, DigitalOcean  
- **Almacenamiento de archivos**: AWS S3  
- **Autenticación**: JWT

---

## 8. Anexos

- Bocetos de interfaz (pendiente)  
- Lista de campos por moto y cliente  
- Reglas del negocio y operaciones comunes  

---
