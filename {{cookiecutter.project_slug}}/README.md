{% for _ in cookiecutter.project_name %}={% endfor %}
{{ cookiecutter.project_name }}
{% for _ in cookiecutter.project_name %}={% endfor %}

## Contributing

This project uses [Makefile.venv](https://github.com/sio/Makefile.venv) which
takes care of creating, updating and invoking Python virtual environment.

### Makefile Targets

*Makefile.venv* provides useful Python-related targets for managing virtual environment.
Some are meant to be executed directly via `make $target`, some are meant to be dependencies for other targets.

| Make Target  | Description |
| ------------ | ----------- |
| `venv`       | Use this as a dependency for any target that requires virtual environment to be created and configured. |
| `python`     | Launch interactive Python shell within virtual environment. |
| `ipython`    | Launch interactive Python shell within virtual environment. Note: IPython is not installed by default when creating the virtual environment but will be installed automatically when called for the first time. |
| `show-venv`  | Show versions of Python and pip, and the path to the virtual environment. |
| `clean-venv` | Remove virtual environment. Included in `clean` |

