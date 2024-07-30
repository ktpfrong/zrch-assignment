# Instructions

Follow these steps to set up and run the ETL pipeline:

1. **Download File**
   - Download the `zrch.zip` file.

2. **Extract Zip File**
   - Unzip `zrch.zip`.

3. **Open Command Prompt**
   - Change the directory to the unzipped folder `zrch` (based on the location of your local folder):
     ```sh
     cd path/to/zrch
     ```

4. **Build and Run Docker Container**
   - In the Command Prompt, run the following command to build and start the Docker container:
     ```sh
     docker-compose up --build
     ```

5. **Open Docker Desktop**
   - Launch Docker Desktop.

6. **Access the Database Container**
   - Navigate to the `zrch` container.
   - Click `Open in terminal` on the `zrch-db-1` database container.

7. **Connect to the Database**
   - Execute the following command to connect to the PostgreSQL database:
     ```sh
     psql -U zrch -d shopsmart
     ```

8. **Profile Customer Transaction Data**
   - Query the customer transaction data by executing this SQL command:
     ```sql
     SELECT * FROM customer_transaction;
     ```
