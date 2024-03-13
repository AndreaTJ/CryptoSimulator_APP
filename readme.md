# Crypto Simulator

## Installation
1. Run
```
pip install -r requirements.txt
```

2. Create config.py

* Rename `config_template.py` to `config.py` and correctly fill in your keys.

```
 mv config_template.py config.py
```

3. Create Database.

* Execute `migrations.sql` with `sqlite3` in the file chosen as the Database.

    a) Execute DB migrations with sqlite3 ○ from the /data directory run
    
    ``` 
    sqlite3 <database_name>.db

    ```
    b) From the sqlite3 console

    - Run

    ```
    .read migrations.sql
    ```

    - Check that the tables have been created

    ```
    .tables
    ```

    - Exit

    ```
    .q
    ```
4. Rename `config_template.ini` to `config.ini` and correctly fill in your APIKEY.

* To obtain the APIKEY, visit [CoinMarketCap](https://coinmarketcap.com/api/). There is a free plan.

```
 mv config_template.ini config.ini
```

5. Correctly fill in .env (for development only)

Rename `.env_template` to `.env` and fill in the keys

```
 mv .env_template .env
```

    - FLASK_APP=run.py
    - FLASK_ENV=`development` or `production`

6. Run

```
python cargaMonedas.py
```

7. Run

```
flask run
```


Please remember that you need an internet connection.