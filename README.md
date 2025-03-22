# Banco App

Este es un proyecto básico de una aplicación bancaria desarrollado en Java utilizando Spring Boot y JPA. La aplicación permite gestionar clientes, cuentas y transacciones.

## Entidades

### Cliente
Representa a un cliente del banco. Contiene los siguientes campos:
- `id`: Identificador único.
- `nombre`: Nombre del cliente.
- `apellido`: Apellido del cliente.
- `email`: Correo electrónico del cliente.

### Cuenta
Representa una cuenta bancaria. Contiene los siguientes campos:
- `id`: Identificador único.
- `numeroCuenta`: Número único de la cuenta.
- `saldo`: Saldo actual de la cuenta.

### Transaccion
Representa una transacción bancaria. Contiene los siguientes campos:
- `id`: Identificador único.
- `monto`: Monto de la transacción.
- `fecha`: Fecha y hora de la transacción.

## Repositorios

Los repositorios proporcionan acceso a las operaciones CRUD básicas para las entidades:
- `ClienteRepository`: Repositorio para la entidad `Cliente`.
- `CuentaRepository`: Repositorio para la entidad `Cuenta`.
- `TransaccionRepository`: Repositorio para la entidad `Transaccion`.

## Requisitos Previos

- Java 17 o superior.
- Maven 3.8 o superior.
- Base de datos compatible con JPA (por ejemplo, MySQL, PostgreSQL, H2).

## Configuración

1. Clona el repositorio:
   ```bash
   git clone https://github.com/CarlosQuiroz25/banco-app.git
   cd banco-app

2. Configura la base de datos en el archivo src/main/resources/application.properties. Ejemplo para MySQL:
   
   spring.datasource.url=jdbc:mysql://localhost:3306/banco_app
   spring.datasource.username=tu_usuario
   spring.datasource.password=tu_contraseña
   spring.jpa.hibernate.ddl-auto=update


4. Ejecuta el proyecto:
  ```bash
  mvn spring-boot:run
   
