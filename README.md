# WeatherStation-EmbeddedSystems
 Weather Station in a PIC microcontroller
 
 ## System Architecture
 
 ![image](https://user-images.githubusercontent.com/60743836/181848981-acbd9021-a628-4deb-9f8a-bd9e90914917.png)
 
 ## Command description
 
* rc - read clock

* sc h m s - set clock

* rtl - read temperature and luminosity

* rp - read parameters (PMON, TALA)

* mmp p - modify monitoring period (seconds - 0 deactivate)

* mta t - modify time alarm (seconds)

* ra - read alarms (temperature, luminosity, active/inactive-1/0)

* dtl t l - define alarm temperature and luminosity

* aa a - activate/deactivate alarms (1/0)

* ir - information about registers (NREG, nr, iread, iwrite)

* trc n - transfer n registers from current iread position

* tri n i - transfer n registers from index i (0 - oldest)

* irl - information about local registers (NRBUF, nr, iread, iwrite)

* lr n i - list n registers (local memory) from index i (0 - oldest)

* dr - delete registers (local memory)

* cpt - check period of transference

* mpt p - modify period of transference (minutes - 0 deactivate)

* cttl - check threshold temperature and luminosity for processing

* dttl t l - define threshold temperature and luminosity for processing

* pr [h1 m1 s1 [h2 m2 s2]] - process registers (max, min, mean) between instants t1 and t2 (h,m,s)


* RCLK [h m s] - read clock

* SCLK h m s - set clock

* RTL [T L] - read temperature and luminosity

* RPAR [pars] - read parameters (PMON, TALA)

* MMP p - modify monitoring period

* MTA t - modify time alarm

* RALA [T L a] - read alarms (temperature, luminosity, active/inactive)

* DATL T L - define alarm temperature and luminosity

* AALA a - activate/deactivate alarms

* IREG [N nr ri wi] - information about registers (NREG, nr, iread, iwrite)

* TRGC n [regs] - transfer n registers from current iread position

* TRGI n i [regs] - transfer n registers from index i

* NMFL [N nr ri wi] - notification memory (half) full

