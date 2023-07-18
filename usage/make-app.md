---
description: No more spaghetti code. Ever.
---

# Make app

### `swiftly makeapp`

```batch
swiftly makeapp incredibleapp
```

This creates a new folder by the name `incredibleapp` and gives you default files to work with.

**You can also create nested apps:**

```batch
swiftly makeapp models.regression
```

This creates an app inside an existing app `models`. This allows you to keep the organisation while maintaining a very modular codebase. You can nest as much as you like using the "." notation.

Eg: `models.regression.linear`

### Swiftly App

This is a file structure that has been perfected after years of building projects and one that keeps huge projects so manageable that it's almost magic. It's a simple structure with a very simple philosophy.

> Philosophy: A new functionality is a new app. Apps are nested if their functionality is a part of a bigger app.
>
>
>
> Eg: `models` is a new functionality, hence it's a new app. If you now wanna add regression and knn as 2 other functionalities, but it's a part of models, so you can create `models.regression` and `models.knn`

**Structure:**

```
models
├── __init__.py
├── __main__.py
├── models.py
└── tests.py
```

#### `__init__.py`

This file acts as the face of you project. It makes your folder into a python package that can be imported by other files in the project.

{% code title="__init__.py" %}
```python
from .models import *
```
{% endcode %}

Then, inside another app you can use everything from models app like this:

{% code title="anotherapp.py" %}
```python
from models import a_function_in_models
```
{% endcode %}



#### `__main__.py`

The reason to have this file is to make sure you can see how it feels like to work with the app you just wrote. Everything that used to go inside `if __name__ == "__main__"` can now go inside this file.

This way, the main codebase for the app remains clutter free, and it's just one file that a developer needs to see to know how to operate with your app.



#### `app_name.py`

This file is the main codebase for the app. By default it has a function or a class predefined to work with, but you can change it to any way you like. This is where all your awesome logic goes.



#### `tests.py`

This is a file where you can run tests for checking the code inside `app_name.py`
