# Elixir Demo Application

This repository contains a simple Elixir application used to demonstrate GitHub Actions and cross-repository CI/CD workflows.

The project serves as the source application in a proof of concept where:

* Elixir tests are executed automatically on every push to the `main` branch.
* After the tests succeed, a GitHub Actions workflow triggers a Playwright end-to-end test suite located in a separate repository.
* The Playwright repository runs browser-based tests and publishes the test report as a workflow artifact.

## Purpose

This project demonstrates how to:

* Build a basic CI pipeline for an Elixir application.
* Trigger workflows in another GitHub repository using `workflow_dispatch`.
* Coordinate multiple repositories in a single CI/CD process.
* Integrate backend validation with end-to-end UI testing.

This repository is intended as a learning and demonstration project rather than a production application.

## Installation

If [available in Hex](https://hex.pm/docs/publish), the package can be installed
by adding `elixir_app` to your list of dependencies in `mix.exs`:

```elixir
def deps do
  [
    {:elixir_app, "~> 0.1.0"}
  ]
end
```

Documentation can be generated with [ExDoc](https://github.com/elixir-lang/ex_doc) and published on [HexDocs](https://hexdocs.pm).
Once published, the docs can be found at <https://hexdocs.pm/elixir_app>.
