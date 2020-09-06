# donations_part_II

Analysis of donations to anonymous charity, 2013-2017

##### __Data__
* Originally provided in a json file, converted to csv (was told most of columns were retained).
* 2,024,554 entries
* 92 original columns (because of conversion to tabular format)

##### Organization of notebooks
1_donation_export_cohort_create_dataframes
* Read in and clean up data; create dataframes to work with
  - donations_df (original read of csv)
  - donations (additional columns, converted cents to dollars, etc.)
  - donations <-- PICKLE created
  - donations_13to17 (only donors who donated 2013-2017; removed other cohorts) <-- PICKLE created
  - donations_13to17_sample <-- CSV created
 
2_create_cohort_dataframes
* Use donations_13to17.pkl to create dataframes for each cohort
  - cohort13, cohort14, cohort15, cohort16, cohort17 <-- PICKLES created

3_analysis_of_donor_makeup_over_time
* Divide donors into categories and analysis by number and amount given over time.
  - new
  - retain
    - upgrade
    - downgrade
    - maintain
  - recover
  - lapse
    - first
    - again
* Analyze donation gain/loss over time
  - Gain
    * new
    * retain (upgrade margin)
    * recover
  - Same
    * maintain
    * upgrade base
    * downgrade base
  - Loss
    * lapse
      - first
      - again
    * retain (downgrade margin)
    
  -


