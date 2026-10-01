# Ecological Species Identification Pipeline

Research pipeline for evaluating species identification in complex crowdsourced ecological imagery.

The system studies whether target localization improves biological foundation model species identification and how localization, description strategy, and uncertainty affect downstream performance.

## System Contract

Input:

- ecological image
- target description

Output:

- one species prediction
- or abstention for human review

## Research Questions

The project investigates:

1. How well biological foundation models identify target species directly
   from complex ecological images.

2. Whether target localization improves species identification.

3. How target-description strategy affects localization and downstream
   classification.

4. How errors propagate through the pipeline and how reliably the system
   can abstain from uncertain predictions.

## Repository Structure

```text
configs/       Experiment configuration
data/          Raw, interim, processed, and annotation data
docs/          Research and experiment documentation
manifests/     Versioned dataset and candidate-space metadata
notebooks/     Inspection, visualization, and exploratory analysis
runs/          Individual experiment outputs and run manifests
src/           Core implementation
tests/         Automated validation and evaluation tests