# Ontology for Laptops using Protégé

This project presents a simple ontology for laptops developed using Protégé. The ontology models laptop specifications such as processor, memory, storage, display, and operating system using ontology concepts including classes, object properties, data properties, and individuals. The project further integrates the HermiT reasoner for ontology consistency checking and DL queries for inferencing.

# Objective

The objective of this project is to:

Create an ontology for laptops and their components
Define relationships between laptops and hardware/software specifications
Perform ontology consistency checking using a reasoner
Execute DL queries for inferencing and knowledge retrieval

# Ontology Design

The ontology is designed with the following hierarchy:

Device
Computers
Laptops

Additional component classes include:

- Processor (CPU)
- Memory (RAM)
- Storage (Hard Drive/SSD)
- Display (Screen)
- OperatingSystem (OS)

All classes are subclasses of owl:Thing.

# Object Properties

The ontology uses object properties to connect laptop instances with their components.

Examples:

- hasProcessor
- hasMemory
- hasDisplay
- hasOS
- hasStorage

These are defined as sub-properties of hasComponent.

# Data Properties

Data properties are used to store literal values related to laptop specifications.

Examples:

- modelName
- processorName
- ramSizeGB
- storageCapacityGB
- screenSizeInches
- osName

# Individuals

The ontology includes individuals representing:

Hardware components
Operating systems
Laptop instances

Example laptop individuals:

Dell_Inspiron_15_3000
MacBook_Air_M2

These individuals are linked to their corresponding components through object properties.

# Reasoner Integration

The ontology is validated using the HermiT Reasoner available in Protégé.

The reasoner is used for:

- Consistency checking
- Validation of ontology relationships
- Logical inferencing

# DL Queries

DL (Description Logic) queries are executed using the Protégé DL Query plugin to retrieve and infer information from the ontology.

Example queries:

- Laptop and hasOS value Windows_11_Pro
- Laptop and hasMemory some Memory

# Tools and Technologies

Protégé Desktop (Version 5.6.9)
Web Protégé
HermiT Reasoner (Version 1.4.3)
DL Query Plugin (Version 4.0.1)
OWL (Web Ontology Language)

# Future Work
- Expand the ontology with additional laptop specifications
- Add logical constraints and restrictions
- Introduce advanced reasoning rules
- Extend inferencing capabilities using more complex DL queries
