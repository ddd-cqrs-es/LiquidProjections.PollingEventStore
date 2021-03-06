# Liquid Projections [![Build status](https://ci.appveyor.com/api/projects/status/5j2rboeh9vg8773w/branch/master?svg=true)](https://ci.appveyor.com/project/dennisdoomen/liquidprojections-pollingeventstore-ctw8n/branch/master)

## What is this?
A source-only Nuget package for event stores that cannot actively push events to [LiquidProjections](https://github.com/liquidprojections/LiquidProjections). It efficiently support multiple concurrent subscribers each interested in a different checkpoint without hitting the underlying event store concurrently.

## Important Notes
* The `PollingEventStoreAdapter` constructor takes an optional delegate of type `LogMessage` that you can use for logging to your framework of choice. You can also have it log more diagnostic messages by setting the `LIQUIDPROJECTIONS_DIAGNOSTICS` condition symbol.
