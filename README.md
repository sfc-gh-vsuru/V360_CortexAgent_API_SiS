# V360_CortexAgent_API_SiS

SiS Cortex Agent API orchestration between Cortex Analyst and Search

# Vehicle360_CortexAgent
Vehicle 360 Cortex Agent Demo in SiS

## Steps to complete before running the streamlit app

### Structured data ingest
    Create DB.Schema
    Creates tables for sales data and Kafka sensor data
### Un-structured data ingest
    Setup Stage
    Upload pdf documents

### Cortex Analyst Setup
    Setup in Snowsight using the two tables (sales and kafka data)
    Test in UI asking questions - natural language questions

### Cortex Search Setup
    Setup in Snowsight using the stage created above and the documents
    Test in UI asking natural language questions
    

Update the streamlit.py file with the below schema to access Cortex Analyst and Search:

CORTEX_SEARCH_SERVICES = "VEHICLE360_DB.PUBLIC.SERVICE_MANUAL"
SEMANTIC_MODELS = "@VEHICLE360_DB.PUBLIC.v360/vehicle_data.yaml"
