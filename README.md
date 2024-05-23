# Assessessment of Intergrated HV-LV OE Calculations to Orchestrate DERs - OE Algorithm 2: Asset Capacity

This repository is part of the project [Accelerating the Implementation of Operating Envelopes Across Australia](https://electrical.eng.unimelb.edu.au/power-energy/projects/accelerating-the-implementation-of-operating-envelopes-across-australia) funded by CSIRO. This project provided key metrics, recommendations, and guidance for distribution companies (known as Distribution Network Service Providers [DNSPs] in Australia) and AEMO (the Australian system operator) to assist them in improving and, hence, accelerating the use of Operating Envelopes (OEs) across Australia.

In this repository, we use interactive code via Jupyter Notebook and Python as well as a [realistic integrated high voltage and low voltage (HV-LV) network](https://github.com/Team-Nando/MV-LV-Networks) to demonstrate the process and necessary calculations for the *Asset Capacity OE Algorithm with Integrated HV-LV Calculation* produced by The University of Melbourne. This demonstration is useful for different stakeholders (e.g., DNSPs, AEMO, CSIRO, regulators, consultancy companies, technology providers) as it can help them familiarise with the corresponding algorithm and the required inputs as well as the pros and cons.

## Asset Capacity OE with Integrated HV-LV Calculation
The Asset Capacity OE is the simplest OE implementations investigated in the project. At a given moment in time, it only considers the spare thermal capacity of the distribution transformer (i.e., thermal capacity minus net demand of all the customers) and splits it among active customers. It is the least accurate OE approach as it does not consider voltage aspects.
- Required Monitoring: At the secondary of the transformer (aggregated P and aggregated Q per phase).
- Required Electrical Models: None.

For simplicity, the case study used to demonstrate the OE algorithm corresponds to a low voltage (LV) network without modelling the upstream high voltage (HV) network. Although some adaptations have been made to ensure realistic voltage fluctuations at the distribution transformer of the LV network, the results are not exactly the same as those presented in the Final Report of the project (which used an integrated HV-LV network model). Nevertheless, the behaviour of the OE algorithm and the qualitative nature of the results remain the same. 

## Pre-Requisites
- Python (Anaconda) and Jupyter Notebook (comes with Anaconda). For download links and more info: https://www.anaconda.com/download. Note that you must install the Anaconda that is compatible with your operating system (e.g., Windows, Mac). Also note that this repository is meant to be used by individuals (who can get free access to Anaconda).
- dss_python module. We use this Python-native module to run power flows based on OpenDSS (https://sourceforge.net/projects/electricdss/). To install, run `pip install dss_python` in the Anaconda Prompt. For more info: https://github.com/Team-Nando/Tutorial-DERHostingCapacity-0-dss_python#part-0-using-dss_python.
- To guarantee that you have all the necessary packages you can also run the **`requirements.txt`** file using **`pip install -r requirements.txt`** in the Anaconda prompt.

## Run the Code
Make sure you have installed all the pre-requisites (Anaconda, dss_python, requirements). Otherwise, you will not be able to go through the repository.

1. Download all the files using the green **`<> Code`** button at the top right.
   - You will get a ZIP file with a folder that contains all the files.
   - Unzip the file and place the folder somewhere on your computer/laptop.
2. To open the Jupyter Notebook file (extension **`ipynb`**) you need to:
   - Open Anaconda Navigator
   - Click on Launch Jupyter Notebook (it will open in your browser)
   - Upload the unzipped folder (with all the corresponding files) to Jupyter Notebook (the location is up to you)
   - Go inside the folder and open the **`ipynb`** file

All the instructions will be in the **`ipynb`** file.

## Credits

Arthur Gonçalves Givisiez (a.goncalvesgivisiez@unimelb.edu.au)

Nando Ochoa (luis.ochoa@unimelb.edu.au ; https://sites.google.com/view/luisfochoa)

## Licenses

Since this repository uses dss_python which is based on OpenDSS, both licenses have been included. This repository uses the BSD 3-Clause "New" or "Revised" license. Check all corresponding files (`LICENSE-OpenDSS`, `LICENSE-dss_python`, `LICENSE`).
