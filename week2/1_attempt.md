# Auditing File

problems:
 1. column "Price" is missing one value - data is incomplete 
 code used - raw.isna().sum()
 planned decision: investigate - missing value could be 

 2. Duplicate values
 code used - raw.duplicated() 
 planned decision: retain - entirely possible for 2 values to be exact same 

 3. Price data type should be numeric, instead of obj
 code used - raw.info() 
 planned decision: correct - needs to be changed to the correct data type 

 4. Date should be in datetime format, instead of obj 
 code used - raw.info() 
 planned decision: correct - needs to be changed to the correct data type 

