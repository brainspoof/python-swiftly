---
description: Initialise your project; any way you like!
---

# Init

## New project

### `swiftly init <awesome-project-name>`

If you are starting a fresh new project, swiftly provides a command to make the setup one liner.

{% tabs %}
{% tab title="MacOS / Linux" %}
```bash
source swiftly init awesomeproject
```

Using source allows you to use swiftly to the fullest. It automatically activates the virtual environment and put in the project's directory so you can get to coding right away!
{% endtab %}

{% tab title="Windows" %}
```batch
swiftly init awesomeproject
```
{% endtab %}
{% endtabs %}

***

### `swiftly init <git-repo-url>`

If you have a repo you want to start working on; even if it's not a swiftly project, you can still use swiftly to work with it.

{% hint style="info" %}
You must have git cli already setup for this to work.
{% endhint %}

{% tabs %}
{% tab title="MacOS / Linux" %}
```bash
source swiftly init git@github.com:brainspoof/awesomeproject.git
```

Using source allows you to use swiftly to the fullest. It automatically activates the virtual environment and put in the project's directory so you can get to coding right away!
{% endtab %}

{% tab title="Windows" %}
```batch
swiftly init git@github.com:brainspoof/awesomeproject.git
```
{% endtab %}
{% endtabs %}

***

## Existing project

* [x] Check git repo for changes
* [x] Install any uninstalled requirements
* [x] Check swiftly project's integrity
* [x] Activate virtual environment
* [x] Swiftly done!

### `swiftly init`

To initialise the swiftly project the next time you go to work on it is super simple. Just go inside the project and run the one magical command

{% tabs %}
{% tab title="MacOS / Linux" %}
```bash
source swiftly init
```

Using source allows you to use swiftly to the fullest. It automatically activates the virtual environment and put in the project's directory so you can get to coding right away!
{% endtab %}

{% tab title="Windows" %}
```batch
swiftly init
```
{% endtab %}
{% endtabs %}

***

### `swiftly init <awesome-project-name>`

You can also activate an exiting project by just writing the name of the project. This works if you are not already inside your swiftly project, but just on folder outside it.

{% tabs %}
{% tab title="MacOS / Linux" %}
```bash
source swiftly init awesomeproject
```

Using source allows you to use swiftly to the fullest. It automatically activates the virtual environment and put in the project's directory so you can get to coding right away!
{% endtab %}

{% tab title="Windows" %}
```batch
swiftly init awesomeproject
```
{% endtab %}
{% endtabs %}

***
