# energy_data_analysis
Basic notebooks for processing Building Management System and energy monitoring data
A building energy management system (BEMS) controls a buildings environment including heating and ventilation. Different sensors are used to take readings including temperature and pressure which feed back into BEMS. Energy use, including electricity, gas, oil and heat, is also monitored which allows an energy manager to spot high areas of use for example.

An example of a half hourly energy log 'comma seperated variable' (CSV) file is attached from a Schneider Continuum BEMS system. The first column shows the datetime stamp of every read. The other columns represent a meter for a different piece of kit, distribution boards as examples and kWh readings taken every half hour.

Here I am trying to calculate consumption amounts in kWh (kilo watt hours) for the meters. For example, to find a daily total, I could take the final read on that day and subtract the first read taken that day. This would give the total kWh consumption over that period. As there are approx. 189 meters across the build, over many weeks, I wanted to write something in Python using the Pandas library which would speed up this process.

