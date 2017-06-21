# Spectral sensor data

Storing spectral data

* Management Tips:
    - Back up all data to at least 2 separate locations
    - Store data by project first, then date of flight
    - Keep all "raw" imagery 
    - Metadata to keep (in the form of filenames)
        * Date of flight (year.month.day)
        * Platform utilized
        * Altitude flown
        * Sensor type
        * Location
        * Pertinent weather information (anything that will affect the data output-- clouds, excessive wind, etc...)
    - Use metadata information to name exports of data to efficiently describe the dataset
        * year.month.day, location, platform, sensor, altitude, additional descriptor(s)
            - For example, an exported orthomosiac would have the name: *2017.06.21 FarmLocation S1000 RedEdgeNIR 400ft Windy*
            - Additional descriptors can tell the end user why the data set turned out the way it did. "Windy" can indicate that some of the pictures couldn't stitch together, which would explain why there would be holes in a data set
            - Metadata should be arranged in a way that makes sense for the project. If the main goal of a dataset is to compare outputs of different altitudes then move the atltitude in the front of the name, or put it last, so that it can be quickly spotted.
     - When working with photogrammetric processing software (in which you cannot just 'undo' mistakes, save new files along the way with a descriptor at the end
        * Example: 2017.06.21 AgisoftPhotoscanDataset Before Refinement

        
* Outline of suggested file format naming:
    - Project/Customer
      * Platform
         - Date, Location, Sensor (if same sensor was used for all flights that day)
            * Altitude
            * GCP
                - Sensor
                    * Raw
                    * JPEG
                    * Video
                    * Exports 
                    * ...

    - This is a good example for organizing data in which data from different platfroms have different applications, and different sensors may be flown at different altitudes on one day at one location. File formatting should be made standard across all projects and naming conventions should make sense so that someone outside of the project could go in and locate a specific data set.
        
