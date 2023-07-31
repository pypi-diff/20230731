# Comparing `tmp/ipfabric_diagrams-6.3.0b2.tar.gz` & `tmp/ipfabric_diagrams-6.3.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric_diagrams-6.3.0b2.tar", max compression
+gzip compressed data, was "ipfabric_diagrams-6.3.1b0.tar", max compression
```

## Comparing `ipfabric_diagrams-6.3.0b2.tar` & `ipfabric_diagrams-6.3.1b0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1829 2023-07-27 12:53:56.681338 ipfabric_diagrams-6.3.0b2/ipfabric/__init__.py
--rw-r--r--   0        0        0     1906 2023-07-27 17:53:40.204546 ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/__init__.py
--rw-r--r--   0        0        0     7320 2023-07-27 18:09:49.878919 ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/graphs.py
--rw-r--r--   0        0        0     3625 2023-05-25 13:21:36.148253 ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/icmp.py
--rw-r--r--   0        0        0      580 2023-05-25 13:21:36.148253 ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/input_models/__init__.py
--rw-r--r--   0        0        0     3755 2023-05-25 13:21:36.148253 ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/input_models/constants.py
--rw-r--r--   0        0        0        0 2023-05-25 13:21:36.149259 ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/input_models/factory_defaults/__init__.py
--rw-r--r--   0        0        0     5792 2023-07-27 14:55:19.860010 ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json
--rw-r--r--   0        0        0     2173 2023-07-27 14:55:44.537121 ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json
--rw-r--r--   0        0        0    11200 2023-07-27 18:16:43.733444 ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/input_models/graph_parameters.py
--rw-r--r--   0        0        0    10995 2023-07-27 18:16:43.740304 ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/input_models/graph_settings.py
--rw-r--r--   0        0        0       68 2023-07-27 17:57:52.713767 ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/output_models/__init__.py
--rw-r--r--   0        0        0     5127 2023-07-27 18:09:56.612433 ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/output_models/graph_result.py
--rw-r--r--   0        0        0     1957 2023-07-27 18:09:56.575671 ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/output_models/protocols.py
--rw-r--r--   0        0        0     3350 2023-07-27 13:11:08.625007 ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/output_models/trace.py
--rw-r--r--   0        0        0     1152 2023-05-25 13:21:36.160649 ipfabric_diagrams-6.3.0b2/ipfabric_diagrams/__init__.py
--rw-r--r--   0        0        0      176 2023-05-25 13:21:36.166244 ipfabric_diagrams-6.3.0b2/ipfabric_diagrams/graphs.py
--rw-r--r--   0        0        0     2910 2023-05-25 13:21:36.173769 ipfabric_diagrams-6.3.0b2/ipfabric_diagrams/icmp.py
--rw-r--r--   0        0        0     1087 2023-05-25 13:21:36.111751 ipfabric_diagrams-6.3.0b2/LICENSE
--rw-r--r--   0        0        0     1808 2023-07-27 18:44:55.905948 ipfabric_diagrams-6.3.0b2/pyproject.toml
--rw-r--r--   0        0        0     2820 2023-07-17 15:30:22.891723 ipfabric_diagrams-6.3.0b2/README.md
--rw-r--r--   0        0        0     3913 1970-01-01 00:00:00.000000 ipfabric_diagrams-6.3.0b2/setup.py
--rw-r--r--   0        0        0     3945 1970-01-01 00:00:00.000000 ipfabric_diagrams-6.3.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1498 2023-07-17 15:33:42.174440 ipfabric_diagrams-6.3.1b0/ipfabric/__init__.py
+-rw-r--r--   0        0        0     1809 2023-07-17 15:36:43.381090 ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/__init__.py
+-rw-r--r--   0        0        0     7488 2023-05-25 13:21:36.146926 ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/graphs.py
+-rw-r--r--   0        0        0     3625 2023-05-25 13:21:36.148253 ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/icmp.py
+-rw-r--r--   0        0        0      580 2023-05-25 13:21:36.148253 ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/input_models/__init__.py
+-rw-r--r--   0        0        0     3755 2023-05-25 13:21:36.148253 ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/input_models/constants.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:21:36.149259 ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/input_models/factory_defaults/__init__.py
+-rw-r--r--   0        0        0     7009 2023-05-25 13:21:36.149259 ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json
+-rw-r--r--   0        0        0     2277 2023-05-25 13:21:36.150259 ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json
+-rw-r--r--   0        0        0    10507 2023-05-25 13:21:36.150259 ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/input_models/graph_parameters.py
+-rw-r--r--   0        0        0    10534 2023-05-25 13:21:36.150259 ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/input_models/graph_settings.py
+-rw-r--r--   0        0        0       68 2023-05-25 13:21:36.151765 ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/output_models/__init__.py
+-rw-r--r--   0        0        0     2608 2023-05-25 13:21:36.151765 ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/output_models/graph_result.py
+-rw-r--r--   0        0        0     1412 2023-05-25 13:21:36.152771 ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/output_models/protocols.py
+-rw-r--r--   0        0        0     3198 2023-05-25 13:35:46.575244 ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/output_models/trace.py
+-rw-r--r--   0        0        0     1152 2023-05-25 13:21:36.160649 ipfabric_diagrams-6.3.1b0/ipfabric_diagrams/__init__.py
+-rw-r--r--   0        0        0      176 2023-05-25 13:21:36.166244 ipfabric_diagrams-6.3.1b0/ipfabric_diagrams/graphs.py
+-rw-r--r--   0        0        0     2910 2023-05-25 13:21:36.173769 ipfabric_diagrams-6.3.1b0/ipfabric_diagrams/icmp.py
+-rw-r--r--   0        0        0     1087 2023-05-25 13:21:36.111751 ipfabric_diagrams-6.3.1b0/LICENSE
+-rw-r--r--   0        0        0     1679 2023-07-17 15:38:12.296734 ipfabric_diagrams-6.3.1b0/pyproject.toml
+-rw-r--r--   0        0        0     2820 2023-07-17 15:30:22.891723 ipfabric_diagrams-6.3.1b0/README.md
+-rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 ipfabric_diagrams-6.3.1b0/setup.py
+-rw-r--r--   0        0        0     3859 1970-01-01 00:00:00.000000 ipfabric_diagrams-6.3.1b0/PKG-INFO
```

### Comparing `ipfabric_diagrams-6.3.0b2/ipfabric/__init__.py` & `ipfabric_diagrams-6.3.1b0/ipfabric/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,26 +21,17 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 # This file must be copied from ipfabric repo to ipfabric_diagrams repo at /ipfabric/__init__.py until v7.0.0
 
 __path__ = __import__("pkgutil").extend_path(__path__, __name__)  # TODO Remove in v7.0.0
 
-# noinspection PyUnresolvedReferences
-from .client import IPFClient
-
-try:
-    import importlib.metadata as importlib_metadata
-except ModuleNotFoundError:
-    import importlib_metadata
-
 import logging
-from platform import python_version_tuple
+from importlib import metadata
 
-logger = logging.getLogger("ipfabric")
+from .client import IPFClient
 
-if tuple(map(int, (python_version_tuple()[0:2]))) < (3, 8):
-    logger.warning("Python 3.7 will be deprecated in ipfabric v7.0.0")  # TODO v7.0.0
+logger = logging.getLogger("ipfabric")
 
-__version__ = importlib_metadata.version(__name__)
+__version__ = metadata.version(__name__)
 
 __all__ = ["IPFClient"]
```

### Comparing `ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/__init__.py` & `ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,18 +35,15 @@
     NetworkSettings,
     PathLookupSettings,
     Overlay,
     VALID_NET_PROTOCOLS,
     VALID_PATH_PROTOCOLS,
 )
 
-try:
-    import importlib.metadata as importlib_metadata
-except ModuleNotFoundError:
-    import importlib_metadata
+from importlib import metadata
 
 __all__ = [
     "IPFDiagram",
     "Unicast",
     "Multicast",
     "Host2GW",
     "Network",
@@ -58,8 +55,8 @@
     "PathLookupSettings",
     "EntryPoint",
     "VALID_NET_PROTOCOLS",
     "VALID_PATH_PROTOCOLS",
     "Layout",
 ]
 
-__version__ = importlib_metadata.version("ipfabric_diagrams")
+__version__ = metadata.version("ipfabric_diagrams")
```

### Comparing `ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/graphs.py` & `ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/graphs.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         snapshot_id: str = None,
         overlay: Overlay = None,
         image: str = None,
         graph_settings: Union[NetworkSettings, PathLookupSettings, GraphSettings] = None,
         attr_filters: Optional[Dict[str, List[str]]] = None,
     ):
         """
-        Submits a query, does no formatting on the parameters.  Use for copy/pasting from the webpage.
+        Submits a query, does no formating on the parameters.  Use for copy/pasting from the webpage.
         :param parameters: dict: Dictionary to submit in POST.
         :return: list: List of Dictionary objects.
         """
         url = GRAPHS_URL + image if image else GRAPHS_URL
         payload = dict(parameters=parameters, snapshot=self._check_graph_cache(snapshot_id))
         if overlay:
             if overlay.type == "compare":
@@ -127,18 +127,17 @@
         else:
             return self._diagram_pathlookup(json_data, edge_setting_dict)
 
     @staticmethod
     def _diagram_network(json_data: dict, edge_setting_dict: dict, pathlookup: bool = False) -> GraphResult:
         edges, nodes = dict(), dict()
         for node_id, node in json_data["graphResult"]["graphData"]["nodes"].items():
-            nodes[node_id] = Node.model_validate(node)
-
+            nodes[node_id] = Node(**node)
         for edge_id, edge_json in json_data["graphResult"]["graphData"]["edges"].items():
-            edge = PathLookupEdge.model_validate(edge_json) if pathlookup else NetworkEdge.model_validate(edge_json)
+            edge = PathLookupEdge(**edge_json) if pathlookup else NetworkEdge(**edge_json)
             edge.protocol = (
                 edge_setting_dict[edge.edgeSettingsId].name if edge.edgeSettingsId in edge_setting_dict else None
             )
             if edge.source:
                 edge.source = nodes[edge.source]
             if edge.target:
                 edge.target = nodes[edge.target]
@@ -150,16 +149,20 @@
         graph_result = self._diagram_network(json_data, edge_setting_dict, pathlookup=True)
 
         for edge_id, edge in graph_result.edges.items():
             for prev_id in edge.prevEdgeIds:
                 edge.prevEdge.append(graph_result.edges[prev_id])
             for next_id in edge.nextEdgeIds:
                 edge.nextEdge.append(graph_result.edges[next_id] if next_id in graph_result.edges else next_id)
-        graph_result.pathlookup = PathLookup.model_validate(json_data["pathlookup"])
-
+        # for a in json_data["pathlookup"]['decisions'].values():
+        #     for b in a['traces']:
+        #         for c in b['trace']:
+        #             for d in c['events']:
+        #                 print(d)
+        graph_result.pathlookup = PathLookup(**json_data["pathlookup"])
         return graph_result
 
     @staticmethod
     def _diagram_edge_settings(graph_settings: dict) -> dict:
         net_settings = GraphSettings(**graph_settings)
         edge_setting_dict = dict()
         for edge in net_settings.edges:
```

### Comparing `ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/icmp.py` & `ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/icmp.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/input_models/__init__.py` & `ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/input_models/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/input_models/constants.py` & `ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/input_models/constants.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json` & `ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888888888888888%*

 * *Differences: {'delete': '[8]'}*

```diff
@@ -146,28 +146,9 @@
                 2,
                 4,
                 8
             ]
         },
         "type": "pathLookupEdge",
         "visible": true
-    },
-    {
-        "grouped": false,
-        "labels": [
-            "intName",
-            "protocol"
-        ],
-        "name": "fp",
-        "style": {
-            "color": "#ff9800",
-            "pattern": "solid",
-            "thicknessThresholds": [
-                2,
-                4,
-                8
-            ]
-        },
-        "type": "pathLookupEdge",
-        "visible": true
     }
 ]
```

### Comparing `ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/input_models/graph_parameters.py` & `ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/input_models/graph_parameters.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,56 @@
-import os
 import re
 from copy import deepcopy
-from ipaddress import IPv4Interface, IPv4Address, IPv4Network, AddressValueError
+from ipaddress import IPv4Interface, IPv4Address
 from typing import Optional, Union, List
 
-try:
-    from typing import Annotated  # py38 required Annotated
-except ImportError:
-    from typing_extensions import Annotated
-
-from pydantic import field_validator, BaseModel, Field
-from pydantic.functional_validators import BeforeValidator
+from pydantic import BaseModel, validator, Field
 
 from .constants import VALID_LAYOUTS
 
-PYDANTIC_EXTRAS = os.getenv("IPFABRIC_PYDANTIC_EXTRAS", "allow")
 PORT_REGEX = re.compile(r"^\d*$|^\d*-\d*$")
 ALL_NETWORK = "$main"
 
 
-def check_ip_network(v: Union[str, IPv4Address, IPv4Network, IPv4Interface]):
-    if isinstance(v, IPv4Address):
-        return str(v)
-    if isinstance(v, (IPv4Network, IPv4Interface)):
-        return v.with_prefixlen
-    try:
-        return IPv4Interface(v).with_prefixlen
-    except AddressValueError:
-        raise ValueError(f'IP "{v}" not a valid IP Address')
-
-
-IPv4 = Annotated[Union[str, IPv4Address, IPv4Network, IPv4Interface], BeforeValidator(check_ip_network)]
-
-
-class Instance(BaseModel, extra=PYDANTIC_EXTRAS):
+class Instance(BaseModel):
     rootId: str
     vlanId: int
     visible: bool = True
     grouped: bool = True
 
 
-class STPInstances(BaseModel, extra=PYDANTIC_EXTRAS):
+class STPInstances(BaseModel):
     isolate: bool = False
     instances: List[Instance]
 
 
-class Technologies(BaseModel, extra=PYDANTIC_EXTRAS):
+class Technologies(BaseModel):
     expandDeviceGroups: Optional[List[str]] = Field(default_factory=list)
-    stpInstances: Optional[STPInstances] = None
+    stpInstances: Optional[STPInstances]
 
     def technologies_parameters(self) -> dict:
         params = dict(expandDeviceGroups=self.expandDeviceGroups)
         if self.stpInstances:
             params["stpInstances"] = dict(isolate=self.stpInstances.isolate, instances=list())
             for i in self.stpInstances.instances:
                 params["stpInstances"]["instances"].append(vars(i))
         return params
 
 
-class ICMP(BaseModel, extra=PYDANTIC_EXTRAS):
+class ICMP(BaseModel):
     type: int
     code: int
 
 
-class OtherOptions(BaseModel, extra=PYDANTIC_EXTRAS):
+class OtherOptions(BaseModel):
     applications: Optional[str] = ".*"
     tracked: Optional[bool] = False
 
 
-class EntryPoint(BaseModel, extra=PYDANTIC_EXTRAS):
+class EntryPoint(BaseModel):
     sn: str = Field(title="Serial Number", description="IP Fabric Unique Device Serial Number API column sn")
     iface: str = Field(
         title="Interface", description="Interface to use as entry point. This is the intName not nameOriginal."
     )
     hostname: str = Field(title="Hostname", description="Hostname of the Device")
 
 
@@ -89,15 +67,15 @@
     def algorithm_parameters(self) -> dict:
         if self.entryPoints:
             return dict(type=self.type, entryPoints=[vars(e) for e in self.entryPoints])
         else:
             return dict(type=self.type, vrf=self.vrf) if self.vrf else dict(type=self.type)
 
 
-class PathLookup(BaseModel, extra=PYDANTIC_EXTRAS):
+class PathLookup(BaseModel):
     protocol: Optional[str] = Field("tcp", title="Protocol", description="Valid protocols are tcp, udp, or icmp.")
     srcPorts: Optional[Union[str, int]] = Field(
         "1024-65535",
         title="Source Ports",
         description="Source ports if protocol is tcp or udp. "
         "Can be comma separated, a range using -, or any combination.",
     )
@@ -126,38 +104,35 @@
     securedPath: Optional[bool] = True
     enableRegions: Optional[bool] = False
     srcRegions: Optional[str] = ".*"
     dstRegions: Optional[str] = ".*"
     otherOptions: Optional[OtherOptions] = Field(default_factory=OtherOptions)
     firstHopAlgorithm: Optional[Algorithm] = Field(default_factory=Algorithm)
 
-    @field_validator("protocol")
-    @classmethod
+    @validator("protocol")
     def _valid_protocols(cls, v):
         if v.lower() not in ["tcp", "udp", "icmp"]:
             raise ValueError(f'Protocol "{v}" not in ["tcp", "udp", "icmp"]')
         return v.lower()
 
-    @field_validator("srcPorts", "dstPorts")
-    @classmethod
+    @validator("srcPorts", "dstPorts")
     def _check_ports(cls, v):
-        ports = str(v).replace(" ", "").split(",")
+        ports = v.replace(" ", "").split(",")
         for p in ports:
             if not PORT_REGEX.match(p):
                 raise ValueError(
                     f'Ports "{v}" is not in the valid syntax, examples: ["80", "80,443", "0-1024", "80,8000-8100,8443"]'
                 )
             if "-" in p:
                 pn = p.split("-")
                 if int(pn[0]) >= int(pn[1]):
                     raise ValueError(f'Ports "{p}" is invalid. {pn[0]} must be smaller than {pn[1]}.')
         return str(",".join(ports))
 
-    @field_validator("tcpFlags")
-    @classmethod
+    @validator("tcpFlags")
     def _valid_flags(cls, v):
         v = [f.lower() for f in v] if v else list()
         if all(f in ["ack", "fin", "psh", "rst", "syn", "urg"] for f in v):
             return v
         raise ValueError(f'TCP Flags "{v}" must be None or combination of ["ack", "fin", "psh", "rst", "syn", "urg"]')
 
     def _l4_options(self):
@@ -193,25 +168,23 @@
                 params["l4Options"]["srcPorts"],
             )
         params["srcRegions"], params["dstRegions"] = params["dstRegions"], params["srcRegions"]
         params["startingPoint"], params["destinationPoint"] = params["destinationPoint"], params["startingPoint"]
         return params
 
 
-class Multicast(PathLookup, BaseModel, extra=PYDANTIC_EXTRAS):
-    group: IPv4
-    source: IPv4
-    receiver: Optional[IPv4] = None
-
-    @field_validator("group")
-    @classmethod
-    def _valid_group(cls, v):
-        ip = IPv4Interface(v)
-        if not ip.network.is_multicast:
-            raise ValueError(f'Group IP "{v}" is not a valid Multicast Address.')
+class Multicast(PathLookup, BaseModel):
+    group: Union[IPv4Address, str]
+    source: Union[IPv4Address, str]
+    receiver: Optional[Union[IPv4Address, str]] = None
+
+    @validator("group", "source", "receiver")
+    def _valid_ip(cls, v):
+        if v and not isinstance(v, IPv4Address):
+            raise ValueError(f'IP "{v}" not a valid IP Address')
         return v
 
     def parameters(self):
         parameters = self.base_parameters()
         parameters.update(
             dict(
                 pathLookupType="multicast",
@@ -220,76 +193,86 @@
             )
         )
         if self.receiver:
             parameters["receiver"] = str(self.receiver)
         return parameters
 
 
-class Unicast(PathLookup, BaseModel, extra=PYDANTIC_EXTRAS):
-    startingPoint: IPv4 = Field(title="Source IP Address or Subnet")
-    destinationPoint: IPv4 = Field(title="Destination IP Address or Subnet")
+class Unicast(PathLookup, BaseModel):
+    startingPoint: Union[IPv4Interface, str] = Field(title="Source IP Address or Subnet")
+    destinationPoint: Union[IPv4Interface, str] = Field(title="Destination IP Address or Subnet")
+
+    @validator("startingPoint", "destinationPoint")
+    def _valid_ip(cls, v):
+        if not isinstance(v, IPv4Interface):
+            raise ValueError(f'IP "{v}" not a valid IP Address or Subnet')
+        return v
 
     def parameters(self, swap: bool = False):
         parameters = self.base_parameters()
         parameters.update(
             dict(
                 pathLookupType="unicast",
                 networkMode=self._check_subnets(),
-                startingPoint=self.startingPoint,
-                destinationPoint=self.destinationPoint,
+                startingPoint=self.startingPoint.with_prefixlen,
+                destinationPoint=self.destinationPoint.with_prefixlen,
             )
         )
         return self.swap_src_dst(parameters) if swap else parameters
 
     def _check_subnets(self) -> bool:
         """
         Checks for valid IP Addresses or Subnet
         :param ips: ip addresses
         :return: True if a subnet is found to set to networkMode, False if only hosts
         """
-        masks = {IPv4Interface(ip).network.prefixlen for ip in [self.startingPoint, self.destinationPoint]}
+        masks = {ip.network.prefixlen for ip in [self.startingPoint, self.destinationPoint]}
         return True if masks != {32} else False
 
 
-class Host2GW(BaseModel, extra=PYDANTIC_EXTRAS):
-    startingPoint: IPv4
+class Host2GW(BaseModel):
+    startingPoint: Union[IPv4Address, str]
     vrf: Optional[str] = None
 
+    @validator("startingPoint")
+    def _valid_ip(cls, v):
+        if v and not isinstance(v, IPv4Address):
+            raise ValueError(f'IP "{v}" not a valid IP Address')
+        return v
+
     def parameters(self):
         parameters = dict(
             pathLookupType="hostToDefaultGW",
             type="pathLookup",
             groupBy="siteName",
-            startingPoint=self.startingPoint,
+            startingPoint=str(self.startingPoint),
         )
         if self.vrf:
             parameters["vrf"] = self.vrf
         return parameters
 
 
-class Layout(BaseModel, extra=PYDANTIC_EXTRAS):
+class Layout(BaseModel):
     path: str
     layout: str
 
-    @field_validator("layout")
-    @classmethod
+    @validator("layout")
     def _valid_layout(cls, v):
         if v and v not in VALID_LAYOUTS:
             raise ValueError(f'Layout "{v}" is not in the valid layouts of {VALID_LAYOUTS}')
         return v
 
 
-class Network(BaseModel, extra=PYDANTIC_EXTRAS):
+class Network(BaseModel):
     sites: Optional[Union[str, List[str]]] = [ALL_NETWORK]
     all_network: Optional[bool] = Field(False, description="Show all sites as clouds, UI option 'All Network'")
     layouts: Optional[List[Layout]] = None
     technologies: Optional[Technologies] = None
 
-    @field_validator("sites")
-    @classmethod
+    @validator("sites")
     def _format_paths(cls, v):
         if isinstance(v, str):
             return [v]
         return v
 
     def parameters(self):
         parameters = dict(type="topology", groupBy="siteName", paths=self.sites.copy())
```

### Comparing `ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/input_models/graph_settings.py` & `ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/input_models/graph_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,37 @@
-import os
-import re
 from typing import Optional, List, Union
 from uuid import UUID
 
-from pydantic import field_validator, BaseModel, Field
-from pydantic_extra_types.color import Color
+from pydantic import BaseModel, validator, Field
+from pydantic.color import Color
 
 from .constants import VALID_DEV_TYPES, DEFAULT_NETWORK, DEFAULT_PATHLOOKUP, \
     VALID_NET_PROTOCOLS, VALID_PROTOCOL_LABELS, VALID_PATH_PROTOCOLS
 
-PYDANTIC_EXTRAS = os.getenv("IPFABRIC_PYDANTIC_EXTRAS", "allow")
 
-
-class Style(BaseModel, extra=PYDANTIC_EXTRAS):
+class Style(BaseModel):
     color: Color
     pattern: Optional[str] = 'solid'
     thicknessThresholds: Optional[List[int]] = [2, 4, 8]
 
-    @field_validator("pattern")
-    @classmethod
+    @validator("pattern")
     def _valid_patterns(cls, v):
         if v.lower() not in ["solid", "dashed", "dotted"]:
             raise ValueError(f'Pattern "{v}" not in ["solid", "dashed", "dotted"]')
         return v.lower()
 
     def style_settings(self) -> dict:
         return dict(
             color=self.color.as_hex(),
             pattern=self.pattern,
             thicknessThresholds=self.thicknessThresholds
         )
 
 
-class Setting(BaseModel, extra=PYDANTIC_EXTRAS):
+class Setting(BaseModel):
     name: str
     visible: bool = True
     grouped: bool = True
     style: Style
     type: str
 
     def base_settings(self) -> dict:
@@ -45,59 +40,57 @@
             visible=self.visible,
             grouped=self.grouped,
             style=self.style.style_settings(),
             type=self.type
         )
 
 
-class EdgeSettings(Setting, BaseModel, extra=PYDANTIC_EXTRAS):
+class EdgeSettings(Setting, BaseModel):
     labels: List[str] = ['protocols']
     id: Optional[UUID] = None
 
     def settings(self) -> dict:
         base_settings = self.base_settings()
         base_settings['labels'] = self.labels
         return base_settings
 
 
-class GroupSettings(Setting, BaseModel, extra=PYDANTIC_EXTRAS):
+class GroupSettings(Setting, BaseModel):
     label: str
     children: List[EdgeSettings]
     id: Optional[UUID] = None
 
     def settings(self) -> dict:
         base_settings = self.base_settings()
         base_settings.update(dict(
             children=[child.settings() for child in self.children],
             label=self.label
         ))
         return base_settings
 
 
-class PathLookup(BaseModel, extra=PYDANTIC_EXTRAS):
+class PathLookup(BaseModel):
     ignoredTopics: Optional[List[str]] = Field(
         default_factory=list,
         description="List of topics to ignore.  Valid topics are in ['ACL', 'FORWARDING', 'ZONEFW'].")
     colorDetectedLoops: Optional[bool] = True
 
-    @field_validator('ignoredTopics')
-    @classmethod
+    @validator('ignoredTopics')
     def _valid_topics(cls, v):
         if v and not all(t in ['ACL', 'FORWARDING', 'ZONEFW'] for t in v):
             raise ValueError(f"Ignored Topics '{v}' must be None or in ['ACL', 'FORWARDING', 'ZONEFW'].")
         return v
 
 
-class GraphSettings(BaseModel, extra=PYDANTIC_EXTRAS):
+class GraphSettings(BaseModel):
     edges: List[Union[GroupSettings, EdgeSettings]]
     hiddenDeviceTypes: Optional[List[str]] = Field(default_factory=list)
     pathLookup: Optional[PathLookup] = None
 
-    @field_validator('hiddenDeviceTypes')
-    @classmethod
+    @validator('hiddenDeviceTypes')
     def _valid_dev_types(cls, v):
         if v and not all(d in VALID_DEV_TYPES for d in v):
             raise ValueError(f"Device Types '{v}' must be None or in {VALID_DEV_TYPES}.")
         return v
 
 
 class NetworkSettings(GraphSettings):
@@ -233,32 +226,29 @@
     """Set snapshotToCompare or intentRuleId, not both."""
     snapshotToCompare: Optional[Union[UUID, str]] = Field(None, description="Snapshot ID to compare.")
     intentRuleId: Optional[Union[int, str]] = Field(
         None,
         description="Intent Rule ID to overlay. Also valid: ['nonRedundantEdges', 'singlePointsOfFailure']",
     )
 
-    @field_validator("snapshotToCompare")
-    @classmethod
+    @validator("snapshotToCompare")
     def _valid_snapshot(cls, v):
         if v and v in ["$last", "$prev", "$lastLocked"]:
             return v
         elif v and isinstance(v, UUID):
             return str(v)
-        elif re.match(r"^[\da-f]{8}-([\da-f]{4}-){3}[\da-f]{12}$", v.lower()):
-            return v.lower()
         raise ValueError(f'"{v}" is not a Snapshot ID or in ["$last", "$prev", "$lastLocked"]')
 
-    @field_validator("intentRuleId")
-    @classmethod
+    @validator("intentRuleId")
     def _valid_intentrule(cls, v):
         if v and v in ["nonRedundantEdges", "singlePointsOfFailure"]:
             return v
         try:
-            return str(int(v))
+            int(v)
+            return str(v)
         except ValueError:
             raise ValueError(f'"{v}" is not an Intent Rule ID or in ["nonRedundantEdges", "singlePointsOfFailure"]')
 
     @property
     def type(self):
         return "compare" if self.snapshotToCompare else "intent"
```

### Comparing `ipfabric_diagrams-6.3.0b2/ipfabric/diagrams/output_models/trace.py` & `ipfabric_diagrams-6.3.1b0/ipfabric/diagrams/output_models/trace.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from typing import Optional, List, Union
 
-try:
-    from typing import Annotated, Literal  # py38 required Annotated, Literal py37
-except ImportError:
-    from typing_extensions import Annotated, Literal
-
-
 from pydantic import BaseModel, Field
+from typing_extensions import Annotated
+from typing_extensions import Literal
 
 from .protocols import PROTOCOLS
 
 
 class SeverityInfo(BaseModel):
     name: str
     severity: int
@@ -60,41 +56,41 @@
     header: PROTOCOLS
     headerType: str
     index: int
     type: Literal["insert header"]
 
 
 class Patch(BaseModel):
-    stack: Optional[List[int]] = None
-    ttl: Optional[int] = None
+    stack: Optional[List[int]]
+    ttl: Optional[int]
 
 
 class PatchHeader(BaseModel):
     patch: Patch
     index: int
     type: Literal["patch header"]
 
 
 class DropPacket(BaseModel):
     type: Literal["drop packet"]
     reason: str
-    severityInfo: Optional[SeverityInfo] = None
+    severityInfo: Optional[SeverityInfo]
 
 
 class SeverityEvent(BaseModel):
     type: Literal["severity event"]
-    severityInfo: Optional[SeverityInfo] = None
+    severityInfo: Optional[SeverityInfo]
 
 
 class BaseEvent(BaseModel):
-    decidingPolicyName: Optional[str] = None
-    decidingRule: Optional[List[int]] = None
+    decidingPolicyName: Optional[str]
+    decidingRule: Optional[List[int]]
     protocolId: str
     securityType: str
-    severityInfo: Optional[SeverityInfo] = None
+    severityInfo: Optional[SeverityInfo]
 
 
 class SecurityCheck(BaseEvent, BaseModel):
     type: Literal["security check"]
 
 
 class SecurityCheckIgnored(BaseEvent, BaseModel):
@@ -108,25 +104,25 @@
 
 class AcceptPacket(BaseModel):
     type: Literal["accept packet"]
 
 
 class DestinationNAT(BaseEvent, BaseModel):
     type: Literal["destination NAT"]
-    field: Optional[str] = None
+    field: Optional[str]
 
 
 class SourceNAT(BaseEvent, BaseModel):
     type: Literal["source NAT"]
     field: str
 
 
 class PolicyBasedRouting(BaseEvent, BaseModel):
     type: Literal["policy based routing"]
-    field: Optional[str] = None
+    field: Optional[str]
 
 
 EVENT = Annotated[
     Union[
         PacketDataMatch,
         RemoveHeader,
         TableEntryMatch,
```

### Comparing `ipfabric_diagrams-6.3.0b2/ipfabric_diagrams/__init__.py` & `ipfabric_diagrams-6.3.1b0/ipfabric_diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.3.0b2/ipfabric_diagrams/icmp.py` & `ipfabric_diagrams-6.3.1b0/ipfabric_diagrams/icmp.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.3.0b2/LICENSE` & `ipfabric_diagrams-6.3.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.3.0b2/pyproject.toml` & `ipfabric_diagrams-6.3.1b0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipfabric-diagrams"
-version = "v6.3.0b2"
+version = "v6.3.1b0"
 description = "Python package for interacting with IP Fabric Diagrams"
 authors = [
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
     "Community Fabric <communityfabric@ipfabric.io>"
 ]
 license = "MIT"
 readme = "README.md"
@@ -17,23 +17,22 @@
 ]
 
 [tool.poetry.urls]
 "IP Fabric" = "https://ipfabric.io/"
 "Changelog" = "https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams/-/blob/develop/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
-ipfabric = "6.3.0b2"  # TODO: Change when released
-typing-extensions = {version = "^4.7.1", python = "<3.9"}  # TODO: Remove after Python 3.8
-rich = {version = "^13.4.2", optional = true}
-pydantic-extra-types = "^2.0.0"
+python = "^3.8"
+ipfabric = "6.3.1b2"
+typing-extensions = "^4.5"
+rich = {version = "^13.3.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.0"
-pytest-cov = "^4.1.0"
+pytest = "^7.2.0"
+pytest-cov = "^4.0.0"
 flake8 = "^5.0.4"
 black = "^22.12"
 
 [tool.poetry.extras]
 examples = ["rich"]
 
 [build-system]
```

### Comparing `ipfabric_diagrams-6.3.0b2/README.md` & `ipfabric_diagrams-6.3.1b0/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.3.0b2/setup.py` & `ipfabric_diagrams-6.3.1b0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,32 +9,31 @@
  'ipfabric.diagrams.output_models',
  'ipfabric_diagrams']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['ipfabric==6.3.0b2', 'pydantic-extra-types>=2.0.0,<3.0.0']
+['ipfabric==6.3.1b2', 'typing-extensions>=4.5,<5.0']
 
 extras_require = \
-{':python_version < "3.9"': ['typing-extensions>=4.7.1,<5.0.0'],
- 'examples': ['rich>=13.4.2,<14.0.0']}
+{'examples': ['rich>=13.3.0,<14.0.0']}
 
 setup_kwargs = {
     'name': 'ipfabric-diagrams',
-    'version': '6.3.0b2',
+    'version': '6.3.1b0',
     'description': 'Python package for interacting with IP Fabric Diagrams',
     'long_description': "# IP Fabric\n\nipfabric_diagrams is a Python module for connecting to and graphing topologies against an IP Fabric instance.\n\n## About\n\nFounded in 2015, [IP Fabric](https://ipfabric.io/) develops network infrastructure visibility and analytics solution to\nhelp enterprise network and security teams with network assurance and automation across multi-domain heterogeneous\nenvironments. From in-depth discovery, through graph visualization, to packet walks and complete network history, IP\nFabric enables to confidently replace manual tasks necessary to handle growing network complexity driven by relentless\ndigital transformation.\n\n## v6.3.1 Deprecation Notices\n\nIn `ipfabric>=v6.3.1` Python 3.7 support will be removed.  This was originally\nplanned for `v7.0.0` however to add new functionality of Pandas Dataframe we\nare required to move this forward.\n\n**Python 3.7 is now End of Life as of June 27th 2023**\n\n## v7.0.0 Deprecation Notices\n\nIn `ipfabric>=v7.0.0` the following will be deprecated:\n\n- `ipfabric_diagrams` package will move to `ipfabric.diagrams`\n- The use of `token='<TOKEN>'` or `username='<USER>', password='<PASS>'` in `IPFClient()` will be removed:\n  - Token: `IPFClient(auth='TOKEN')`\n  - User/Pass: `IPFClient(auth=('USER', 'PASS'))`\n  - `.env` file will only accept `IPF_TOKEN` or (`IPF_USERNAME` and `IPF_PASSWORD`) and not `auth`\n\n## Versioning\n\nStarting with IP Fabric version 5.0.x the python-ipfabric and python-ipfabric-diagrams will need to\nmatch your IP Fabric version.  The API's are changing and instead of `api/v1` they will now be `api/v5.0`.\n\nVersion 5.1 will have backwards compatability with version 5.0 however 6.0 will not support any 5.x versions.\nBy ensuring that your ipfabric SDK's match your IP Fabric Major Version will ensure compatibility and will continue to work.\n\n## Installation\n\n```\npip install ipfabric-diagrams\n```\n\n## Introduction\n\nThis package is used for diagramming via the API for IP Fabric v4.3.0.  \nExamples can be located under [examples](examples/) directory.\n\n## Authentication\nPlease take a look at [python-ipfabric](https://gitlab.com/ip-fabric/integrations/python-ipfabric#authentication) \nfor all authentication options.\n\n```python\nfrom ipfabric.diagrams import IPFDiagram\nipf = IPFDiagram(base_url='https://demo3.ipfabric.io/', auth='token', verify=False, timeout=15)\n```\n\n## Development\n\nIPFabric uses poetry for the python packaging module. Install poetry globally:\n\n```\npip install poetry\n```\n\nTo install a virtual environment run the following command in the root of this directory.\n\n```\npoetry install\n```\n\nTo test and build:\n\n```\npoetry run pytest\npoetry build\n```\n\nPrior to pushing changes run:\n```\npoetry run black ipfabric_diagrams ipfabric\npoetry update\n```\n",
     'author': 'Justin Jeffery',
     'author_email': 'justin.jeffery@ipfabric.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.7.1,<4.0.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `ipfabric_diagrams-6.3.0b2/PKG-INFO` & `ipfabric_diagrams-6.3.1b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: ipfabric-diagrams
-Version: 6.3.0b2
+Version: 6.3.1b0
 Summary: Python package for interacting with IP Fabric Diagrams
 Home-page: https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Justin Jeffery
 Author-email: justin.jeffery@ipfabric.io
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: examples
-Requires-Dist: ipfabric (==6.3.0b2)
-Requires-Dist: pydantic-extra-types (>=2.0.0,<3.0.0)
-Requires-Dist: rich (>=13.4.2,<14.0.0) ; extra == "examples"
-Requires-Dist: typing-extensions (>=4.7.1,<5.0.0) ; python_version < "3.9"
+Requires-Dist: ipfabric (==6.3.1b2)
+Requires-Dist: rich (>=13.3.0,<14.0.0) ; extra == "examples"
+Requires-Dist: typing-extensions (>=4.5,<5.0)
 Project-URL: Changelog, https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams/-/blob/develop/CHANGELOG.md
 Project-URL: IP Fabric, https://ipfabric.io/
 Project-URL: Repository, https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams
 Description-Content-Type: text/markdown
 
 # IP Fabric
```

