# Comparing `tmp/faadelays-0.0.7.tar.gz` & `tmp/faadelays-2023.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ntilley905/Documents/Coding/Git/delays/dist/tmpmwj2tr71/faadelays-0.0.7.tar", last modified: Mon Apr 19 21:38:45 2021, max compression
+gzip compressed data, was "faadelays-2023.8.0.tar", last modified: Mon Jul 31 16:47:20 2023, max compression
```

## Comparing `faadelays-0.0.7.tar` & `faadelays-2023.8.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ntilley905  (1000) ntilley905  (1000)        0 2021-04-19 21:38:45.296646 faadelays-0.0.7/
--rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)     1069 2020-07-28 16:36:03.000000 faadelays-0.0.7/LICENSE
--rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)     2436 2021-04-19 21:38:45.296646 faadelays-0.0.7/PKG-INFO
--rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)     1734 2021-04-19 21:21:28.000000 faadelays-0.0.7/README.md
-drwxrwxr-x   0 ntilley905  (1000) ntilley905  (1000)        0 2021-04-19 21:38:45.296646 faadelays-0.0.7/faadelays/
--rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)     8782 2021-04-19 21:35:07.000000 faadelays-0.0.7/faadelays/__init__.py
-drwxrwxr-x   0 ntilley905  (1000) ntilley905  (1000)        0 2021-04-19 21:38:45.296646 faadelays-0.0.7/faadelays.egg-info/
--rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)     2436 2021-04-19 21:38:45.000000 faadelays-0.0.7/faadelays.egg-info/PKG-INFO
--rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)      212 2021-04-19 21:38:45.000000 faadelays-0.0.7/faadelays.egg-info/SOURCES.txt
--rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)        1 2021-04-19 21:38:45.000000 faadelays-0.0.7/faadelays.egg-info/dependency_links.txt
--rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)        8 2021-04-19 21:38:45.000000 faadelays-0.0.7/faadelays.egg-info/requires.txt
--rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)       10 2021-04-19 21:38:45.000000 faadelays-0.0.7/faadelays.egg-info/top_level.txt
--rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)       38 2021-04-19 21:38:45.296646 faadelays-0.0.7/setup.cfg
--rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)      709 2021-04-19 21:38:17.000000 faadelays-0.0.7/setup.py
+drwxrwxr-x   0 ntilley905  (1000) ntilley905  (1000)        0 2023-07-31 16:47:20.587701 faadelays-2023.8.0/
+-rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)     1069 2020-07-28 16:36:03.000000 faadelays-2023.8.0/LICENSE
+-rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)     3654 2023-07-31 16:47:20.587701 faadelays-2023.8.0/PKG-INFO
+-rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)     1893 2023-07-30 23:44:36.000000 faadelays-2023.8.0/README.md
+drwxrwxr-x   0 ntilley905  (1000) ntilley905  (1000)        0 2023-07-31 16:47:20.587701 faadelays-2023.8.0/faadelays/
+-rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)     9579 2023-07-31 16:10:00.000000 faadelays-2023.8.0/faadelays/__init__.py
+drwxrwxr-x   0 ntilley905  (1000) ntilley905  (1000)        0 2023-07-31 16:47:20.587701 faadelays-2023.8.0/faadelays.egg-info/
+-rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)     3654 2023-07-31 16:47:20.000000 faadelays-2023.8.0/faadelays.egg-info/PKG-INFO
+-rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)      218 2023-07-31 16:47:20.000000 faadelays-2023.8.0/faadelays.egg-info/SOURCES.txt
+-rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)        1 2023-07-31 16:47:20.000000 faadelays-2023.8.0/faadelays.egg-info/dependency_links.txt
+-rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)        8 2023-07-31 16:47:20.000000 faadelays-2023.8.0/faadelays.egg-info/requires.txt
+-rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)       10 2023-07-31 16:47:20.000000 faadelays-2023.8.0/faadelays.egg-info/top_level.txt
+-rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)      659 2023-07-31 16:45:50.000000 faadelays-2023.8.0/pyproject.toml
+-rw-rw-r--   0 ntilley905  (1000) ntilley905  (1000)       38 2023-07-31 16:47:20.587701 faadelays-2023.8.0/setup.cfg
```

### Comparing `faadelays-0.0.7/LICENSE` & `faadelays-2023.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `faadelays-0.0.7/README.md` & `faadelays-2023.8.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # FAA Airport Status
 
-This is a simple Python package used to retrieve data from the FAA's ASWS API. See https://app.swaggerhub.com/apis/FAA/ASWS/1.1.0 for API documentation.
+This is a simple Python package used to retrieve data from the FAA's NAS Status API.
 
 ## Classes
 
 The following classes are available and in some cases dynamically generated when retrieving data:
 
 Class | Information Provided | Methods
 --- | --- | ---
-ArriveDepartDelay | Airport, Status, Minimum delay, Maximum delay, Trend, Reason
-GroundDelay | Airport, Status, Average delay, Reason
-GroundStop | Airport, Status, End Time, Reason
-Closure | Airport, Status, Begin Time, End Time, Reason
-Nationwide | Total count of delays, Array of Ground delays, Count of Ground Delays, Array of Ground Stops, Count of Ground Stops, Array of ArriveDepart Delays, Count of ArriveDepart Delays, Array of Closures, Count of Closures | Update
-Airport | Code (provide when creating, IATA format), Name, City, State, ICAO identifier, IATA identifier, Bool of Supported Airport, Bool of any delays, Count of delays, GroundDelay object, GroundStop object, Depart Delay object (ArriveDepartDelay), Arrive Delay object (ArriveDepartDelay), Closure object | Update
+ArriveDepartDelay | Airport, Status, Minimum delay, Maximum delay, Trend, Reason, Update time
+GroundDelay | Airport, Status, Average delay, Maximum delay, Start time, End time, Reason, Update time, URL to the advisory, Departure scope (if applicable), Included Facilities (if applicable), Included flights (if applicable)
+GroundStop | Airport, Status, End Time, Reason, Update time, URL to advisory, Included facilities (if applicable), Included flights (if applicable), Probabibility of extension
+Closure | Airport, Status, Begin Time, End Time, Update time, NOTAM text
+AirportConfig | Airport, Time the data was created, Arrival runway config, Departure runway config, Arrival rate, Source time stamp
+Airport | Code (provide when creating, IATA format), *Name*, *Longitude*, *Latitude*, Bool of if airport is deicing (see note), Bool of any delays, Count of delays, GroundDelay object, GroundStop object, Depart Delay object (ArriveDepartDelay), Arrive Delay object (ArriveDepartDelay), Closure object, Airport config | Update
 
-## Methods Available
+Items in *italics* are not updated until delay data is present
+
+Note: Information about airport deicing is untested
 
-`get_nationwide_delays(session)` requires an asyncio HTTP session (such as aiohttp.ClientSession) and returns a Nationwide object
+## Methods Available
 
 `get_airport_delays(airport_code, session)` requires the code for the airport to get delays for in IATA format (i.e. ATL for Atlanta) and an asyncio HTTP session (such as aiohttp.ClientSession) and returns an Airport object
 
 ## Support
 [![Buy me a coffee][buymeacoffee-shield]][buymeacoffee]
```

### Comparing `faadelays-0.0.7/faadelays/__init__.py` & `faadelays-2023.8.0/faadelays/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,246 +1,221 @@
 """Fetch latest data from the FAA ASWS API."""
 from aiohttp import ClientSession, ClientResponseError
 
-BASE_URL = "https://soa.smext.faa.gov/asws/api/airport/{}"
+BASE_URL = "https://nasstatus.faa.gov/api/airport-events"
 
-# define custom errors
-class InvalidAirport(Exception):
-    """Raised when the airport returns no data from the API."""
-    pass
 
 class ArriveDepartDelay:
     # Class for Arrival/Departure delays
-    def __init__(self, airport, status=False, minimum=None, maximum=None, trend=None, reason=None):
+    def __init__(self, airport, status=False, minimum=None, maximum=None, average_delay=None, trend=None, reason=None, update_time=None):
         self.airport = airport
         self.status = status
         self.minimum = minimum
         self.maximum = maximum
+        self.average_delay = average_delay
         self.trend = trend
         self.reason = reason
+        self.update_time = update_time
 
 class GroundDelay:
     # Class for Ground Delays
-    def __init__(self, airport, status=False, average=None, reason=None):
+    def __init__(self, airport, status=False, average=None, max_delay=None, start_time=None, end_time=None, reason=None, update_time=None, advisory_url=None, departure_scope=None, included_facilities=None, included_flights=None):
         self.airport = airport
         self.status = status
         self.average = average
+        self.max_delay = max_delay
+        self.start_time = start_time
+        self.end_time = end_time
         self.reason = reason
+        self.update_time = update_time
+        self.advisory_url = advisory_url
+        self.departure_scope = departure_scope
+        self.included_facilities = included_facilities
+        self.included_flights = included_flights
+
 
 class GroundStop:
     # Class for Ground Stops
-    def __init__(self, airport, status=False, endtime=None, reason=None):
+    def __init__(self, airport, status=False, endtime=None, reason=None, update_time=None, advisory_url=None, included_facilities=None, included_flights=None, probability_of_extension=None):
         self.airport = airport
         self.status = status
         self.endtime = endtime
         self.reason = reason
+        self.update_time = update_time
+        self.advisory_url = advisory_url
+        self.included_facilities = included_facilities
+        self.included_flights = included_flights
+        self.probabibility_of_extension = probability_of_extension
 
 class Closure:
     # Class for closures
-    def __init__(self, airport, status=False, begin=None, end=None, reason=None):
+    def __init__(self, airport, status=False, start=None, end=None, reason=None, update_time=None, notam=None):
         self.airport = airport
         self.status = status
-        self.begin = begin
+        self.start = start
         self.end = end
-        self.reason = reason
-
-
-class Nationwide:
-    # Class for storing data from a nationwide API call
-    def __init__(self, session: ClientSession):
-        self.url = BASE_URL.format("delays")
-        self.count = 0
-        self.ground_delays = []
-        self.ground_delay_count = 0
-        self.ground_stops = []
-        self.ground_stop_count = 0
-        self.arrive_depart_delays = []
-        self.arrive_depart_count = 0
-        self.closures = []
-        self.closure_count = 0
-        self.session = session
+        self.update_time = update_time
+        self.notam = notam
 
-    async def update(self):
-        resp = await self.session.get(self.url)
-        if resp.status == 200:
-            data = await resp.json()
-        else:
-            raise ClientResponseError(
-                    resp.request_info,
-                    resp.history
-                    )
-        self.count = data['status']['count']
-
-        for gd in data['GroundDelays']['groundDelay']:
-            # Define a ground delay object and append that to the list of nationwide ground delays
-            gdelay = GroundDelay(gd['airport'],
-            True,
-            gd['avgTime'],
-            gd['reason'])
-
-            self.ground_delays.append(gdelay)
-
-        self.ground_delay_count = data['GroundDelays']['count']
-        for gs in data['GroundStops']['groundStop']:
-            # Define a ground stop object and append that to the list of nationwide ground stops
-            stop = GroundStop(
-                gs['airport'],
-                True,
-                gs['endTime'],
-                gs['reason']
-            )
-
-            self.ground_stops.append(stop)
-
-        self.ground_stop_count = data['GroundStops']['count']
-        for ad in data['ArriveDepartDelays']['arriveDepart']:
-            # Define an Arrival/Departure object and append that to the list of nationwide arrival/departure delays
-            ardp = ArriveDepartDelay(
-                ad['airport'],
-                True,
-                ad['minTime'],
-                ad['maxTime'],
-                None, # The API does not provide a trend for Arrival/Departure delays from the nationwide call so none will be passed through.
-                ad['reason']
-            )
-
-            self.arrive_depart_delays.append(ardp)
-
-        self.arrive_depart_count = data['ArriveDepartDelays']['count']
-        for cl in data['Closures']['closure']:
-            # Define a closure object and append that to the list of nationwide closures
-            close = Closure(
-                cl['airport'],
-                True,
-                None, # The API does not provide a beginning time for a closure from the nationwide call so none will be passed through.
-                cl['reopen'],
-                cl['reason']
-            )
-
-            self.closures.append(close)
+class AirportConfig:
+    # Class for storing airport config data
+    def __init__(self, airport, created_time=None, arrival_runway_config=None, departure_runway_config=None, arrival_rate=None, source_time_stamp=None):
+        self.airport = airport
+        self.created_time = created_time
+        self.arrival_runway_config = arrival_runway_config
+        self.departure_runway_config = departure_runway_config
+        self.arrival_rate = arrival_rate
+        self.source_time_stamp = source_time_stamp
 
-        self.closure_count = data['Closures']['count']
 
 class Airport:
     # Class for storing data for an individual airport
     def __init__(self, code, session: ClientSession):
         self.code = code
         self.name = None
-        self.city = None
-        self.state = None
-        self.icao = None
-        self.iata = None
+        self.latitude = None
+        self.longitude = None
+        self.is_deicing = False
         self.supported_airport = None
-        self.delay = None
-        self.delay_count = None
+        self.delay = False
+        self.delay_count = 0
         self.ground_delay = GroundDelay(self.code)
         self.ground_stop = GroundStop(self.code)
         self.depart_delay = ArriveDepartDelay(self.code)
         self.arrive_delay = ArriveDepartDelay(self.code)
         self.closure = Closure(self.code)
-        self.url = BASE_URL.format("status/" + self.code)
+        self.config = None
         self.session = session
 
     async def update(self):
-        resp = await self.session.get(self.url)
+        resp = await self.session.get(BASE_URL)
         if resp.status == 200:
             data = await resp.json()
         else:
             raise ClientResponseError(
                 resp.request_info,
                 resp.history,
                 )
-        try:
-            self.name = data['Name']
-        # check for key error here because if a name is not returned no other data will be either as the API does not recognize the airport
-        except KeyError:
-            raise InvalidAirport(self.code + " is not a valid airport")
-        self.city = data['City']
-        self.state = data['State']
-        self.icao = data['ICAO']
-        self.iata = data['IATA']
-        self.supported_airport = data['SupportedAirport']
-        self.delay = data['Delay']
-        self.delay_count = data['DelayCount']
-        self.weather = data['Weather']['Weather'][0]['Temp'][0]
-        self.visibility = data['Weather']['Visibility'][0]
-        self.temp = data['Weather']['Temp'][0]
-        self.wind = data['Weather']['Wind'][0]
-
-        # If no delays, set all types to false
-        if self.delay == False:
-            ar = de = gd = gs = cl = False
-        else:
-            # Look for each type of delay in the API response
-            # The API does not order the delays and does not return each in a consistent type so each has to use a different method
-            ar = next((i for i, d in enumerate(data['Status']) if d.get('Type') == "Arrival"), False)
-            de = next((i for i, d in enumerate(data['Status']) if d.get('Type') == "Departure"), False)
-            gd = next((i for i, d in enumerate(data['Status']) if d.get('Type') == "Ground Delay"), False)
-            gs = next((i for i, d in enumerate(data['Status']) if "EndTime" in d), False)
-            cl = next((i for i, d in enumerate(data['Status']) if "ClosureEnd" in d), False)
-
-        if ar is False:
-            self.arrive_delay = ArriveDepartDelay(self.code)
-        else:
-            self.arrive_delay = ArriveDepartDelay(
-                self.code,
-                True,
-                data['Status'][ar]["MinDelay"],
-                data['Status'][ar]["MaxDelay"],
-                data['Status'][ar]["Trend"],
-                data['Status'][ar]["Reason"]
-            )
 
-        if de is False:
-            self.depart_delay = ArriveDepartDelay(self.code)
-        else:
-            self.depart_delay = ArriveDepartDelay(
-                self.code,
-                True,
-                data['Status'][de]["MinDelay"],
-                data['Status'][de]["MaxDelay"],
-                data['Status'][de]["Trend"],
-                data['Status'][de]["Reason"]
-            )
+        # iterate through returned data for correct airport
+        for airport in data:
+            if airport['airportId'] == self.code:
+
+                self.name = airport['airportLongName']
+                self.latitude = airport['latitude']
+                self.longitude = airport['longitude']
+
+                if airport['deicing']:
+                    self.is_deicing = True
+                
+                # check for each type of delay
+                if airport['groundStop']:
+                    self.ground_stop = GroundStop(
+                        airport=self.code,
+                        status=True,
+                        endtime=airport['groundStop']['endTime'],
+                        reason=airport['groundStop']['impactingCondition'],
+                        update_time=airport['groundStop']['updatedAt'],
+                        advisory_url=airport['groundStop']['advisoryUrl'],
+                        included_facilities=airport['groundStop']['includedFacilities'],
+                        included_flights=airport['groundStop']['includedFlights'],
+                        probability_of_extension=airport['groundStop']['probabilityOfExtension'],
+                    )
+                    self.delay_count += 1
+                else:
+                    self.GroundStop = GroundStop(self.code)
+                
+                if airport['arrivalDelay']:
+                    self.arrive_delay = ArriveDepartDelay(
+                        airport=self.code,
+                        status=True,
+                        minimum=airport['arrivalDelay']['arrivalDeparture']['min'],
+                        maximum=airport['arrivalDelay']['arrivalDeparture']['max'],
+                        average_delay=airport['arrivalDelay']['averageDelay'],
+                        trend=airport['arrivalDelay']['arrivalDeparture']['trend'],
+                        reason=airport['arrivalDelay']['reason'],
+                        update_time=airport['arrivalDelay']['updateTime'],
+                    )
+                    self.delay_count += 1
+                
+                else:
+                    self.arrive_delay = ArriveDepartDelay(self.code)
+                
+                if airport['departureDelay']:
+                    self.depart_delay = ArriveDepartDelay(
+                        airport=self.code,
+                        status=True,
+                        minimum=airport['departureDelay']['arrivalDeparture']['min'],
+                        maximum=airport['departureDelay']['arrivalDeparture']['max'],
+                        average_delay=airport['departureDelay']['averageDelay'],
+                        trend=airport['departureDelay']['arrivalDeparture']['trend'],
+                        reason=airport['departureDelay']['reason'],
+                        update_time=airport['departureDelay']['updateTime'],
+                    )
+                    self.delay_count += 1
+                
+                else:
+                    self.depart_delay = ArriveDepartDelay(self.code)
+
+                if airport['groundDelay']:
+                    self.ground_delay = GroundDelay(
+                        airport=self.code,
+                        status=True,
+                        average=airport['groundDelay']['avgDelay'],
+                        max_delay=airport['groundDelay']['maxDelay'],
+                        reason=airport['groundDelay']['impactingCondition'],
+                        update_time=airport['groundDelay']['updatedAt'],
+                        advisory_url=airport['groundDelay']['advisoryUrl'],
+                        departure_scope=airport['groundDelay']['departureScope'],
+                        included_facilities=airport['groundDelay']['includedFacilities'],
+                        included_flights=airport['groundDelay']['includedFlights'],
+                    )
+                    self.delay_count += 1
+                
+                else:
+                    self.ground_delay = GroundDelay(self.code)
+
+                if airport['airportClosure']:
+                    self.closure = Closure(
+                        airport=self.code,
+                        status=True,
+                        start=airport['airportClosure']['startTime'],
+                        end=airport['airportClosure']['endTime'],
+                        update_time=airport['airportClosure']['updatedAt'],
+                        notam=airport['airportClosure']['simpleText'],
+                    )
 
-        if gd is False:
-            self.ground_delay = GroundDelay(self.code)
-        else:
-            self.ground_delay = GroundDelay(
-                self.code,
-                True,
-                data['Status'][gd]['AvgDelay'],
-                data['Status'][gd]['Reason']
-            )
+                elif airport['freeForm']:
+                    # API doesn't always put closures in the actual closure field so check freeform
+                    if "CLSD" in airport['freeForm']['simpleText']:
+                        self.closure = Closure(
+                            airport=self.code,
+                            status=True,
+                            start=airport['freeForm']['startTime'],
+                            end=airport['freeForm']['endTime'],
+                            update_time=airport['freeForm']['updatedAt'],
+                            notam=airport['freeForm']['simpleText'],
+                        )
+
+                else:
+                    self.closure = Closure(self.code)
 
-        if gs is False:
-            self.ground_stop = GroundStop(self.code)
-        else:
-            self.ground_stop = GroundStop(
-                self.code,
-                True,
-                data['Status'][gs]['EndTime'],
-                data['Status'][gs]['Reason']
-            )
+                if self.delay_count > 0:
+                    self.delay = True                
 
-        if cl is False:
-            self.closure = Closure(self.code)
-        else:
-            self.closure = Closure(
-                self.code,
-                True,
-                data['Status'][cl]['ClosureBegin'],
-                data['Status'][cl]['ClosureEnd'],
-                data['Status'][cl]['Reason']
-            )
+                return self
 
-async def get_nationwide_delays(session: ClientSession):
-    results = Nationwide(session)
-    await results.update()
+            
+        # if airport is not in data then no programs are active
+        self.arrive_delay = ArriveDepartDelay(self.code)
+        self.depart_delay = ArriveDepartDelay(self.code)
+        self.ground_stop = GroundStop(self.code)
+        self.ground_delay = GroundDelay(self.code)
+        self.closure = Closure(self.code)
 
-    return results
+                
 
 async def get_airport_delays(code, session: ClientSession):
     results = Airport(code, session)
     await results.update()
 
     return results
```

