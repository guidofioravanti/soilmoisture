

| Name| Description| Source|
|-----|------------|-------|
| ESA-CCI passive| The daily data have been downloaded and the 10-day composites created as a "mean" of the corresponding daily data. | [https://www.esa-soilmoisture-cci.org/](https://www.esa-soilmoisture-cci.org/) |
| ESA-CCI passive from C3S | The 10-day and monthly composites are available for CDR (Climate Data Record) and ICDR (Intermediate Climate Data Record). CDR terminates in 2020, ICDR continues up to 2023. | [https://cds.climate.copernicus.eu/cdsapp#!/dataset/satellite-soil-moisture?tab=overview](https://cds.climate.copernicus.eu/cdsapp#!/dataset/satellite-soil-moisture?tab=overview)|
| LISFLOOD | | |
| ASCAT    |-|-|

## ESA-CCI PASSIVE PRODUCT

The 10-day composite constructed by means of the daily data (Guido's composite) does not match the 10-day composite available through C3S (Copernicus' composite).

Two main differences:

- data value (the Copernicus' composite is the average of the daily data? Yes, according to the manual product)
- spatial gaps (the Copernicus' composite seems to be gap-filled, large areas with missing values in Guido's composites have values in the corresponding Copernicus' composite)

### ESA-CCI PASSIVE PRODUCT ICDR from C3S

The documentation is available [here](https://datastore.copernicus-climate.eu/documents/satellite-soil-moisture/C3S_312b_Lot4.D3.SM.5-v3.0_202101_Product_User_Guide_Specification_i1.0.pdf).

In particular:

```
1.2 ICDR
The Intermediate Climate Data Record is a consistent extension of the CDR. The ICDR products are generated every dekad (approx. 10 days) and extend the CDR of the same version as the ICDR. The
same algorithm and software processor are used for generating the ICDR products, also input parameter are reused. New near real time observation data from the ASCAT-A/B and AMSR2 and
SMOS sensors (Table 23) are processed to extend the ICDR products.
```

### ESA-CCI PASSIVE PRODUCT ICDR from C3S: issues

- 1.5.1.1 Vegetation
- 1.5.1.2 Frozen surfaces and snow
- 1.5.1.3 Water bodies
- 1.5.1.4 Rainfall
- 1.5.1.5 Radio Frequency interference
- 1.5.1.6 Using night-time observations only

IMPORTANT (can this explain the difference between Guido's 10-day composites and Copernicus' 10-day composites?)

```
For the current version of the merged passive product only descending overpasses, corresponding to night-time / early morning observations, were considered. This is because near surface land surface
temperature gradients are regarded to be reduced at night leading to more robust retrievals (Owe et al., 2008). However, (Brocca et al., 2011) suggest that for specific land cover types day-time
observations may provide more robust retrievals than night-time observations, although the exact causes are still unknown. If day-time observations could be introduced to the blended product, this
would significantly increase the observation density.
```
