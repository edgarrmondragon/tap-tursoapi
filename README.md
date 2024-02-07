# `tap-tursoapi`

Singer tap for TursoAPI.

Built with the [Meltano Tap SDK](https://sdk.meltano.com) for Singer Taps.

## Capabilities

* `catalog`
* `state`
* `discover`
* `about`
* `stream-maps`

## Settings

- [ ] `Developer TODO:` Declare tap settings here.

A full list of supported settings and capabilities is available by running: `tap-tursoapi --about`

### Source Authentication and Authorization

- [ ] `Developer TODO:` If your tap requires special access on the source system, or any special authentication requirements, provide those here.

## Usage

You can easily run `tap-tursoapi` by itself or in a pipeline using [Meltano](https://meltano.com/).

### Executing the Tap Directly

```bash
tap-tursoapi --version
tap-tursoapi --help
tap-tursoapi --config CONFIG --discover > ./catalog.json
```

## Developer Resources

- [ ] `Developer TODO:` As a first step, scan the entire project for the text "`TODO:`" and complete any recommended steps, deleting the "TODO" references once completed.

### Initialize your Development Environment

```bash
pipx install hatch
```

### Create and Run Tests

Run integration tests:

```bash
hatch run tests:integration
```

You can also test the `tap-tap-tursoapi` CLI interface directly:

```bash
hatch run sync:console -- --about --format=json
```

### Testing with [Meltano](https://www.meltano.com)

_**Note:** This tap will work in any Singer environment and does not require Meltano.
Examples here are for convenience and to streamline end-to-end orchestration scenarios._

Your project comes with a custom `meltano.yml` project file already created. Open the `meltano.yml` and follow any _"TODO"_ items listed in
the file. Go ahead and [install Meltano](https://docs.meltano.com/getting-started/installation/) if you haven't already.

1. Install all plugins

   ```bash
   meltano install
   ```

1. Check that the extractor is working properly

   ```bash
   meltano invoke tap-tap-tursoapi --version
   ```

1. Execute an ELT pipeline

   ```bash
   meltano run tap-tap-tursoapi target-jsonl
   ```

### SDK Dev Guide

See the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the SDK to
develop your own taps and targets.
