# utl-what-are-the-hourly-air-temperatures-in-New-York-City-Central-Park-using-site-weather-dot-gov
what is the hourly air temperatures in New York City Central Park using site weather dot gov
    %let pgm=utl-what-are-the-hourly-air-temperatures-in-New-York-City-Central-Park-using-site-weather-dot-gov;

    what is the hourly air temperatures in New York City Central Park using site weather dot gov

    github
    https://tinyurl.com/yc5ekzdx
    https://github.com/rogerjdeangelis/utl-what-are-the-hourly-air-temperatures-in-New-York-City-Central-Park-using-site-weather-dot-gov

    stackoverflow
    https://tinyurl.com/ycx5h43k
    https://stackoverflow.com/questions/79067346/date-parameter-errors-with-weather-gov-api

    Solution by
    https://stackoverflow.com/users/646761/margusl


    Related repos

    REPO
    ---------------------------------------------------------------------------------------------------------------
    https://github.com/rogerjdeangelis/utl-scrape-weather-conditions-for-a-past-march-red-sox-vs-orioles-game-
    https://github.com/rogerjdeangelis/utl-scraping-san-francisco-hourly-weather-forecast-reading-xml-on-the-web
    https://github.com/rogerjdeangelis/utl_last_80_years_of_daily_weather_data_for_BWI_airport_from_noaa

    /*               _     _
     _ __  _ __ ___ | |__ | | ___ _ __ ___
    | `_ \| `__/ _ \| `_ \| |/ _ \ `_ ` _ \
    | |_) | | | (_) | |_) | |  __/ | | | | |
    | .__/|_|  \___/|_.__/|_|\___|_| |_| |_|
    |_|
    */

    /**************************************************************************************************************************/
    /* PRODUCE THIS GRAPH                                                                                                     */
    /*                                                                                                                        */
    /* HISTORIC AIR TEMPERATURES FOR NEW YORK CITY, CENTRAL PARK                                                              */
    /* =========================================================                                                              */
    /*                                                                                                                        */
    /*         10/07/2024 NOON TO 10/09/2024 MIDNIGHT BY HOURLY TEMPERATURES        SD1.RWANT total obs=57                    */
    /*                                                                                                                        */
    /*           000000000000000000000000000000000000000000000000000000001           ROWNAMES    DAYHR    AIRTEMP             */
    /*           777777777777888888888888888888888888999999999999999999990                                                    */
    /*           TTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTT               1       09T23     60.98              */
    /*           111111112222000000000011111111112222000000001111111122220               2       09T22     62.96              */
    /*           234567890123012345678901234567890123013456781234568901230               3       09T21     64.94              */
    /*      P ---++++++++++++++++++++++++++++++++++++++++++++++++++++++++---             4       09T20     66.92              */
    /*     80 +                                                            + 80          5       09T19     66.02              */
    /*     79 +  HISTORIC AIR TEMPERATURES FOR NEW YORK CITY, CENTRAL PARK + 79         ...                                   */
    /*     78 +    from 10/07/2024 Noon to 10/09/2024 Midnight by hours    + 78         53       07T15     71.96              */
    /*   N 77 +                                                            + 77 N       54       07T14     66.92              */
    /*   Y 76 +               latitude = "40.71"                           + 76 Y       55       07T13     66.02              */
    /*   C 75 +      *  75    longitude = "-74.00"                         + 75 C       56       07T13     66.02              */
    /*     74 +       *                                                    + 74         57       07T12     64.94              */
    /*   C 73 +        *      start = "2024-10-07T12:00:00Z"               + 73 C                                             */
    /*   E 72 +     *   *     end   = "2024-10-09T23:59:59Z"               + 72 E                                             */
    /*   N 71 +          *                                                 + 71 N                                             */
    /*   T 70 +                                                            + 70 T                                             */
    /*   R 69 +                                                            + 69 R                                             */
    /*   A 68 +           *                                        * 68    + 68 A                                             */
    /*   L 67 +    *       *                  ** 67                  *     + 67 L                                             */
    /*     66 +   *                             **                * *      + 66                                               */
    /*   P 65 +  *          *                *    **                  *    + 65 P                                             */
    /*   A 64 +              *                                   *         + 64 A                                             */
    /*   R 63 +                             *       *                  *   + 63 R                                             */
    /*   K 62 +               *                      **                    + 62 K                                             */
    /*     61 +                                                 *       *  + 61                                               */
    /*   T 60 +                *           *           **                  + 60 T                                             */
    /*   E 59 +                 **                       **    *           + 59 E                                             */
    /*   M 58 +                   *                                        + 58 M                                             */
    /*   P 57 +                    *      *                *  *            + 57 P                                             */
    /*   S 56 +                     *                       ** 56          + 56 S                                             */
    /*     55 +                      *   *                                 + 55                                               */
    /*     54 +                       * *                                  + 54                                               */
    /*     53 +                        * 53                                + 53                                               */
    /*     52 + closest weather station                                    + 52                                               */
    /*     51 + https://api.weather.gov/stations/KNY                       + 51                                               */
    /*     50 +                                                            + 50                                               */
    /*        ---++++++++++++++++++++++++++++++++++++++++++++++++++++++++---                                                  */
    /*           000000000000000000000000000000000000000000000000000000001                                                    */
    /*           777777777777888888888888888888888888999999999999999999990                                                    */
    /*           TTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTTT                                                    */
    /*           111111112222000000000011111111112222000000001111111122220                                                    */
    /*           234567890123012345678901234567890123013456781234568901230                                                    */
    /*                                                                                                                        */
    /*        10/07/2024 NOON TO 10/09/2024 MIDNIGHT BY HOURLY TEMPERATURES                                                   */
    /*                                                                                                                        */
    /**************************************************************************************************************************/


    /*                   _
    (_)_ __  _ __  _   _| |_
    | | `_ \| `_ \| | | | __|
    | | | | | |_) | |_| | |_
    |_|_| |_| .__/ \__,_|\__|
            |_|
    */

    %let latitude = "40.71"   ;
    %let longitude = "-74.00" ;

    %let start = "2024-10-07T12:00:00Z";
    %let end   = "2024-10-09T23:59:59Z";

    /*                                    ___                 _               _
     _ __  _ __ ___   ___ ___  ___ ___   ( _ )     ___  _   _| |_ _ __  _   _| |_
    | `_ \| `__/ _ \ / __/ _ \/ __/ __|  / _ \/\  / _ \| | | | __| `_ \| | | | __|
    | |_) | | | (_) | (_|  __/\__ \__ \ | (_>  < | (_) | |_| | |_| |_) | |_| | |_
    | .__/|_|  \___/ \___\___||___/___/  \___/\/  \___/ \__,_|\__| .__/ \__,_|\__|
    |_|                                                          |_|
    */

    options ls=255;

    libname sd1 "d:/sd1";

    proc datasets lib=sd1 nodetails nolist;
     delete rwant;
    run;quit;

    %utl_rbeginx;
    parmcards4;
    library(data.table)
    library(httr2)
    library(sqldf)
    library(purrr)
    library(dplyr)
    library(tidyr)
    library(sf)
    library(haven)
    source("c:/oto/fn_tosas9x.R")
    have<-read_sas("d:/sd1/have.sas7bdat")
    #> Linking to GEOS 3.12.1, GDAL 3.8.4, PROJ 9.3.1; sf_use_s2() is TRUE

    # Define the base URL for the NWS API
    base_url <- "https://api.weather.gov"

    # Define the latitude and longitude for the location
    #latitude <- "40.71"
    #longitude <- "-74.00"

    latitude <-  &latitude
    longitude <- &longitude

    # get stations for a grid cell, parse GeoJSON response with sf
    location_sf <-
      request(base_url) |>
      req_url_path("points", paste(latitude, longitude, sep = ",")) |>
      req_perform() |>
      resp_body_string() |>
      read_sf()
    glimpse(location_sf)
    #> Rows: 1
    #> Columns: 19
    #> $ id                  <chr> "https://api.weather.gov/points/40.71,-74"
    #> $ `@id`               <chr> "https://api.weather.gov/points/40.71,-74"
    #> $ `@type`             <chr> "wx:Point"
    #> $ cwa                 <chr> "OKX"
    #> $ forecastOffice      <chr> "https://api.weather.gov/offices/OKX"
    #> $ gridId              <chr> "OKX"
    #> $ gridX               <int> 33
    #> $ gridY               <int> 35
    #> $ forecast            <chr> "https://api.weather.gov/gridpoints/OKX/33,35/fore…
    #> $ forecastHourly      <chr> "https://api.weather.gov/gridpoints/OKX/33,35/fore…
    #> $ forecastGridData    <chr> "https://api.weather.gov/gridpoints/OKX/33,35"
    #> $ observationStations <chr> "https://api.weather.gov/gridpoints/OKX/33,35/stat…
    #> $ relativeLocation    <chr> "{ \"type\": \"Feature\", \"geometry\": { \"type\"…
    #> $ forecastZone        <chr> "https://api.weather.gov/zones/forecast/NYZ072"
    #> $ county              <chr> "https://api.weather.gov/zones/county/NYC061"
    #> $ fireWeatherZone     <chr> "https://api.weather.gov/zones/fire/NYZ212"
    #> $ timeZone            <chr> "America/New_York"
    #> $ radarStation        <chr> "KDIX"
    #> $ geometry            <POINT [°]> POINT (-74 40.71)

    # get a list of stations, pick one closest to location_sf / input location
    closest_obs_station_sf <-
      location_sf$observationStations |>
      request() |>
      req_perform() |>
      resp_body_string() |>
      read_sf() |>
      slice(st_nearest_feature(location_sf, geometry))
    glimpse(closest_obs_station_sf)
    #> Rows: 1
    #> Columns: 11
    #> $ id                <chr> "https://api.weather.gov/stations/KNYC"
    #> $ `@id`             <chr> "https://api.weather.gov/stations/KNYC"
    #> $ `@type`           <chr> "wx:ObservationStation"
    #> $ elevation         <chr> "{ \"unitCode\": \"wmoUnit:m\", \"value\": 46.9392 }"
    #> $ stationIdentifier <chr> "KNYC"
    #> $ name              <chr> "New York City, Central Park"
    #> $ timeZone          <chr> "America/New_York"
    #> $ forecast          <chr> "https://api.weather.gov/zones/forecast/NYZ072"
    #> $ county            <chr> "https://api.weather.gov/zones/county/NYC061"
    #> $ fireWeatherZone   <chr> "https://api.weather.gov/zones/fire/NYZ212"
    #> $ geometry          <POINT [°]> POINT (-73.96667 40.78333)

    # observations from station, pluck-map-hoist to extract relevant bits from GeoJSON response

    want<-request(base_url) |>
      req_url_path("stations", closest_obs_station_sf$stationIdentifier, "observations") |>
      req_url_query(
        start = &start,
        end   = &end
      ) |>
      req_perform() |>
      resp_body_json() |>
      pluck("features") |>
      map("properties") |>
      tibble(props = _) |>
      hoist(props, "timestamp", temp_value = list("temperature", "value")) |>
      select(-props)

    rwant<-sqldf('
     select
        substr(timestamp, 9, 5) as dayHr
       ,32 + 9.*temp_value/5   as airtemp
     from
        want
    ')
    rwant
    fn_tosas9x(
          inp    =rwant
         ,outlib ="d:/sd1/"
         ,outdsn ="rwant"
         )
    ;;;;
    %utl_rendx;

    libname sd1 "d:/sd1";

    proc print data=sd1.rwant;
    run;quit;

    options ls=80 ps=44;
    proc plot data=rwant;
      plot airtemp*dayhr='*'/box vaxis=50 to 80;;
    run;quit;


    /**************************************************************************************************************************/
    /*                                                                                                                        */
    /* R                                                                                                                      */
    /*                                                                                                                        */
    /*  > rwant                                                                                                               */
    /*     dayHr airtemp                                                                                                      */
    /*  1  09T23   60.98                                                                                                      */
    /*  2  09T22   62.96                                                                                                      */
    /*  3  09T21   64.94                                                                                                      */
    /*  4  09T20   66.92                                                                                                      */
    /*  5  09T19   66.02                                                                                                      */
    /*  ...                                                                                                                   */
    /* 53  07T15   71.96                                                                                                      */
    /* 54  07T14   66.92                                                                                                      */
    /* 55  07T13   66.02                                                                                                      */
    /* 56  07T13   66.02                                                                                                      */
    /* 57  07T12   64.94                                                                                                      */
    /*                                                                                                                        */
    /* SAS                                                                                                                    */
    /*                                                                                                                        */
    /* SD1.RWANT total obs=57                                                                                                 */
    /*                                                                                                                        */
    /*  ROWNAMES    DAYHR    AIRTEMP                                                                                          */
    /*                                                                                                                        */
    /*      1       09T23     60.98                                                                                           */
    /*      2       09T22     62.96                                                                                           */
    /*      3       09T21     64.94                                                                                           */
    /*      4       09T20     66.92                                                                                           */
    /*      5       09T19     66.02                                                                                           */
    /*     ...                                                                                                                */
    /*     53       07T15     71.96                                                                                           */
    /*     54       07T14     66.92                                                                                           */
    /*     55       07T13     66.02                                                                                           */
    /*     56       07T13     66.02                                                                                           */
    /*     57       07T12     64.94                                                                                           */
    /*                                                                                                                        */
    /**************************************************************************************************************************/

    /*              _
      ___ _ __   __| |
     / _ \ `_ \ / _` |
    |  __/ | | | (_| |
     \___|_| |_|\__,_|

    */
