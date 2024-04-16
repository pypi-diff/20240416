# Comparing `tmp/boario-0.5.7.tar.gz` & `tmp/boario-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boario-0.5.7.tar", max compression
+gzip compressed data, was "boario-0.5.8.tar", max compression
```

## Comparing `boario-0.5.7.tar` & `boario-0.5.8.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0    35149 2024-03-07 07:52:20.849427 boario-0.5.7/LICENSE
--rw-r--r--   0        0        0     5269 2024-03-13 16:25:58.791001 boario-0.5.7/README.rst
--rw-r--r--   0        0        0     2011 2024-03-07 07:52:20.849427 boario-0.5.7/boario/__init__.py
--rw-r--r--   0        0        0    52348 2024-03-07 07:52:20.849427 boario-0.5.7/boario/event.py
--rw-r--r--   0        0        0     8045 2024-03-07 07:52:20.849427 boario-0.5.7/boario/extended_models.py
--rw-r--r--   0        0        0    70878 2024-03-07 07:52:20.849427 boario-0.5.7/boario/model_base.py
--rw-r--r--   0        0        0    41996 2024-03-14 09:35:04.206252 boario-0.5.7/boario/simulation.py
--rw-r--r--   0        0        0     4949 2024-03-07 07:52:20.849427 boario-0.5.7/boario/utils/misc.py
--rw-r--r--   0        0        0     4066 2024-03-07 07:52:20.849427 boario-0.5.7/boario/utils/recovery_functions.py
--rw-r--r--   0        0        0     2355 2024-03-15 09:27:14.262192 boario-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     6187 1970-01-01 00:00:00.000000 boario-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-07 07:52:20.849427 boario-0.5.8/LICENSE
+-rw-r--r--   0        0        0     5510 2024-04-16 12:01:59.867821 boario-0.5.8/README.rst
+-rw-r--r--   0        0        0     2082 2024-04-16 12:01:59.867821 boario-0.5.8/boario/__init__.py
+-rw-r--r--   0        0        0    58513 2024-04-16 12:01:59.867821 boario-0.5.8/boario/event.py
+-rw-r--r--   0        0        0     8076 2024-04-16 12:01:59.867821 boario-0.5.8/boario/extended_models.py
+-rw-r--r--   0        0        0    70939 2024-04-16 12:01:59.871821 boario-0.5.8/boario/model_base.py
+-rw-r--r--   0        0        0    42008 2024-04-16 12:01:59.871821 boario-0.5.8/boario/simulation.py
+-rw-r--r--   0        0        0     3568 2024-04-14 08:59:21.723881 boario-0.5.8/boario/utils/__pycache__/misc.cpython-310.pyc
+-rw-r--r--   0        0        0     3977 2024-03-14 07:49:40.040054 boario-0.5.8/boario/utils/__pycache__/recovery_functions.cpython-310.pyc
+-rw-r--r--   0        0        0     4894 2024-04-16 12:01:59.871821 boario-0.5.8/boario/utils/misc.py
+-rw-r--r--   0        0        0     4066 2024-03-07 07:52:20.849427 boario-0.5.8/boario/utils/recovery_functions.py
+-rw-r--r--   0        0        0     2474 2024-04-16 12:01:59.871821 boario-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     6433 1970-01-01 00:00:00.000000 boario-0.5.8/PKG-INFO
```

### Comparing `boario-0.5.7/LICENSE` & `boario-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `boario-0.5.7/README.rst` & `boario-0.5.8/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 .. role:: pythoncode(code)
    :language: python
 
 #######
 BoARIO
 #######
+|build-status| |black| |contribute| |licence| |pypi| |pythonv| |joss|
 
-
-.. image:: https://img.shields.io/github/actions/workflow/status/spjuhel/boario/CI.yml
+.. |build-status| image:: https://img.shields.io/github/actions/workflow/status/spjuhel/boario/CI.yml
    :target: https://github.com/spjuhel/BoARIO/actions/workflows/CI.yml
    :alt: GitHub Actions Workflow Status
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000
    :target: https://github.com/psf/black
    :alt: Code Style - Black
-
-.. image:: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
+.. |contribute| image:: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
    :target: https://github.com/spjuhel/BoARIO/issues
    :alt: Contribution - Welcome
-
-.. image:: https://img.shields.io/badge/License-GPLv3-blue
+.. |licence| image:: https://img.shields.io/badge/License-GPLv3-blue
    :target: https://www.gnu.org/licenses/gpl-3.0
    :alt: Licence - GPLv3
-
-.. image:: https://img.shields.io/pypi/v/boario
+.. |pypi| image:: https://img.shields.io/pypi/v/boario
    :target: https://pypi.org/project/boario/
    :alt: PyPI - Version
-
-.. image:: https://img.shields.io/pypi/pyversions/boario
+.. |pythonv| image:: https://img.shields.io/pypi/pyversions/boario
    :target: https://pypi.org/project/boario/
    :alt: PyPI - Python Version
-
-.. image:: https://joss.theoj.org/papers/71386aa01a292ecff8bafe273b077701/status.svg
+.. |joss| image:: https://joss.theoj.org/papers/71386aa01a292ecff8bafe273b077701/status.svg
    :target: https://joss.theoj.org/papers/71386aa01a292ecff8bafe273b077701
    :alt: Joss Status
 
 `BoARIO` : The Adaptative Regional Input Output model in python.
 
 .. _`Documentation Website`: https://spjuhel.github.io/BoARIO/boario-what-is.html
 
@@ -84,14 +78,20 @@
 
 You can install BoARIO from ``pip`` with:
 
 .. code:: console
 
    pip install boario
 
+Or from ``conda-forge`` using conda (or mamba):
+
+.. code:: console
+
+   conda install -c conda-forge boario
+
 
 The full source code is also available on Github at: https://github.com/spjuhel/BoARIO
 
 More info in the `installation <https://spjuhel.github.io/BoARIO/boario-installation.html>`_ page of the documentation.
 
 How does BoARIO work?
 =========================
@@ -109,15 +109,15 @@
 - the step by step, sector by sector, region by region evolution of most of the variables involved in the simulation (`production`, `demand`, `stocks`, ...)
 
 - aggregated indicators for the whole simulation (`shortages duration`, `aggregated impacts`, ...)
 
 Example of use
 =================
 
-See `Boario quickstart <https://spjuhel.github.io/BoARIO/boario-quickstart.html>`_.
+See `Boario quickstart <https://spjuhel.github.io/BoARIO/boario-tutorials.html>`_.
 
 Credits
 ========
 
 Associated PhD project
 ------------------------
 
@@ -130,15 +130,15 @@
            :alt: ADEME Logo
 
 .. _`ADEME`: https://www.ademe.fr/
 
 Development
 ------------
 
-* Samuel Juhel (pro@sjuhel.org)
+** Samuel Juhel (pro@sjuhel.org)
 
 Contributions
 ---------------
 
 All `contributions <https://spjuhel.github.io/BoARIO/development.html>`_ to the project are welcome !
 
 Acknowledgements
```

### Comparing `boario-0.5.7/boario/__init__.py` & `boario-0.5.8/boario/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+"""BoARIO : The Adaptative Regional Input Output model in python."""
+
 try:
     import coloredlogs as coloredlogs  # noqa: F401
 except ImportError:
     _has_coloredlogs = False
 else:
     _has_coloredlogs = True
```

### Comparing `boario-0.5.7/boario/event.py` & `boario-0.5.8/boario/event.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,24 +58,39 @@
     r"(?i)(?=.*household)(?=.*final)(?!.*NPISH|profit).*|HFCE"
 )
 
 LOW_DEMAND_THRESH = 10
 
 
 class Event(ABC):
-    # Class Attributes
+    r"""An Event object stores all information about a unique shock during simulation
+    such as time of occurrence, duration, type of shock, amount of damages.
+    Computation of recovery or initially requested rebuilding demand is also
+    done in this class.
+
+    .. warning::
+       The Event class is abstract and cannot be instantiated directly. Only its non-abstract subclasses can be instantiated.
+
+    .. note::
+       Events should be constructed using :py:meth:`~Event.from_series()`, :py:meth:`~Event.from_dataframe()`, :py:meth:`~Event.from_scalar_industries()` or from :py:meth:`~Event.from_scalar_regions_sectors()`.
+       Depending on the type of event chosen, these constructors require additional keyword arguments, that are documented for each instantiable Event subclass.
+       For instance, :py:class:`EventKapitalRebuild` additionally requires `rebuild_tau` and `rebuilding_sectors`.
+
+    .. seealso::
+       Tutorial :ref:`boario-events`
+    """
 
     possible_sectors: pd.Index = pd.Index([])
-    r"""List of sectors present in the MRIO used by the model"""
+    r"""List of sectors present in the MRIOT used by the model"""
 
     possible_regions: pd.Index = pd.Index([])
-    r"""List of regions present in the MRIO used by the model"""
+    r"""List of regions present in the MRIOT used by the model"""
 
     possible_final_demand_cat: pd.Index = pd.Index([])
-    r"""List of final demand categories present in the MRIO used by the model"""
+    r"""List of final demand categories present in the MRIOT used by the model"""
 
     temporal_unit_range: int = 0
     r"""Maximum temporal unit simulated"""
 
     z_shape: tuple[int, int] = (0, 0)
     r"""Shape of the Z (intermediate consumption) matrix in the model"""
 
@@ -88,58 +103,40 @@
     regions_idx: npt.NDArray = np.array([])
     r"""lexicographic region indexes"""
 
     sectors_idx: npt.NDArray = np.array([])
     r"""lexicographic sector indexes"""
 
     model_monetary_factor: int = 1
-    r"""Amount of unitary currency used in the MRIO (e.g. 1000000 if in € millions)"""
+    r"""Amount of unitary currency used in the MRIOT (e.g. 1000000 if in € millions)"""
 
     gva_df: pd.Series = pd.Series([], dtype="float64")
     r"""GVA per (region,sector)"""
 
     sectors_gva_shares: npt.NDArray = np.array([])
     r"""Fraction of total (regional) GVA for each sectors"""
 
     Z_distrib: npt.NDArray = np.array([])
     r"""Normalized intermediate consumption matrix"""
 
     Y_distrib: npt.NDArray = np.array([])
     r"""Normalized final consumption matrix"""
 
     mrio_name: str = ""
-    r"""MRIO identification"""
+    r"""MRIOT identification"""
 
     @abstractmethod
     def __init__(
         self,
         *,
         impact: pd.Series,
         name: str | None = "Unnamed",
         occurrence: int = 1,
         duration: int = 1,
     ) -> None:
-        r"""Create an event shocking the model from a dictionary.
-
-        An Event object stores all information about a unique shock during simulation such as
-        time of occurrence, duration, type of shock, amount of damages. Computation
-        of recovery or initially requested rebuilding demand is also done in this
-        class.
-
-        Parameters
-        ----------
-
-        event : dict
-            A dictionary holding the necessary information to define an event.
-
-        Examples
-        --------
-            FIXME: Add docs.
-
-        """
         logger.info("Initializing new Event")
         logger.debug("Checking required Class attributes are defined")
 
         if np.size(self.possible_regions) == 0 or np.size(self.possible_sectors) == 0:
             raise AttributeError(
                 "It appears that no model has been instantiated as some class attributes are not initialized (possible_regions, possible_sectors). Events require to instantiate a model and a simulation context before they can be instantiated"
             )
@@ -202,27 +199,57 @@
         impact: pd.Series,
         *,
         occurrence: int = 1,
         duration: int = 1,
         name: Optional[str] = None,
         **kwarg,
     ) -> Event:
-        """Create an event from an impact pd.Series.
+        """Create an event for an impact given as a pd.Series.
 
-        Args:
-            impact (pd.Series): A vector definition of the impact per (region,sector)
-            occurrence (int, optional): The ordinal of occurrence of the event (requires to be > 0). Defaults to 1.
-            duration (int, optional): The duration of the event (entire impact applied during this number of steps). Defaults to 1.
-            name (Optional[str], optional): A possible name for the event, for convenience. Defaults to None.
+        Parameters
+        ----------
+        impact : pd.Series
+            A pd.Series defining the impact per (region, sector)
+        occurrence : int
+            The ordinal of occurrence of the event (requires to be > 0). Defaults to 1.
+        duration : int
+            The duration of the event (entire impact applied during this number of steps). Defaults to 1.
+        name : Optional[str]
+            A possible name for the event, for convenience. Defaults to None.
+        **kwarg :
+            Keyword arguments keyword arguments to pass to the instantiating method
+        (depends on the type of event).
 
-        Raises:
-            ValueError: Raised if impact is empty or contains negative values.
+        Returns
+        -------
+        Event
+            An Event object or one of its subclass
+
+        Raises
+        ------
+        ValueError
+            Raised if impact is empty of contains negative values.
+
+        Examples
+        --------
+        >>> import pandas as pd
+        >>> import pymrio as pym
+        >>> from boario.simulation import Simulation
+        >>> from boario.extended_model import ARIOPsiModel
+        >>> from boario.event import EventKapitalRecover
+        >>>
+        >>> mriot = pym.load_test()
+        >>> mriot.calc_all()
+        >>>
+        >>> impact_series = pd.Series({('reg1', 'electricity'): 100000.0, ('reg1', 'mining'): 50000.0})
+        >>> model = ARIOPsiModel(mriot)
+        >>> sim = Simulation(model)
+        >>> event = EventKapitalRecover.from_series(impact_series, occurrence=5, duration=10, recovery_time=30, name="Event 1")
+        >>> sim.add_event(event)
 
-        Returns:
-            Event: an Event object (or one of its subclass).
         """
         if impact.size == 0:
             raise ValueError(
                 "Empty impact Series at init, did you not set the impact correctly ?"
             )
         impact = impact[impact != 0]
         if np.less_equal(impact, 0).any():
@@ -242,21 +269,39 @@
         impact: pd.DataFrame,
         *,
         occurrence: int = 1,
         duration: int = 1,
         name: Optional[str] = None,
         **kwarg,
     ) -> Event:
-        """Convenience function for DataFrames. See :meth:`~boario.event.Event.from_series`
+        """Convenience function for DataFrames. See :meth:`~boario.event.Event.from_series`. This constructor only apply ``.squeeze()`` to the given DataFrame.
 
-        Raises:
-            ValueError: If impact cannot be squeezed to a Series
+        Parameters
+        ----------
+        impact : pd.DataFrame
+           A pd.DataFrame defining the impact per (region, sector)
+        occurrence : int
+            The ordinal of occurrence of the event (requires to be > 0). Defaults to 1.
+        duration : int
+            The duration of the event (entire impact applied during this number of steps). Defaults to 1.
+        name : Optional[str]
+            A possible name for the event, for convenience. Defaults to None.
+        **kwarg :
+            Keyword arguments
+            Other keyword arguments to pass to the instantiate method (depends on the type of event)
+
+        Raises
+        ------
+        ValueError
+            If impact cannot be squeezed to a Series
 
-        Returns:
-            Event: an Event object (or one of its subclass).
+        Returns
+        -------
+        Event
+           An Event object (or one of its subclass).
         """
         impact = impact.squeeze()
         if not isinstance(impact, pd.Series):
             raise ValueError("Could not squeeze impact dataframe to a serie.")
 
         return cls.from_series(
             impact=impact,
@@ -269,75 +314,100 @@
     @classmethod
     def distribute_impact_by_gva(cls, impact_vec: pd.Series) -> pd.Series:
         """Distribute a vector of impact by the GVA of affected industries.
 
         Each values of the given impact are mutliplied by the share of the GVA
         the industry has over the GVA of all affected industries.
 
-        Args:
-            impact_vec (pd.Series): The impact values to be reweigthed.
-            Current use-case assumes all values are the total impact.
-
-        Returns:
-            pd.Series: The impact where each value was multiplied by the share
-            of GVA of each affected industry (over total GVA affected).
+        Parameters
+        ----------
+        impact_vec : pd.Series
+            The impact values to be reweigthed. Current use-case assumes all values are the total impact.
+
+        Returns
+        -------
+        pd.Series
+            The impact where each value was multiplied by the share of GVA of each affected industry (over total GVA affected).
+
         """
         gva = cls.gva_df.loc[impact_vec.index]
         gva = gva.transform(lambda x: x / sum(x))
         return impact_vec * gva
 
     @classmethod
     def distribute_impact_equally(cls, impact_vec: pd.Series) -> pd.Series:
         """Distribute an impact equally between all affected regions.
 
         Assume impact is given as a vector with all value being the
         total impact to distribute.
 
-        Args:
-            impact_vec (pd.Series): The impact to distribute.
+        Parameters
+        ----------
+        impact_vec : pd.Series
+            The impact to distribute.
+
+        Returns
+        -------
+        pd.Series
+            The impact vector equally distributed among affected industries.
 
-        Returns:
-            pd.Series: The impact vector equally distributed among affected industries.
         """
         dfg = impact_vec.groupby("region")
         return dfg.transform(lambda x: x / (dfg.ngroups * x.count()))
 
     @classmethod
     def from_scalar_industries(
         cls,
         impact: ScalarImpact,
         *,
         industries: IndustriesList,
         impact_industries_distrib: Optional[npt.ArrayLike] = None,
-        gva_distrib: bool = False,
-        occurrence: int = 1,
-        duration: int = 1,
+        gva_distrib: Optional[bool] = False,
+        occurrence: Optional[int] = 1,
+        duration: Optional[int] = 1,
         name: Optional[str] = None,
         **kwarg,
     ) -> Event:
         """Creates an Event from a scalar and a list of industries affected.
 
-        The scalar impact is distributed evenly by default. Otherwise it can be distributed proportionnaly to the GVA of
-        affected industries, or to a custom distribution.
+        The scalar impact is distributed evenly by default. Otherwise it can
+        be distributed proportionnaly to the GVA of affected industries, or to
+        a custom distribution.
 
-        Args:
-            impact (ScalarImpact): The scalar impact.
-            industries (IndustriesList): The list of industries affected by the impact
-            impact_industries_distrib (Optional[npt.ArrayLike], optional): A vector of equal size to the list of industries, stating the
+        Parameters
+        ----------
+        impact : ScalarImpact
+            The scalar impact.
+        industries : IndustriesList
+            The list of industries affected by the impact.
+        impact_industries_distrib : Optional[npt.ArrayLike]
+            A vector of equal size to the list of industries, stating the
             share of the impact each industry should receive. Defaults to None.
-            gva_distrib (bool, optional): A boolean stating if the impact should be distributed proportionnaly to GVA. Defaults to False.
-            occurrence (int, optional): The ordinal of occurrence of the event (requires to be > 0). Defaults to 1.
-            duration (int, optional): The duration of the event (entire impact applied during this number of steps). Defaults to 1.
-            name (Optional[str], optional): A possible name for the event, for convenience. Defaults to None.
+        gva_distrib : Optional[bool]
+            A boolean stating if the impact should be distributed proportionnaly to GVA. Defaults to False.
+        occurrence : Optional[int]
+            The ordinal of occurrence of the event (requires to be > 0). Defaults to 1.
+        duration : Optional[int]
+            The duration of the event (entire impact applied during this number of steps). Defaults to 1.
+        name : Optional[str]
+            A possible name for the event, for convenience. Defaults to None.
+        **kwarg :
+            Keyword arguments
+            Other keyword arguments to pass to the instantiate method (depends on the type of event)
+
+        Raises
+        ------
+        ValueError
+            Raised if Impact is null, if len(industries) < 1 or if the sum of impact_industries_distrib differs from 1.0.
 
-        Raises:
-            ValueError: Raise if Impact is null, if len(industries) < 1 or if the sum of impact_industries_distrib differs from 1.0.
+        Returns
+        -------
+        Event
+            An Event object or one of its subclass.
 
-        Returns:
-            Event: An Event object or one of its subclass.
         """
         if impact <= 0:
             raise ValueError("Impact is null")
 
         if len(industries) < 1:
             raise ValueError("Null sized affected industries ?")
 
@@ -380,33 +450,50 @@
         occurrence: int = 1,
         duration: int = 1,
         name: Optional[str] = None,
         **kwarg,
     ) -> Event:
         """Creates an Event from a scalar, a list of regions and a list of sectors affected.
 
-
-
-        Args:
-            impact (ScalarImpact): The scalar impact.
-            regions (RegionsList): The list of regions affected.
-            sectors (SectorsList): The list of sectors affected in each region.
-            impact_regional_distrib (Optional[npt.ArrayLike], optional): A vector of equal size to the list of regions affected, stating the
-            share of the impact each industry should receive. Defaults to None.
-            impact_sectoral_distrib (Optional[Union[str, npt.ArrayLike]], optional): A vector of equal size to the list of sectors affected, stating the
+        Parameters
+        ----------
+        impact : ScalarImpact
+            The scalar impact.
+        regions : RegionsList
+            The list of regions affected.
+        sectors : SectorsList
+            The list of sectors affected in each region.
+        impact_regional_distrib : Optional[npt.ArrayLike], optional
+            A vector of equal size to the list of regions affected, stating the
             share of the impact each industry should receive. Defaults to None.
-            occurrence (int, optional): The ordinal of occurrence of the event (requires to be > 0). Defaults to 1.
-            duration (int, optional): The duration of the event (entire impact applied during this number of steps). Defaults to 1.
-            name (Optional[str], optional): A possible name for the event, for convenience. Defaults to None.
+        impact_sectoral_distrib : Optional[Union[str, npt.ArrayLike]], optional
+            Either:
+
+            * ``\"gdp\"``, the impact is then distributed using the gross value added of each sector as a weight.
+            * A vector of equal size to the list of sectors affected, stating the share of the impact each industry should receive. Defaults to None.
 
-        Raises:
-            ValueError: Raise if Impact is null, if len(regions) or len(sectors) < 1,
+        occurrence : int, optional
+            The ordinal of occurrence of the event (requires to be > 0). Defaults to 1.
+        duration : int, optional
+            The duration of the event (entire impact applied during this number of steps). Defaults to 1.
+        name : Optional[str], optional
+            A possible name for the event, for convenience. Defaults to None.
+        **kwarg :
+            Keyword arguments
+            Other keyword arguments to pass to the instantiate method (depends on the type of event)
+
+        Raises
+        ------
+        ValueError
+            Raise if Impact is null, if len(regions) or len(sectors) < 1,
 
-        Returns:
-            Event: An Event object or one of its subclass
+        Returns
+        -------
+        Event
+            An Event object or one of its subclass.
         """
         if impact <= 0:
             raise ValueError("Impact is null")
 
         if isinstance(regions, str):
             regions = [regions]
 
@@ -446,23 +533,23 @@
 
         assert isinstance(_regions, pd.Index)
         if impact_regional_distrib is None:
             regional_distrib = pd.Series(1.0 / len(_regions), index=_regions)
         elif not isinstance(impact_regional_distrib, pd.Series):
             impact_regional_distrib = pd.Series(impact_regional_distrib, index=_regions)
             regional_distrib = pd.Series(0.0, index=_regions)
-            regional_distrib.loc[
-                impact_regional_distrib.index
-            ] = impact_regional_distrib
+            regional_distrib.loc[impact_regional_distrib.index] = (
+                impact_regional_distrib
+            )
         else:
             regional_distrib = pd.Series(0.0, index=_regions)
             try:
-                regional_distrib.loc[
-                    impact_regional_distrib.index
-                ] = impact_regional_distrib
+                regional_distrib.loc[impact_regional_distrib.index] = (
+                    impact_regional_distrib
+                )
             except KeyError:
                 regional_distrib.loc[_regions] = impact_regional_distrib.values
 
         assert isinstance(_sectors, pd.Index)
         if impact_sectoral_distrib is None:
             sectoral_distrib = pd.Series(1.0 / len(_sectors), index=_sectors)
         elif (
@@ -470,23 +557,23 @@
             and impact_sectoral_distrib == "gdp"
         ):
             gva = cls.gva_df.loc[(_regions, _sectors)]
             sectoral_distrib = gva.groupby("region").transform(lambda x: x / sum(x))
         elif not isinstance(impact_sectoral_distrib, pd.Series):
             impact_sectoral_distrib = pd.Series(impact_sectoral_distrib, index=_sectors)
             sectoral_distrib = pd.Series(0.0, index=_sectors)
-            sectoral_distrib.loc[
-                impact_sectoral_distrib.index
-            ] = impact_sectoral_distrib
+            sectoral_distrib.loc[impact_sectoral_distrib.index] = (
+                impact_sectoral_distrib
+            )
         else:
             sectoral_distrib = pd.Series(0.0, index=_sectors)
             try:
-                sectoral_distrib.loc[
-                    impact_sectoral_distrib.index
-                ] = impact_sectoral_distrib
+                sectoral_distrib.loc[impact_sectoral_distrib.index] = (
+                    impact_sectoral_distrib
+                )
             except KeyError:
                 sectoral_distrib.loc[_sectors] = impact_sectoral_distrib.values
 
         logger.debug(f"{sectoral_distrib}")
         logger.debug(f"{regional_distrib}")
         if isinstance(sectoral_distrib.index, pd.MultiIndex):
             industries_distrib = sectoral_distrib * regional_distrib
@@ -529,27 +616,15 @@
         self.aff_industries = self.impact_df.loc[self.impact_df > 0].index  # type: ignore
         self.impact_industries_distrib = self.impact_df.transform(lambda x: x / sum(x))
         self.total_impact = self.impact_df.sum()
         self.impact_vector = self.impact_df.values
 
     @property
     def aff_industries(self) -> pd.MultiIndex:
-        r"""The industries affected by the event.
-
-        Parameters
-        ----------
-
-        index : pd.MultiIndex
-             The affected industries as a pandas MultiIndex
-
-        Returns
-        -------
-             A pandas MultiIndex with the regions affected as first level, and sectors affected as second level
-
-        """
+        r"""The industries affected by the event."""
 
         return self._aff_industries
 
     @aff_industries.setter
     def aff_industries(self, index: pd.MultiIndex):
         if not isinstance(index, pd.MultiIndex):
             raise ValueError(
@@ -691,36 +766,56 @@
         self._impact_regional_distrib = self._impact_industries_distrib.groupby(
             "region",
             observed=False,
         ).sum()
 
     def __repr__(self):
         # TODO: find ways to represent long lists
-        return f"""
+        return f"""[WIP]
         Event(
               name = {self.name},
               occur = {self.occurrence},
               duration = {self.duration}
               aff_regions = {self.aff_regions.to_list()},
               aff_sectors = {self.aff_sectors.to_list()},
              )
         """
 
 
 class EventArbitraryProd(Event):
+    r"""An EventArbitraryProd object holds an event with arbitrary impact on production capacity.
+
+    Such events can be used to represent temporary loss of production capacity in a completely exogenous way (e.g., loss of working hours from a heatwave).
+
+    .. warning::
+       This type of event suffers from a problem with the recovery and does not function properly at the moment.
+
+    .. note::
+       For this type of event, the impact value represent the share of production capacity lost of an industry.
+
+    .. note::
+       In addition to the base arguments of an Event, EventArbitraryProd requires a ``recovery_time`` (1 step by default) and a ``recovery_function`` (linear by default).
+
+    .. seealso::
+       Tutorial :ref:`boario-events`
+    """
+
     def __init__(
         self,
         *,
         impact: pd.Series,
         recovery_time: int = 1,
         recovery_function: str = "linear",
         name: str | None = "Unnamed",
         occurrence: int = 1,
         duration: int = 1,
     ) -> None:
+        raise NotImplementedError(
+            "This type of Event suffers from a major bug and cannot be used at the moment."
+        )
         if (impact > 1.0).any():
             raise ValueError(
                 "Impact is greater than 100% (1.) for at least an industry."
             )
 
         super().__init__(
             impact=impact,
@@ -845,14 +940,28 @@
             fun,
             init_impact_stock=self._prod_cap_delta_arbitrary_0,
             recovery_time=self.recovery_time,
         )
         self._recovery_fun = r_fun_partial
 
     def recovery(self, current_temporal_unit: int):
+        """Apply the recovery function to the capital destroyed for the current temporal unit.
+
+        Parameters
+        ----------
+        current_temporal_unit : int
+            The current temporal unit
+
+        Raises
+        ------
+        RuntimeError
+            Raised if no recovery function has been set.
+
+        """
+
         elapsed = current_temporal_unit - (self.occurrence + self.duration)
         if elapsed < 0:
             raise RuntimeError("Trying to recover before event is over")
         if self.recovery_function is None:
             raise RuntimeError(
                 "Trying to recover event while recovery function isn't set yet"
             )
@@ -861,14 +970,29 @@
         res = np.around(res, precision)
         if not np.any(res):
             self.over = True
         self._prod_cap_delta_arbitrary = res
 
 
 class EventKapitalDestroyed(Event, ABC):
+    r"""EventKapitalDestroyed is an abstract class to hold events with where some capital (from industries or households) is destroyed. See :py:class:`EventKapitalRecover` and :py:class:`EventKapitalRebuild` for its instantiable classes.
+
+    .. note::
+       For this type of event, the impact value represent the amount of capital destroyed in monetary terms.
+
+    .. note::
+       We distinguish between impacts on household and industrial (productive) capital. We assume destruction of the former not to reduce production capacity contrary to the latter (but possibly induce reconstruction demand). Impacts on household capital is null by default, but can be set via the ``households_impacts`` argument in the constructor. The amount of production capacity lost is computed as the share of capital lost over total capital of the industry.
+
+    .. note::
+       The user can specify a monetary factor via the ``event_monetary_factor`` argument for the event if it differs from the monetary factor of the MRIOT used. By default the constructor assumes the two factors to be the same (i.e., if the MRIOT is in €M, the so is the impact).
+
+    .. seealso::
+       Tutorial :ref:`boario-events`
+    """
+
     def __init__(
         self,
         *,
         impact: pd.Series,
         households_impact: Optional[Impact] = None,
         name: str | None = "Unnamed",
         occurrence: int = 1,
@@ -1006,14 +1130,30 @@
                     value.shape, self.x_shape
                 )
             )
         self._regional_sectoral_productive_capital_destroyed = value
 
 
 class EventKapitalRebuild(EventKapitalDestroyed):
+    r"""EventKapitalRebuild holds a :py:class:`EventKapitalDestroyed` event where the destroyed capital requires to be rebuilt, and creates a reconstruction demand.
+
+    This subclass requires and enables new arguments to pass to the constructor:
+
+    * A characteristic time for reconstruction (``tau_rebuild``)
+    * A set of sectors responsible for the reconstruction (``rebuilding_sectors``)
+    * A ``rebuilding_factor`` in order to modulate the reconstruction demand. By default, this factor is 1, meaning that the entire impact value is translated as an additional demand.
+
+    .. note::
+       The ``tau_rebuild`` of an event takes precedence over the one defined for a model.
+
+    .. seealso::
+       Tutorial :ref:`boario-events`
+
+    """
+
     def __init__(
         self,
         *,
         impact: pd.Series,
         households_impact: Impact | None = None,
         name: str | None = "Unnamed",
         occurrence: int = 1,
@@ -1157,19 +1297,19 @@
                     if ri not in self._aff_regions_idx
                     for si in self._rebuilding_sectors_idx
                 ]
             )
             self._rebuilding_sectors_shares[self._rebuilding_industries_idx] = np.tile(
                 np.array(reb_sectors.values), np.size(self.aff_regions)
             )
-            self._rebuilding_sectors_shares[
-                self._rebuilding_industries_RoW_idx
-            ] = np.tile(
-                np.array(reb_sectors.values),
-                (np.size(self.possible_regions) - np.size(self.aff_regions)),
+            self._rebuilding_sectors_shares[self._rebuilding_industries_RoW_idx] = (
+                np.tile(
+                    np.array(reb_sectors.values),
+                    (np.size(self.possible_regions) - np.size(self.aff_regions)),
+                )
             )
 
     @property
     def rebuilding_demand_house(self) -> npt.NDArray:
         r"""The optional array of rebuilding demand from households"""
         return self._rebuilding_demand_house
 
@@ -1224,14 +1364,25 @@
                     self.total_productive_capital_destroyed,
                 )
             )
         self._rebuildable = reb
 
 
 class EventKapitalRecover(EventKapitalDestroyed):
+    r"""EventKapitalRecover holds a :py:class:`EventKapitalDestroyed` event where the destroyed capital does not create a reconstruction demand.
+
+    This subclass requires and enables new arguments to pass to the constructor:
+
+    * A characteristic time for the recovery (``recovery_time``)
+    * Optionally a ``recovery_function`` (linear by default).
+
+    .. seealso::
+       Tutorial :ref:`boario-events`
+    """
+
     def __init__(
         self,
         *,
         impact: pd.Series,
         recovery_time: int,
         recovery_function: str = "linear",
         households_impact: Optional[Impact] = None,
```

### Comparing `boario-0.5.7/boario/extended_models.py` & `boario-0.5.8/boario/extended_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,17 +48,18 @@
         productive_capital_vector: Optional[
             pd.Series | np.ndarray | pd.DataFrame
         ] = None,
         productive_capital_to_VA_dict: Optional[dict] = None,
         psi_param=0.80,
         inventory_restoration_tau: int | Dict[str, int] = 60,
     ) -> None:
-        """An ARIO3 model with some additional features
+        """An ARIO model with some additional features.
 
         Added feature are parameter psi of production adjustment inventories constraint threshold, as well as a characteristic time of inventories resupplying.
+        See :ref:`model_type`.
         """
 
         super().__init__(
             pym_mrio,
             order_type=order_type,
             alpha_base=alpha_base,
             alpha_max=alpha_max,
```

### Comparing `boario-0.5.7/boario/model_base.py` & `boario-0.5.8/boario/model_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+"""This module defines the core mechanisms of the model."""
+
 from __future__ import annotations
 
 import json
 import pathlib
 import typing
 from typing import Optional
 
@@ -1130,17 +1132,17 @@
 """
 
         if scheme != "proportional":
             raise ValueError(f"Scheme {scheme} is currently not implemented")
 
         # list_of_demands = [self.matrix_orders, self.final_demand]
         # # 1. Calc demand from rebuilding requirements (with characteristic time rebuild_tau)
-        house_reb_dem_per_event = (
-            house_reb_dem_tot_per_event
-        ) = indus_reb_dem_per_event = indus_reb_dem_tot_per_event = None
+        house_reb_dem_per_event = house_reb_dem_tot_per_event = (
+            indus_reb_dem_per_event
+        ) = indus_reb_dem_tot_per_event = None
 
         if rebuildable_events:
             logger.debug("There are rebuildable events")
             n_events = len(rebuildable_events)
             tot_rebuilding_demand_summed = self.tot_rebuild_demand.copy()
             # debugging assert
             if not tot_rebuilding_demand_summed.shape == self.X_0.shape:
```

### Comparing `boario-0.5.7/boario/simulation.py` & `boario-0.5.8/boario/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -620,17 +620,17 @@
 
         if (
             self.model.tot_rebuild_demand is None
             or not self.model.tot_rebuild_demand.any()
         ):
             self.equi[(n_checks, self.current_temporal_unit, "rebuilding")] = "finished"
         else:
-            self.equi[
-                (n_checks, self.current_temporal_unit, "rebuilding")
-            ] = "not finished"
+            self.equi[(n_checks, self.current_temporal_unit, "rebuilding")] = (
+                "not finished"
+            )
 
     def add_events(self, events: list[Event]):
         """Add a list of events to the simulation.
 
         Parameters
         ----------
         events : list[Event]
@@ -727,41 +727,41 @@
         self._production_evolution[self.current_temporal_unit] = self.model.production
 
     def _write_rebuild_prod(self) -> None:
         """Saves the current rebuilding production vector to the memmap."""
         logger.debug(
             f"self._rebuild_production_evolution shape : {self._rebuild_production_evolution.shape}, self.model.rebuild_prod shape : {self.model.rebuild_prod.shape}"
         )
-        self._rebuild_production_evolution[
-            self.current_temporal_unit
-        ] = self.model.rebuild_prod
+        self._rebuild_production_evolution[self.current_temporal_unit] = (
+            self.model.rebuild_prod
+        )
 
     def _write_productive_capital_lost(self) -> None:
         """Saves the current remaining productive_capital to rebuild vector to the memmap."""
         self._regional_sectoral_productive_capital_destroyed_evolution[
             self.current_temporal_unit
         ] = self.model.productive_capital_lost
 
     def _write_production_max(self) -> None:
         """Saves the current production capacity vector to the memmap."""
-        self._production_cap_evolution[
-            self.current_temporal_unit
-        ] = self.model.production_cap
+        self._production_cap_evolution[self.current_temporal_unit] = (
+            self.model.production_cap
+        )
 
     def _write_io_demand(self) -> None:
         """Saves the current (total per industry) intermediate demand vector to the memmap."""
-        self._io_demand_evolution[
-            self.current_temporal_unit
-        ] = self.model.matrix_orders.sum(axis=1)
+        self._io_demand_evolution[self.current_temporal_unit] = (
+            self.model.matrix_orders.sum(axis=1)
+        )
 
     def _write_final_demand(self) -> None:
         """Saves the current (total per industry) final demand vector to the memmap."""
-        self._final_demand_evolution[
-            self.current_temporal_unit
-        ] = self.model.final_demand.sum(axis=1)
+        self._final_demand_evolution[self.current_temporal_unit] = (
+            self.model.final_demand.sum(axis=1)
+        )
 
     def _write_rebuild_demand(self) -> None:
         """Saves the current (total per industry) rebuilding demand vector to the memmap."""
         to_write = np.full(self.model.n_regions * self.model.n_sectors, 0.0)
         if len(r_dem := self.model.tot_rebuild_demand) > 0:
             self._rebuild_demand_evolution[self.current_temporal_unit] = r_dem  # type: ignore
         else:
@@ -769,17 +769,17 @@
 
     def _write_overproduction(self) -> None:
         """Saves the current overproduction vector to the memmap."""
         self._overproduction_evolution[self.current_temporal_unit] = self.model.overprod
 
     def _write_final_demand_unmet(self) -> None:
         """Saves the unmet final demand (for this step) vector to the memmap."""
-        self._final_demand_unmet_evolution[
-            self.current_temporal_unit
-        ] = self.model.final_demand_not_met
+        self._final_demand_unmet_evolution[self.current_temporal_unit] = (
+            self.model.final_demand_not_met
+        )
 
     def _write_stocks(self) -> None:
         """Saves the current inputs stock matrix to the memmap."""
         self._inputs_evolution[self.current_temporal_unit] = self.model.matrix_stock
 
     def _write_limiting_stocks(self, limiting_stock: np.ndarray) -> None:
         """Saves the current limiting inputs matrix to the memmap."""
```

### Comparing `boario-0.5.7/boario/utils/misc.py` & `boario-0.5.8/boario/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         else:
             yield el
 
 
 def lexico_reindex(mrio: pymrio.IOSystem) -> pymrio.IOSystem:
     """Reindex IOSystem lexicographicaly
 
-    Sort indexes and columns of the dataframe of a ``pymrio`` `IOSystem <https://pymrio.readthedocs.io/en/latest/intro.html>` by
+    Sort indexes and columns of the dataframe of a ``pymrio.IOSystem`` by
     lexical order.
 
     Parameters
     ----------
     mrio : pymrio.IOSystem
         The IOSystem to sort
```

### Comparing `boario-0.5.7/boario/utils/recovery_functions.py` & `boario-0.5.8/boario/utils/recovery_functions.py`

 * *Files identical despite different names*

### Comparing `boario-0.5.7/pyproject.toml` & `boario-0.5.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "boario"
-version = "0.5.7"
+version = "0.5.8"
 description = "BoARIO : The Adaptative Regional Input Output model in python."
 authors = ["Samuel Juhel <pro@sjuhel.org>"]
 license = "GNU General Public License v3 or later (GPLv3+)"
 readme = "README.rst"
 
 [tool.poetry.dependencies]
-python=">=3.9"
+python=">=3.9,<4.0"
 coloredlogs = "^15.0.1"
 country-converter = "^1.0.0"
 dask = ">=2023"
 numpy = "<1.24"
 odfpy = "^1.4.1"
 pandas = ">=1.5"
 progressbar2 = "^4.2.0"
@@ -19,26 +19,30 @@
 pymrio = ">=0.4"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pygit2 = "^1.12.1"
 ipykernel = "^6.23.0"
-black = "^23.3.0"
+black = ">=23.3,<25.0"
 sphinxcontrib-bibtex = "^2.5.0"
-sphinx-autoapi = "^2.1.0"
+sphinx-autoapi = ">=2.1,<4.0"
 sphinx-automodapi = "^0.15.0"
 sphinx-copybutton = "^0.5.2"
-pydata-sphinx-theme = "^0.13.3"
+pydata-sphinx-theme = ">=0.13.3,<0.16.0"
 nbsphinx = "^0.9.2"
 pytest-cov = "^4.1.0"
 isort = "^5.13.2"
 flake8 = "^7.0.0"
 flake8-pyproject = "^1.2.3"
 safety = "^3.0.1"
+pydoclint = "^0.4.1"
+autoapi = "^2.0.1"
+sphinx-autodoc-typehints = "^2.0.0"
+numpydoc = "^1.7.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project]
 keywords = [
```

### Comparing `boario-0.5.7/PKG-INFO` & `boario-0.5.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: boario
-Version: 0.5.7
+Version: 0.5.8
 Summary: BoARIO : The Adaptative Regional Input Output model in python.
 License: GNU General Public License v3 or later (GPLv3+)
 Author: Samuel Juhel
 Author-email: pro@sjuhel.org
-Requires-Python: >=3.9
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
@@ -25,41 +25,35 @@
 
 .. role:: pythoncode(code)
    :language: python
 
 #######
 BoARIO
 #######
+|build-status| |black| |contribute| |licence| |pypi| |pythonv| |joss|
 
-
-.. image:: https://img.shields.io/github/actions/workflow/status/spjuhel/boario/CI.yml
+.. |build-status| image:: https://img.shields.io/github/actions/workflow/status/spjuhel/boario/CI.yml
    :target: https://github.com/spjuhel/BoARIO/actions/workflows/CI.yml
    :alt: GitHub Actions Workflow Status
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000
    :target: https://github.com/psf/black
    :alt: Code Style - Black
-
-.. image:: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
+.. |contribute| image:: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
    :target: https://github.com/spjuhel/BoARIO/issues
    :alt: Contribution - Welcome
-
-.. image:: https://img.shields.io/badge/License-GPLv3-blue
+.. |licence| image:: https://img.shields.io/badge/License-GPLv3-blue
    :target: https://www.gnu.org/licenses/gpl-3.0
    :alt: Licence - GPLv3
-
-.. image:: https://img.shields.io/pypi/v/boario
+.. |pypi| image:: https://img.shields.io/pypi/v/boario
    :target: https://pypi.org/project/boario/
    :alt: PyPI - Version
-
-.. image:: https://img.shields.io/pypi/pyversions/boario
+.. |pythonv| image:: https://img.shields.io/pypi/pyversions/boario
    :target: https://pypi.org/project/boario/
    :alt: PyPI - Python Version
-
-.. image:: https://joss.theoj.org/papers/71386aa01a292ecff8bafe273b077701/status.svg
+.. |joss| image:: https://joss.theoj.org/papers/71386aa01a292ecff8bafe273b077701/status.svg
    :target: https://joss.theoj.org/papers/71386aa01a292ecff8bafe273b077701
    :alt: Joss Status
 
 `BoARIO` : The Adaptative Regional Input Output model in python.
 
 .. _`Documentation Website`: https://spjuhel.github.io/BoARIO/boario-what-is.html
 
@@ -109,14 +103,20 @@
 
 You can install BoARIO from ``pip`` with:
 
 .. code:: console
 
    pip install boario
 
+Or from ``conda-forge`` using conda (or mamba):
+
+.. code:: console
+
+   conda install -c conda-forge boario
+
 
 The full source code is also available on Github at: https://github.com/spjuhel/BoARIO
 
 More info in the `installation <https://spjuhel.github.io/BoARIO/boario-installation.html>`_ page of the documentation.
 
 How does BoARIO work?
 =========================
@@ -134,15 +134,15 @@
 - the step by step, sector by sector, region by region evolution of most of the variables involved in the simulation (`production`, `demand`, `stocks`, ...)
 
 - aggregated indicators for the whole simulation (`shortages duration`, `aggregated impacts`, ...)
 
 Example of use
 =================
 
-See `Boario quickstart <https://spjuhel.github.io/BoARIO/boario-quickstart.html>`_.
+See `Boario quickstart <https://spjuhel.github.io/BoARIO/boario-tutorials.html>`_.
 
 Credits
 ========
 
 Associated PhD project
 ------------------------
 
@@ -155,15 +155,15 @@
            :alt: ADEME Logo
 
 .. _`ADEME`: https://www.ademe.fr/
 
 Development
 ------------
 
-* Samuel Juhel (pro@sjuhel.org)
+** Samuel Juhel (pro@sjuhel.org)
 
 Contributions
 ---------------
 
 All `contributions <https://spjuhel.github.io/BoARIO/development.html>`_ to the project are welcome !
 
 Acknowledgements
```

