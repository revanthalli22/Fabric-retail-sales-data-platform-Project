# Data Model Design


## Modeling Approach

The project follows Star Schema design.


## Dimension Tables


| Table | Description |
|-|-|
| DIM_Customer | Customer master |
| DIM_Product | Product information |
| DIM_Driver | Driver details |
| DIM_Vehicle | Vehicle details |
| DIM_Route | Route information |


## Fact Tables


| Table | Description |
|-|-|
| FACT_Shipment | Shipment transactions |
| FACT_Invoice | Invoice transactions |
| FACT_Delivery | Delivery details |
| FACT_Maintenance | Vehicle maintenance |


## Relationships


Example:


DIM_Customer

Customer_ID

        |

        |

FACT_Invoice

Customer_ID



Relationship Type:

One-to-Many


## Slowly Changing Dimensions

Dimension handling:

Type 1:
Overwrite existing value

Type 2:
Maintain historical changes
