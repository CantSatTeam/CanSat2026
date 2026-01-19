# 2026 CSDCMS CanSat Competition: Coudln'tSat

This repository will contain the Couldn'tSat team's submission to the [2026 CSDCMS CanSat Competition](https://www.csdcms.ca/CanSat_info.html).

As specified in the [primary mission](https://www.csdcms.ca/Docs/CSDC_CanSat_Requirements_2024-25.pdf#page=7), our CanSat will collect air temperature and presssure data at a rate of no less than 1 Hz, and transmit this data to a ground station using LoRa radio.

Our CanSat has two main parts to its [secondary mission](https://www.csdcms.ca/Docs/CSDC_CanSat_Requirements_2024-25.pdf#page=7):
- Using a custom trained Monocular Height Estimation (MHE) model, it will use a single photo from an onboard downwards facing camera to generate a Digital Surface Map (DSM) of the launch site terrain.
- The CanSat will then use the MHE-generated DSM to determine a flat landing spot, and perform a guided landing using a paraglider.

Due to the amount of our code, we have split it into two other repositories:
1. [CanSat-MHE](https://github.com/CantSatTeam/CanSat-MHE), containing the code for MHE model training.
2. [CanSat-Flight](https://github.com/CantSatTeam/CanSat-Flight), containing the onboard and ground station code.
