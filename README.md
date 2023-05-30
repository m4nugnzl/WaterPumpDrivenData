# WaterPumpDrivenData

The goal is to predict the status of a waterpoint for each record in the dataset. We have the following set of variables:

* `amount_tsh` - Total static head (amount of water available)
* `date_recorded` - The date the data was recorded
* `funder` - Who funded the well
* `gps_height` - Altitude of the well
* `installer` - Organization that installed the well
* `longitude` - GPS coordinate (longitude)
* `latitude` - GPS coordinate (latitude)
* `wpt_name` - Name of the waterpoint if there is one
* `num_private` - Not specified
* `basin` - Geographic water basin
* `subvillage` - Geographic location
* `region` - Geographic location (region)
* `region_code` - Geographic location (region code)
* `district_code` - Geographic location (district code)
* `lga` - Geographic location (district)
* `ward` - Geographic location (ward)
* `population` - Population around the well
* `public_meeting` - True/False
* `recorded_by` - Group that entered this row of data
* `scheme_management` - Who operates the waterpoint
* `scheme_name` - Name of the scheme that operates the waterpoint
* `permit` - If the waterpoint is permitted
* `construction_year` - Year the waterpoint was constructed
* `extraction_type` - The extraction type of the waterpoint
* `extraction_type_group` - The extraction type group of the waterpoint
* `extraction_type_class` - The extraction type class of the waterpoint
* `management` - How the waterpoint is managed
* `management_group` - The management group of the waterpoint
* `payment` - What the water costs
* `payment_type` - The payment type for water
* `water_quality` - The quality of the water
* `quality_group` - The quality group of the water
* `quantity` - The quantity of water
* `quantity_group` - The quantity group of the water
* `source` - The source of the water
* `source_type` - The source type of the water
* `source_class` - The source class of the water
* `waterpoint_type` - The type of waterpoint
* `waterpoint_type_group` - The type group of the waterpoint
The provided files are as follows:

* `train_values.csv`: file with the set of variables and observations used for training the model.
* `train_labels.csv`: file with the target variable for each observation in train_values.csv:
  * *functional*
  * *non functional*
  * *functional needs repair*
* `test_values.csv`: test file used to maximize the predictions obtained with the corresponding model.
Throughout the notebook, I will comment on the different tests I have performed on the model and how they affect the score of predictions on the test dataset.


The model created got a score of `0.6265` in drivendata
