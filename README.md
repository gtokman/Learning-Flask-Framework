# Flask Basics

The JSON library docs. 99% of the time, you won't need anything more than .loads() and .dumps().

## New Terms

* **url_for()**: This function, always available in templates but importable in your app, finds the URL for a given view function name.

* **redirect()**: This function returns an HTTP redirect to whatever URL is provided.

* **Response**: A response is the data that the server, Flask, sends back to the client.

* **make_response()**: This function generates the entire response object that'll be sent back to the client, but lets you store it in a variable for further manipulation.

* **response.set_cookie()**: Sets a cookie on the response object. Takes name for the cookie and a value.

* **json.dumps()**: This method turns a Python data structure (list, string, dictionary, etc) into a JSON string.

* **json.loads()**: This method turns a JSON string into a Python object.


```{% for x in y %} 
```
* You already know what for x in y: does in Python, but this is the template version. This will cause the enclosed code to be run as many times as there are things in y. Has to be followed by {% endfor %}.

```
{% if %}
```
* The template version of Python's if condition. Closed with {% endif %}.

* **flash()**: This function stores a message in the session that will self-destruct after the response is returned.

* **get_flashed_messages()**: This function gets all of the flash messages stored in the session.

* **app.secret_key**: This configuration attribute stores the secret key that all messages are cryptographically signed with.

```
{% with %}
```
* The Flask template version of Python's with block. Let's you temporarily define a variable. Must be closed with {% endwith %}.