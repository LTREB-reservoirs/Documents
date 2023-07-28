# Protocols for setting up CI using ACCESS, Jetstream2, and Open Storage Network

## Requests ACCESS credits

1) Request "Explorer" allocation credits
2) Here is the requestion we used

   title: Integrating real-time open data pipelines and forecasting to quantify ecosystem predictability at day to decadal scales
   Abstract: The project is an NSF-funded Long Term Research in Environmental Biology project focused on quantifying our capacity to forecast a range of physical, chemical, and biological variables in two freshwater reservoirs. The project is hosting a forecasting challenge that encourages teams to develop and submit forecasts of the monitored variables before the data is collected. We will be using ACCESS resources as follows: 1) a m3.large VM running on Jetstream2 with a rocker container (https://rocker-project.org) to automatically (via cron jobs) download weather forecasts that are made available to teams, generate baseline (null) forecasts, and evaluate forecasts, 2) a m3.small VM running on Jetstream2 that handles forecast submission processing, and 3) 2 TB of cloud storage on the Open Storage Network where the downloaded weather forecasts, archived forecasts, and scored forecasts are storage and made publicly available. We have experience setting up a similar system as part of Thomas et al. 2023 (https://doi.org/10.1002/fee.2616)

   You will need your NSF CV and the grant information that is available through NSF.

4) Spend allocation credits

## Set up subdomains on webaddress

submit.ltreb-reservoirs.org
rstudio.ltreb-reservoirs.org

## Setting up Virtual Machines on Jetstream2

We use two virtual machines.  The first is a larger machine that has a GitHub action runner on it that handles jobs that can't run on GH Action free resources.  The second is a VM that runs MINIO and rstudio rocker to process submissions and move them to Open Storage Network.

### Submission VM

MINIO

### Self-hosted Runner VM

## Setting up storage on Open Storage Network
