## Requirements

* Install Requirements.txt:
  ```
  $ pip3 install requirements.txt
  ```
  Source: <https://pypi.org/project/mysqlclient/>

## Use
  
* Run python server:
    ```
    $ python manage.py runserver
    ```
- For Car wallet, navigate to 
    ```
    localhost:8000
    ```
    - Generate Wallet here
    - Click `Make Payment` once wallet credentials are generated

- For Charge wallet, navigate to 
    ```
    localhost:8000/charger/create_payment
    ```
    - Enter address to recieve tokens and amount
    - Copy the code generated and paste it in the car's field at `http://localhost:8000/code/`
    - Charger wallet waits for 1 minute to process the payment, else it times out.
    - Once code is entered, values are retrieved from the JSON bin at `https://api.npoint.io/67a6d648e336c1082719`
    - Click `make payment` to finish the transaction.

- To check transactions for Car, navigate to 
    ```
    http://localhost:8000/transactions/
    ```

- To check transactions for Car, navigate to 
    ```
    http://localhost:8000/charger/transactions
    ```