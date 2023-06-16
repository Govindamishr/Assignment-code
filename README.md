# Assignment-code
# Car Service Software

This Java software provides a car service station with the ability to generate detailed bills for different types of cars and services. It calculates the total bill based on the car type and requested service codes, taking into account the different prices associated with each service.

## Features

- Caters to different types of cars: Hatchback, Sedan, SUV.
- Provides the following services:
  - Basic Service
  - Engine Fixing
  - Clutch Fixing
  - Gear Fixing
  - Brake Fixing
- Each service has a service code associated with it.
- Different prices for each service based on the type of car.

## Service Prices

The software initializes the service prices for each car type as follows:

| Service Code | Service           | Hatchback (₹) | Sedan (₹) | SUV (₹) |
|--------------|-------------------|--------------|-----------|---------|
| BS01         | Basic Servicing   | 2000         | 4000      | 5000    |
| EF01         | Engine Fixing     | 5000         | 8000      | 10000   |
| CF01         | Clutch Fixing     | 2000         | 4000      | 6000    |
| BF01         | Brake Fixing      | 1000         | 1500      | 2500    |
| GF01         | Gear Fixing       | 3000         | 6000      | 8000    |

## Usage

1. Instantiate the `CarServiceStation` class.
2. Call the `generateBill` method with the car type and an array of service codes.
3. The method will print the type of car, service codes, charges for each service, total bill, and, if the total bill exceeds ₹ 10,000, it will mention the complimentary cleaning included.

Example:

```java
CarServiceStation serviceStation = new CarServiceStation();

String carType = "Hatchback";
String[] serviceCodes = {"BS01", "EF01"};

serviceStation.generateBill(carType, serviceCodes);
