---
---

Formulários são a forma mais simples de coletar informações dos usuários. Um exemplo de formulário é apresentado abaixo. 

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Forms</title>
</head>
<body>
    <form>
        <input type="text" placeholder="First Name" name="first">
        <input type="password" placeholder="Password" name="password">
        <div>
            Favorite Color:
            <input name="color" type="radio" value="blue"> Blue
            <input name="color" type="radio" value="green"> Green
            <input name="color" type="radio" value="yellow"> Yellow
            <input name="color" type="radio" value="red"> Red
        </div>
        <input type="submit">
    </form>
</body>
</html>
```

![[Examplo de formulário HTML.png]]

Caso utilize o [[Django]] é possível implementar rapidamente um formulário utilizando a classe, rota e HTML a seguir: 

Classe:
``` python
from django import forms

class NameForm(forms.Form):
    your_name = forms.CharField(label='Your name', max_length=100)
```

Rota: 
```python
from django.http import HttpResponseRedirect
from django.shortcuts import render

from .forms import NameForm

def get_name(request):
    # if this is a POST request we need to process the form data
    if request.method == 'POST':
        # create a form instance and populate it with data from the request:
        form = NameForm(request.POST)
        # check whether it's valid:
        if form.is_valid():
            # process the data in form.cleaned_data as required
            # ...
            # redirect to a new URL:
            return HttpResponseRedirect('/thanks/')

    # if a GET (or any other method) we'll create a blank form
    else:
        form = NameForm()

    return render(request, 'name.html', {'form': form})
```

HTML: 
```html
<form action="/your-name/" method="post">
    {{ form }}
    <input type="submit" value="Submit">
</form>
```