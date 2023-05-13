# Contributing

Thank you for considering contributing to this project.

Please read the [code of conduct](./CODE_OF_CONDUCT.md) before getting started.

## Coding Standards

This projects uses the following tools to enforce coding standards.

- [`yamllint`](https://github.com/adrienverge/yamllint) to enforce coding standards in YAML files
- [`php-cs-fixer`](https://github.com/FriendsOfPHP/PHP-CS-Fixer) to enforce coding standards in PHP files
- [`composer-normalize`](https://github.com/ergebnis/composer-normalize) to normalize `composer.json`.

### Detecting
Coding standard violations are automatically reported in GitHub Actions.

Locally, the following command will report all coding standard violations.

```bash
composer standards
```

### Fixing

Coding standard violations may be fixed automatically by running the following command.

```bash
composer fix-standards
```

## Dependency Analysis

This project uses [`composer-require-checker`](https://github.com/maglnet/ComposerRequireChecker) 
to ensure that the source code does not depend on transitive dependencies.

Dependency analysis can be run with the following command.

```bash
composer analyse-dependencies
```

## Mutation Tests

This project uses [`infection`](https://infection.github.io/) to run mutation tests that ensure that we write quality tests.

The following command will run the mutation tests.

```bash
composer infect
```
