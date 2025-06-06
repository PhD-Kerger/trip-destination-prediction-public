# Multi-Operator Free-Floating Trip Destination Prediction in Public Mobility Sharing Systems
Daniel Kerger, Prof. Dr. Heiner Stuckenschmidt
Data and Web Science Group, University of Mannheim, B 6, 26, Mannheim, 68159, Baden-Württemberg, Germany

## Abstract
Public mobility sharing systems are an important component of sustainable urban transportation, particularly for last-mile travel. Analyzing user behavior and trip patterns on public data is challenging due to rotating vehicle identifiers in open data standards such as GBFS. This paper presents a machine learning approach to predict trip destinations under these constraints, enabling the reconstruction of travel patterns without relying on persistent identifiers.

We develop a three-step prediction pipeline: (1) candidate generation and reduction using spatial-temporal filtering, (2) multi-target regression via XGBoost to estimate destination coordinates, and (3) selection of the closest matching candidate from the reduced set. We evaluate the approach using data from two public mobility operators across five German cities between April 2023 and May 2025. The model achieves up to 86\% accuracy within a 500-meter tolerance and 77\%. We further validate generalization across five additional datasets. Compared to existing approaches, our method improves prediction accuracy by up to 30\% over methods that do not use user-specific features and by up to 10\% over those that do, while halving the required tolerance radius.

These results demonstrate the feasibility of accurate destination prediction in shared mobility systems despite anonymized vehicle identifiers, supporting improved system analysis and planning.

## Usage
This repository contains the needed code to execute the pipeline used in our paper with a subset of the datasets from the city of Heidelberg. To run the notebook, install all dependencies listed in the requirements.txt file with Python 3.10. All results are displayed in the notebook output cells.

## Data Usage Restrictions
The dataset included in this repository is intended solely for use within the scope of reproducing the experiments described in our paper. It may not be used for other scenarios or purposes without explicit permission from the authors.
