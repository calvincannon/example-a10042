# Emacs Config

Bundle to manage my emacs config, its pretty generic though and serves as a simple example.


Example Configuration:

```
bundle common nickanderson_emacs_config_settings
# @brief Settings that I like for emacs
{
  vars:
    "config[template]"
      string => "$(this.promise_dirname)/templates/nickanderson.emacs.mustache";

    "config[path]"
      string => "/home/nickanderson/.emacs";
}
```


Example Usage:

```
bundle agent go
{
  methods:
    "emacs" usebundle => emacs_config("nickanderson_emacs_config_settings");
}
```
