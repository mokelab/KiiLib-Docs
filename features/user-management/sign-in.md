---
layout: default
baseName: index
---

# Sign in

Once users are registered with your application (after completing the user verification process if required) they will be able to sign in with their username, phone number or email address. When users sign in, they are granted an access token. It is stored in a context object given to API instance.

## Sign in with username/password combination.

The following snippet shows how to sign in with the username `user_123456` and a password `123ABC`.

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
user = app_api.login(login, password)
print 'access_token:%s\nuser_id:%s' % (context.access_token, user.id)

{% endhighlight %}

### PHP

{% highlight php %}
<?php

?>
{% endhighlight %}

### TypeScript

{% highlight typescript %}

{% endhighlight %}

## Sign in with email address/password combination.

The following snippet shows how to sign in with the email address `user_123456@example.com` and a password `123ABC`.

### Java

{% highlight java %}

{% endhighlight %}

### Python

{% highlight python %}

import kiilib

context = kiilib.KiiContext({APP_ID}, {APP_KEY}, {BASE_URL})
app = kiilib.AppAPI(context)

email = 'user_123456@example.com'
password = '123ABC'
user = app_api.login(email, password)
print 'access_token:%s\nuser_id:%s' % (context.access_token, user.id)

{% endhighlight %}

### PHP

{% highlight php %}
<?php

?>
{% endhighlight %}

### TypeScript

{% highlight typescript %}

{% endhighlight %}

## Sign in with phone numbers/password combination.

The following snippet shows how to sign in with the phone number `+819012345678` and a password `123ABC`.

### Java

{% highlight java %}

{% endhighlight %}

### Python

{% highlight python %}

import kiilib

context = kiilib.KiiContext({APP_ID}, {APP_KEY}, {BASE_URL})
app = kiilib.AppAPI(context)

phone = '+819012345678'
password = '123ABC'
user = app_api.login(phone, password)
print 'access_token:%s\nuser_id:%s' % (context.access_token, user.id)

{% endhighlight %}

### PHP

{% highlight php %}
<?php

?>
{% endhighlight %}

### TypeScript

{% highlight typescript %}

{% endhighlight %}
