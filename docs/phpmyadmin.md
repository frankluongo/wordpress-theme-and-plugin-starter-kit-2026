# Adding PHP My Admin

## Update `.wp-env.json` file:

The `phpmyadminPort` NEEDS to be different between environments.

```json
{
  "$schema": "https://schemas.wp.org/trunk/wp-env.json",
  "phpmyadminPort": 8080,
  "env": {
    "tests": {
      "phpmyadminPort": 8081
    }
  }
}
```