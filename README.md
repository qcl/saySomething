saySomething
----
A simple service which provides a web interface to let user can type something in a textarea, then use a system command `say` to say something.

# Route design

`/` `GET` - home page, redirect to `/say`

`/say` `GET` - provide a `<textarea>`, let user type text in, when user click submit button, **POST** those text to `/say`

`/say` `POST` - call system command `say` to say something.

`/said` `GET` - show sentences which had been said.