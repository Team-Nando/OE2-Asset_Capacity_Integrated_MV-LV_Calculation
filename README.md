# Assessment of Integrated MV-LV OE Calculations to Orchestrate DERs - OE Algorithm 2: Asset Capacity

This repository is part of the project [Accelerating the Implementation of Operating Envelopes Across Australia](https://electrical.eng.unimelb.edu.au/power-energy/projects/accelerating-the-implementation-of-operating-envelopes-across-australia) funded by CSIRO. This project provided key metrics, recommendations, and guidance for distribution companies (known as Distribution Network Service Providers [DNSPs] in Australia) and AEMO (the Australian system operator) to assist them in improving and, hence, accelerating the use of Operating Envelopes (OEs) across Australia.

In this repository, we use interactive code via Jupyter Notebook and Python as well as a [realistic integrated medium voltage and low voltage (MV-LV) network](https://github.com/Team-Nando/MV-LV-Networks) to demonstrate the process and necessary calculations for the *Asset Capacity OE Algorithm with Integrated MV-LV Calculation* produced by The University of Melbourne. This demonstration is useful for different stakeholders (e.g., DNSPs, AEMO, CSIRO, regulators, consultancy companies, technology providers) as it can help them familiarise with the corresponding algorithm and the required inputs as well as the pros and cons.

## Asset Capacity OE with Integrated MV-LV Calculation
The Asset Capacity OE with Integrated MV-LV Calculation is the least advanced and, hence, the least accurate OE approach investigated in the project. However, its implementation is very simple since it needs very limited monitoring and no network model – it only needs the monitoring of few locations of the integrated MV-LV network (MV and LV HoFs), the capacity of few elements (distribution transformers as well as MV and LV HoFs), and an estimation of the aggregated net demand of flexible customers of each LV network. Nevertheless, by design, this approach does not solve voltage problems.
- Required Monitoring: At MV and LV head of feeders (P, Q, and V, all per phase).
- Required Electrical Models: None.

## Run the Code
Choose one of the options below to run the code.

### A. Cloud Option ☁️: Google Colab
Just click on the badge <a target="_blank" href="https://colab.research.google.com/github/Team-Nando/OE2-Asset_Capacity_Integrated_MV-LV_Calculation/blob/main/OE2-Asset_Capacity_Integrated_MV-LV_Calculation.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"/></a>. You don't need to install anything 🤓💪.

### B. Local Option 💻: Jupyter Notebook 
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
Arthur Gonçalves Givisiez (a.goncalvesgivisiez@unimelb.edu.au) <br>
Andres Avila Rojas (aavilarojas@student.unimelb.edu.au)  
Nando Ochoa (luis.ochoa@unimelb.edu.au ; https://sites.google.com/view/luisfochoa)

## Acknowledgements
We acknowledge AusNet Services for providing the data listed below, which was essential to create this repository.
- Anonymised historical active power demand of some customers (smart meter data)
- The data (i.e., topology, impedances, distribution transformers) of one of their MV feeders (indirectly used by this repository)

More details of this data can be found in the [Team Nando GitHub repository for Australian MV-LV Networks](https://github.com/Team-Nando/MV-LV-Networks), files named "Network_4_Urban_CRE21" and "Profiles".

We also acknowledge the Australian Bureau of Meteorology for providing the solar radiation data.

## Licenses
Since this repository uses dss_python which is based on OpenDSS, both licenses have been included. This repository uses the BSD 3-Clause "New" or "Revised" license. Check all corresponding files (`LICENSE-OpenDSS`, `LICENSE-dss_python`, `LICENSE`).
