# Contributing

Thank you for considering contributing to this project.

Please read the [Code of Conduct](./CODE_OF_CONDUCT.md) before getting started.

## Coding Standards

This projects uses the following tools to enforce coding standards.

- [`yamllint`](https://github.com/adrienverge/yamllint) to enforce coding standards in YAML files
- [`php-cs-fixer`](https://github.com/FriendsOfPHP/PHP-CS-Fixer) to enforce coding standards in PHP files
- [`composer-normalize`](https://github.com/ergebnis/composer-normalize) to normalize `composer.json`.

Coding standard violations are will be automatically reported in GitHub Actions.

Locally, the following command will attempt to fix all coding standard violations.

```bash
composer fix-standards
```

## Tests

This project uses [`phpunit`](https://phpunit.de/) to run unit tests and integration tests.

The following command will run the tests.

```bash
composer test
```

## Mutation Tests

This project uses [`infection`](https://infection.github.io/) to run mutation tests that ensure that we write quality tests.

The following command will run the mutation tests.

```bash
composer infect
```
