### About

The `Python` application utilizes `Flask` for effective API management. When `XSUAA` is enabled, a `decorator` helper is in place to seamlessly check for `authorization` and `authentication`.

The project configuration may vary depending on whether `XSUAA` (SAP Cloud Foundry service for authorization and authentication) is enabled or not.

```bash
|---python
|   |---Procfile
|   |---requirements.txt
|   |---server.py
|   |---xsuaa_check.py
```

!!! note "If XSUAA is enabled"

    To ensure proper configuration of your frontend application, you will need to include a `.env` file in the `root` directory of the frontend project. This file should contain the necessary environment variables and configurations for `VCAP_SERVICES` and `VCAP_APPLICATION`.

Here is an example for the same:

![UI5](../../../assets/env.png){width="50%"}


### Usage Instructions

!!! note "If XSUAA is enabled"    

To check if the user is authorized, you can use the decorator function `auth()`

```py
@app.route('/home')
@auth()
```

To check if the user is authorized & has a role, you can use the decorator function `auth('<role>)`

```py
@app.route('/home')
@auth(scopes='import,export')
```

To start the application simply run:

Python
```console
python server.py
```

Flask
```console
flask --app <appname>
```