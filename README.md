# Training: create a FHIR Implementation Guide

Hands-on session (HL7 Europe Working Group Meeting, Málaga 2026) to learn how to create your first FHIR Implementation Guide (IG) with a few artifacts written in FSH: a profile inheriting from the HL7 Europe profiles, a CodeSystem, a ValueSet and an example instance.

**Prerequisite:** a GitHub account. Everything is done on GitHub, no local installation is needed.

Training material: <https://nriss.github.io/create-ig-training/>

## How to use this template

1. Fork this repository (it must be **public**).
2. In `sushi-config.yaml`, set the `id` (`org.fhir.[realm].[code]`) and the `canonical` (an address you make up, ending with `/[code]`). Update the `ig` line of `ig.ini` accordingly.
3. Install the [FHIR IG Builder](https://github.com/apps/fhir-ig-builder) GitHub app on your fork, then commit: the [auto-builder](https://github.com/FHIR/auto-ig-builder) generates your IG in 2-3 minutes at `https://build.fhir.org/ig/<account>/<repository>/branches/<branch>`. Logs are listed at <https://build.fhir.org/ig/>.
4. Add the dependency `hl7.fhir.eu.base: 2.0.1` in `sushi-config.yaml`, then write your FSH artifacts in `input/fsh/`.

## Structure

* `sushi-config.yaml`: IG configuration (dependencies, pages, menu).
* `ig.ini`: IG Publisher configuration (IG resource, template).
* `input/fsh/`: FSH artifacts (profiles, extensions, ValueSets, CodeSystems, examples).
* `input/pagecontent/`: IG pages in Markdown (start at heading level `###`).

Based on [ansforge/IG-modele](https://github.com/ansforge/IG-modele).
