# DB Structure
Modellare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario

## Table name
- cars

## Table structure
- ID | BIGINT - AUTO_INCREMENT - PRIMARY KEY (UNIQUE, NOT NULL)
- model | VARCHAR(255) - NOT NULL
- year_of_costruction | YEAR - NOT NULL
- registration_date | DATE - NOT NULL
- Kilometers | INT - NOT NULL
- price | DECIMAL (10, 2) - NOT NULL
- original_price | DECIMAL (10, 2) - NULL
- description | TEXT(500) - NULL
- avaible | TINYINT - DEFAULT(0)
- color | VARCHAR(50) - NULL
- ?fuel_type 
- ?trasmission_type
- license_plate | CHAR(7) - UNIQUE - NOT NULL
- last_service_date | DATE - NULL
- images | TEXT - NULL

``` js

const cars = [{
    id: 1,
    model: 'fiat panda',
    year_of_costruction: 2015,
    registration_date: '2015-03-01',
    kilometers: 35000,
    price: 8500.00,
    original_price: 12500.00,
    description: 'Auto in buone condizioni, senza incidenti.',
    color: 'Rosso',
    fuel_type: 'Diesel',
    transmission_type: 'Manuale',
    license_plate: 'AB123CD',
    last_service_date: '2023-10-15',
    images: ''
}]

```