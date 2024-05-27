# Tarea en clase semana 8
## La funcion count
### Creacion de la tabla
El siguiente código crea la tabla **client**
```
CREATE TABLE IF NOT EXIST Client (
    id SERIAL,
    nui VARCHAR(50) NOT NULL,
    fullname VARCHAR(100) NOT NULL,
    phone VARCHAR(20),
    type_of_client VARCHAR(50) DEFAULT 'BASIC',
    city VARCHAR(50),
    credit_limit DECIMAL(10, 2)
);


```

 ### Inserción  de datos
```
INSERT INTO Client (nui, fullname, phone, type_of_client, city, credit_limit) VALUES
('1728394857', 'Juan Perez', '0987654321', 'Regular', 'Quito', 5000.00),
('0912345678', 'Maria Gonzalez', '0987123456', 'VIP', 'Guayaquil', 10000.00),
('1102345679', 'Carlos Ramirez', '0998765432', 'Regular', 'Cuenca', 3000.00),
('1203456789', 'Ana Martinez', '0976543210', 'Premium', 'Ambato', 7000.00),
('1304567890', 'Luis Torres', '0965432109', 'Regular', 'Manta', 2000.00),
('1405678901', 'Carmen Sanchez', '0954321098', 'VIP', 'Portoviejo', 8000.00),
('1506789012', 'Pedro Castillo', '0943210987', 'Regular', 'Loja', 4000.00),
('1607890123', 'Laura Herrera', '0932109876', 'Premium', 'Esmeraldas', 6000.00),
('1708901234', 'Jose Rojas', '0921098765', 'Regular', 'Machala', 3500.00),
('1809012345', 'Sofia Ruiz', '0910987654', 'VIP', 'Riobamba', 9000.00);
```
```
INSERT INTO Client (nui, fullname, phone, type_of_client, city, credit_limit) VALUES
('1900123456', 'Gabriela Morales', NULL, 'Regular', 'Santo Domingo', 4500.00),
('2001234567', 'Ricardo Alvarez', NULL, 'VIP', 'Ibarra', 7500.00),
('2102345678', 'Patricia Flores', NULL, 'Regular', 'Latacunga', 3000.00),
('2203456789', 'Jorge Delgado', NULL, 'Premium', 'Quevedo', 6800.00),
('2304567890', 'Monica Castro', NULL, 'Regular', 'Tulcán', 2500.00);

```
![image](https://github.com/DanielaM0101/tarea-event/assets/146010135/64467e6b-35ff-4fb5-8997-6eec204e8b4f)
### Mostrar el total de nombres
Para mostar todas las funciones se usa la funcion ***COUNT*** () pasandole como parametro el campo "fullname"
```
SELECT COUNT (fullname) AS total_names
FROM client;
````
![Captura de pantalla 2024-05-27 094655](https://github.com/DanielaM0101/tarea-event/assets/146010135/151ebcb8-de97-480e-a651-ce2a62de655b)

### Mostrar el total de telefonos

![Captura de pantalla 2024-05-27 095025](https://github.com/DanielaM0101/tarea-event/assets/146010135/a18f2e72-ab75-4050-a5b7-85202aefe280)
### Mostrar el total de telefonos y nombres 
![Captura de pantalla 2024-05-27 095118](https://github.com/DanielaM0101/tarea-event/assets/146010135/454bef42-4065-41eb-9d2f-2cac98a0174b)
![Captura de pantalla 2024-05-27 095452](https://github.com/DanielaM0101/tarea-event/assets/146010135/78fa8d52-47f2-4490-af25-168bcd9960cf)
### Mostrar el total de las cuidades 
![Captura de pantalla 2024-05-27 095748](https://github.com/DanielaM0101/tarea-event/assets/146010135/81d8f0e5-e6be-4a20-bc5f-0800b56268f6)
### Mostrar ciudades sin repetir
![Captura de pantalla 2024-05-27 095748](https://github.com/DanielaM0101/tarea-event/assets/146010135/ea80bb5f-428c-4aba-8032-348846a4e5af)

***El codigo para todas las funciones se muestra en cada captura***









