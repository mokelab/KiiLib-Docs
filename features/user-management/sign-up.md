---
layout: default
baseName: index
---

# Sign up

Kii Cloud allows users to register with the following combinations.

- username/password combination.
- phone numbers/password combination.
- email address/password combination.

When assigning an email address or phone number to a user, you can let Kii Cloud take the steps necessary to verify the credentials (either through a verification email or an SMS).

## Sign up with username/password combination.

The following snippet shows how to sign up a user with the username `user_123456` and a password `123ABC`.

### Java

{% highlight java %}

{% endhighlight %}

### Python

{% highlight python %}

import kiilib

context = kiilib.KiiContext({APP_ID}, {APP_KEY}, {BASE_URL})
app = kiilib.AppAPI(context)

login = 'user_123456'
password = '123ABC'
user = app.signup(login, password)
print user

{% endhighlight %}

### PHP

{% highlight php %}
<?php

?>
{% endhighlight %}

### TypeScript

{% highlight typescript %}

{% endhighlight %}

## Sign up with phone numbers/password combination.

The following snippet shows how to sign up a user with the phone number `+819012345678` and a password `123ABC`.

### Java

{% highlight java %}

{% endhighlight %}

### Python

{% highlight python %}

import kiilib

context = kiilib.KiiContext({APP_ID}, {APP_KEY}, {BASE_URL})
app = kiilib.AppAPI(context)

login = None
phone = '+819012345678'
password = '123ABC'
user = app.signup(login, password, phoneNumber = phone)
print user

{% endhighlight %}

### PHP

{% highlight php %}
<?php

?>
{% endhighlight %}

### TypeScript

{% highlight typescript %}

{% endhighlight %}

## Sign up with email address/password combination.

The following snippet shows how to sign up a user with the email address `user_123456@example.com` and a password `123ABC`.

### Java

{% highlight java %}

{% endhighlight %}

### Python

{% highlight python %}

import kiilib

context = kiilib.KiiContext({APP_ID}, {APP_KEY}, {BASE_URL})
app = kiilib.AppAPI(context)

login = None
email = 'user_123456@example.com'
password = '123ABC'
user = app.signup(login, password, emailAddress = email)
print user

{% endhighlight %}

### PHP

{% highlight php %}
<?php

?>
{% endhighlight %}

### TypeScript

{% highlight typescript %}

{% endhighlight %}
