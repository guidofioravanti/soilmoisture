

| Name| Description| Source|
|-----|------------|-------|
| ESA-CCI passive| The daily data have been downloaded and the 10-day composites created as a "mean" of the corresponding daily data. | [https://www.esa-soilmoisture-cci.org/](https://www.esa-soilmoisture-cci.org/) |
| ESA-CCI passive from C3S | The 10-day and monthly composites are available for CDR (Climate Data Record) and ICDR (Intermediate Climate Data Record). CDR terminates in 2020, ICDR continues up to 2023. | [https://cds.climate.copernicus.eu/cdsapp#!/dataset/satellite-soil-moisture?tab=overview](https://cds.climate.copernicus.eu/cdsapp#!/dataset/satellite-soil-moisture?tab=overview)|
| LISFLOOD | | |
| ASCAT    |-|-|

## ESA-CCI PASSIVE PRODUCT

The 10-day composite constructed by means of the daily data (Guido's composite) does not match the 10-day composite available through C3S (Copernicus' composite).

Two main differences:

- data value (the Copernicus' composite is the average of the daily data? Check it)
- spatial gaps (the Copernicus' composite seems to be gap-filled, large areas with missing values in Guido's composites have values in the corresponding Copernicus' composite)

### ESA-CCI PASSIVE PRODUCT ICDR from C3S

The documentation is available [here](https://datastore.copernicus-climate.eu/documents/satellite-soil-moisture/C3S_312b_Lot4.D3.SM.5-v3.0_202101_Product_User_Guide_Specification_i1.0.pdf).

In particular:

```
1.2 ICDR
The Intermediate Climate Data Record is a consistent extension of the CDR. The ICDR products are
generated every dekad (approx. 10 days) and extend the CDR of the same version as the ICDR. The
same algorithm and software processor are used for generating the ICDR products, also input
parameter are reused. New near real time observation data from the ASCAT-A/B and AMSR2 and
SMOS sensors (Table 23) are processed to extend the ICDR products.
```
