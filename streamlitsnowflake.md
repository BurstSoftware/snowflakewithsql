+----------------+     HTTP Request      +----------------+
|                | <-------------------- |                |
|  Web Browser   |                       | Streamlit App  |
|  (User)        | --------------------> |                |
+----------------+     HTTP Response     +----------------+
                                   |
                                   v
                            +---------------+
                            | Streamlit     |
                            | Server        |
                            +---------------+
                                   |
                            SQL Query  |
                                   v
                          +-----------------+
                          |                 |
                          |   Snowflake     |
                          |   Data Warehouse|
                          |                 |
                          +-----------------+
                                   |
                             Data Response |
                                   v
                            +---------------+
                            | Streamlit     |
                            | Server        |
                            +---------------+
                                   |
                           Updates UI |
                                   v
+----------------+    HTTP Response      +----------------+
|                | <-------------------- |                |
|  Web Browser   |                       | Streamlit App  |
|  (User)        | --------------------> |                |
+----------------+     HTTP Request      +----------------+
