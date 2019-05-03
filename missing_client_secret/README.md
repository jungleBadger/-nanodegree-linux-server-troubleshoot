# Client_secrets.json import error


### Issue description

The `client_secret.json` file is not being imported through the application



#### Debug

* Make sure the file does exists in the same folder as the application

* Make sure the file is being referenced with the correct name


#### Solution

* If the information about is confirmed, and the error still persists, add the absolute path to the open statement.


#### Example

If you are doing something like

```python
open('./client_secrets.json')
```

change to:


```python
open('/var/www/something/something/client_secrets.json')
```


---



#### Documentation/references

* [Absolute path solution reference](https://www.pythonanywhere.com/forums/topic/4200/)




