![Banner](https://github.com/NorsHiden/Intra42Api-wrapper_moduleblob/master/apiwrapper.png)

## 42 Network API Wrapper
Intra42api simply allows you to connect with **42 Network** API and to get all the desired data in an easy way.

##  Installation
#### NOTE: Python 3.6 or higher is required.
```bash
# Windows
py -3.9 -m pip install intra42api

# Linux
python3.9 -m pip install intra42api
```
##  Quick Example

```py
import intra42api

intra = intra42api.Intra42()

intra.setToken('MY_AWESOME_UID', 'MY_AWESOME_SECRET')

user = intra.getUser('ID_OR_LOGIN')

print(f"""
        Login: {user['login']}
        Email: {user['email']}
        Full Name: {user['displayname']}
        Correction Points: {user['correction_point']}
        url: {user['url']}
""")
```
