# Comparing `tmp/hyperx-2024.1.9-py3-none-any.whl.zip` & `tmp/hyperx-2024.1.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 47634 bytes, number of entries: 12
+Zip file size: 50818 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      742 b- defN 24-Jan-17 19:54 hyperx/__init__.py
--rw-rw-rw-  2.0 fat   292632 b- defN 24-Mar-28 17:41 hyperx/api/__init__.py
--rw-rw-rw-  2.0 fat    32628 b- defN 24-Mar-28 17:41 hyperx/api/types/__init__.py
+-rw-rw-rw-  2.0 fat   314452 b- defN 24-May-13 16:19 hyperx/api/__init__.py
+-rw-rw-rw-  2.0 fat    32831 b- defN 24-May-13 16:19 hyperx/api/types/__init__.py
 -rw-rw-rw-  2.0 fat      125 b- defN 23-Oct-16 20:54 hyperx/library/__init__.py
 -rw-rw-rw-  2.0 fat     1621 b- defN 24-Jan-17 19:54 hyperx/library/find.py
 -rw-rw-rw-  2.0 fat     1502 b- defN 24-Jan-17 19:54 hyperx/library/library.py
 -rw-rw-rw-  2.0 fat       71 b- defN 23-Oct-16 20:54 hyperx/utils/__init__.py
--rw-rw-rw-  2.0 fat     2787 b- defN 23-Oct-16 20:54 hyperx/utils/utils.py
--rw-rw-rw-  2.0 fat      629 b- defN 24-Mar-28 17:45 hyperx-2024.1.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-28 17:45 hyperx-2024.1.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-Mar-28 17:45 hyperx-2024.1.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      945 b- defN 24-Mar-28 17:45 hyperx-2024.1.9.dist-info/RECORD
-12 files, 333781 bytes uncompressed, 46056 bytes compressed:  86.2%
+-rw-rw-rw-  2.0 fat     2823 b- defN 24-May-13 16:19 hyperx/utils/utils.py
+-rw-rw-rw-  2.0 fat      630 b- defN 24-May-13 16:33 hyperx-2024.1.9.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-13 16:33 hyperx-2024.1.9.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-13 16:33 hyperx-2024.1.9.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      953 b- defN 24-May-13 16:33 hyperx-2024.1.9.1.dist-info/RECORD
+12 files, 355849 bytes uncompressed, 49224 bytes compressed:  86.2%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: hyperx/utils/__init__.py
 Comment: 
 
 Filename: hyperx/utils/utils.py
 Comment: 
 
-Filename: hyperx-2024.1.9.dist-info/METADATA
+Filename: hyperx-2024.1.9.1.dist-info/METADATA
 Comment: 
 
-Filename: hyperx-2024.1.9.dist-info/WHEEL
+Filename: hyperx-2024.1.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: hyperx-2024.1.9.dist-info/top_level.txt
+Filename: hyperx-2024.1.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: hyperx-2024.1.9.dist-info/RECORD
+Filename: hyperx-2024.1.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hyperx/api/__init__.py

```diff
@@ -2,15 +2,15 @@
 from ..library import _api, _types
 
 from ..api import types
 from typing import TypeVar, Generic, overload
 from enum import Enum
 from System.Collections.Generic import List, IEnumerable, Dictionary, HashSet
 from System.Threading.Tasks import Task
-from System import Guid, DateTime, Action
+from System import Guid, DateTime, Action, Double, String, Nullable
 
 from abc import ABC, abstractmethod
 
 T = TypeVar('T')
 
 def MakeCSharpIntList(ints: list[int]) -> List[int]:
 	intsList = List[int]()
@@ -226,30 +226,32 @@
 
 	@property
 	def IsInformationalCode(self) -> bool:
 		return self._Entity.IsInformationalCode
 
 	@property
 	def MarginCode(self) -> types.MarginCode:
-		return types.MarginCode[self._Entity.MarginCode.ToString()]
+		result = self._Entity.MarginCode
+		return types.MarginCode[result.ToString()] if result is not None else None
 
 
 class AnalysisResult(ABC):
 	'''
 	Contains result information for an analysis
 	'''
 	def __init__(self, analysisResult: _api.AnalysisResult):
 		self._Entity = analysisResult
 
 	@property
 	def LimitUltimate(self) -> types.LimitUltimate:
 		'''
 		Limit vs Ultimate loads.
 		'''
-		return types.LimitUltimate[self._Entity.LimitUltimate.ToString()]
+		result = self._Entity.LimitUltimate
+		return types.LimitUltimate[result.ToString()] if result is not None else None
 
 	@property
 	def LoadCaseId(self) -> int:
 		return self._Entity.LoadCaseId
 
 	@property
 	def Margin(self) -> Margin:
@@ -270,67 +272,73 @@
 		self._Entity = jointAnalysisResult
 
 	@property
 	def ObjectId(self) -> types.JointObject:
 		'''
 		Enum identifying the possible entities within a joint
 		'''
-		return types.JointObject[self._Entity.ObjectId.ToString()]
+		result = self._Entity.ObjectId
+		return types.JointObject[result.ToString()] if result is not None else None
 
 
 class ZoneAnalysisConceptResult(AnalysisResult):
 	def __init__(self, zoneAnalysisConceptResult: _api.ZoneAnalysisConceptResult):
 		self._Entity = zoneAnalysisConceptResult
 
 	@property
 	def ConceptId(self) -> types.FamilyConceptUID:
-		return types.FamilyConceptUID[self._Entity.ConceptId.ToString()]
+		result = self._Entity.ConceptId
+		return types.FamilyConceptUID[result.ToString()] if result is not None else None
 
 
 class ZoneAnalysisObjectResult(AnalysisResult):
 	def __init__(self, zoneAnalysisObjectResult: _api.ZoneAnalysisObjectResult):
 		self._Entity = zoneAnalysisObjectResult
 
 	@property
 	def ObjectId(self) -> types.FamilyObjectUID:
-		return types.FamilyObjectUID[self._Entity.ObjectId.ToString()]
+		result = self._Entity.ObjectId
+		return types.FamilyObjectUID[result.ToString()] if result is not None else None
 
 
 class AssignableProperty(IdNameEntity):
 	def __init__(self, assignableProperty: _api.AssignableProperty):
 		self._Entity = assignableProperty
 
 
 class AssignablePropertyWithFamilyCategory(AssignableProperty):
 	def __init__(self, assignablePropertyWithFamilyCategory: _api.AssignablePropertyWithFamilyCategory):
 		self._Entity = assignablePropertyWithFamilyCategory
 
 	@property
 	def FamilyCategory(self) -> types.FamilyCategory:
-		return types.FamilyCategory[self._Entity.FamilyCategory.ToString()]
+		result = self._Entity.FamilyCategory
+		return types.FamilyCategory[result.ToString()] if result is not None else None
 
 
 class FailureObjectGroup(IdNameEntity):
 	def __init__(self, failureObjectGroup: _api.FailureObjectGroup):
 		self._Entity = failureObjectGroup
 
 	@property
 	def ObjectGroup(self) -> types.ObjectGroup:
-		return types.ObjectGroup[self._Entity.ObjectGroup.ToString()]
+		result = self._Entity.ObjectGroup
+		return types.ObjectGroup[result.ToString()] if result is not None else None
 
 	@property
 	def IsEnabled(self) -> bool:
 		return self._Entity.IsEnabled
 
 	@property
 	def LimitUltimate(self) -> types.LimitUltimate:
 		'''
 		Limit vs Ultimate loads.
 		'''
-		return types.LimitUltimate[self._Entity.LimitUltimate.ToString()]
+		result = self._Entity.LimitUltimate
+		return types.LimitUltimate[result.ToString()] if result is not None else None
 
 	@property
 	def RequiredMargin(self) -> float:
 		return self._Entity.RequiredMargin
 
 	@IsEnabled.setter
 	def IsEnabled(self, value: bool) -> None:
@@ -354,15 +362,16 @@
 
 	@property
 	def CategoryId(self) -> int:
 		return self._Entity.CategoryId
 
 	@property
 	def DataType(self) -> types.UserConstantDataType:
-		return types.UserConstantDataType[self._Entity.DataType.ToString()]
+		result = self._Entity.DataType
+		return types.UserConstantDataType[result.ToString()] if result is not None else None
 
 	@property
 	def DefaultValue(self) -> str:
 		return self._Entity.DefaultValue
 
 	@property
 	def Description(self) -> str:
@@ -401,14 +410,17 @@
 	def SetFloatValue(self, value: float) -> None:
 		return self._Entity.SetFloatValue(value)
 
 	def SetBoolValue(self, value: bool) -> None:
 		return self._Entity.SetBoolValue(value)
 
 	def SetSelectionValue(self, index: int) -> None:
+		'''
+		Set enum value by index.
+		'''
 		return self._Entity.SetSelectionValue(index)
 
 
 class IdEntityCol(Generic[T], ABC):
 	def __init__(self, idEntityCol: _api.IdEntityCol):
 		self._Entity = idEntityCol
 
@@ -544,26 +556,38 @@
 	def Get(self, name: str) -> FailureSetting: ...
 
 	@overload
 	def Get(self, id: int) -> FailureSetting: ...
 
 	def Get(self, item1 = None) -> FailureSetting:
 		if isinstance(item1, str):
-			return FailureSetting(super().Get(item1))
+			result = super().Get(item1)
+			thisClass = type(result).__name__
+			givenClass = FailureSetting
+			for subclass in FailureSetting.__subclasses__():
+				if subclass.__name__ == thisClass:
+					givenClass = subclass
+			return givenClass(result) if result is not None else None
 
 		if isinstance(item1, int):
-			return FailureSetting(super().Get(item1))
+			result = super().Get(item1)
+			thisClass = type(result).__name__
+			givenClass = FailureSetting
+			for subclass in FailureSetting.__subclasses__():
+				if subclass.__name__ == thisClass:
+					givenClass = subclass
+			return givenClass(result) if result is not None else None
 
 		result = self._Entity.Get(item1)
 		thisClass = type(result).__name__
 		givenClass = FailureSetting
 		for subclass in FailureSetting.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		return givenClass(result)
+		return givenClass(result) if result is not None else None
 
 	def __getitem__(self, index: int):
 		return self.FailureSettingColList[index]
 
 	def __iter__(self):
 		yield from self.FailureSettingColList
 
@@ -581,15 +605,16 @@
 
 	@property
 	def IsEnabled(self) -> bool:
 		return self._Entity.IsEnabled
 
 	@property
 	def LimitUltimate(self) -> types.LimitUltimate:
-		return types.LimitUltimate[self._Entity.LimitUltimate.ToString()]
+		result = self._Entity.LimitUltimate
+		return types.LimitUltimate[result.ToString()] if result is not None else None
 
 	@property
 	def ObjectGroups(self) -> FailureObjectGroupCol:
 		result = self._Entity.ObjectGroups
 		return FailureObjectGroupCol(result) if result is not None else None
 
 	@property
@@ -773,34 +798,39 @@
 
 
 class DesignProperty(AssignablePropertyWithFamilyCategory):
 	def __init__(self, designProperty: _api.DesignProperty):
 		self._Entity = designProperty
 
 	def Copy(self, newName: str = None) -> DesignProperty:
+		'''
+		Creates a copy of this DesignProperty.
+		'''
 		result = self._Entity.Copy(newName)
 		thisClass = type(result).__name__
 		givenClass = DesignProperty
 		for subclass in DesignProperty.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		return givenClass(result)
+		return givenClass(result) if result is not None else None
 
 
 class LoadProperty(AssignableProperty):
 	def __init__(self, loadProperty: _api.LoadProperty):
 		self._Entity = loadProperty
 
 	@property
 	def Category(self) -> types.FamilyCategory:
-		return types.FamilyCategory[self._Entity.Category.ToString()]
+		result = self._Entity.Category
+		return types.FamilyCategory[result.ToString()] if result is not None else None
 
 	@property
 	def Type(self) -> types.LoadPropertyType:
-		return types.LoadPropertyType[self._Entity.Type.ToString()]
+		result = self._Entity.Type
+		return types.LoadPropertyType[result.ToString()] if result is not None else None
 
 	@property
 	def IsZeroCurvature(self) -> bool:
 		return self._Entity.IsZeroCurvature
 
 	@property
 	def ModificationDate(self) -> DateTime:
@@ -857,15 +887,16 @@
 
 	@property
 	def RunDeckOrder(self) -> int:
 		return self._Entity.RunDeckOrder
 
 	@property
 	def SolutionType(self) -> types.FeaSolutionType:
-		return types.FeaSolutionType[self._Entity.SolutionType.ToString()]
+		result = self._Entity.SolutionType
+		return types.FeaSolutionType[result.ToString()] if result is not None else None
 
 
 class DesignLoadSubcaseMultiplier(IdNameEntity):
 	def __init__(self, designLoadSubcaseMultiplier: _api.DesignLoadSubcaseMultiplier):
 		self._Entity = designLoadSubcaseMultiplier
 
 	@property
@@ -900,15 +931,16 @@
 		return DesignLoadSubcase(result) if result is not None else None
 
 	@property
 	def TemperatureChoiceType(self) -> types.TemperatureChoiceType:
 		'''
 		Load Case Setting selection for analysis and initial temperature.
 		'''
-		return types.TemperatureChoiceType[self._Entity.TemperatureChoiceType.ToString()]
+		result = self._Entity.TemperatureChoiceType
+		return types.TemperatureChoiceType[result.ToString()] if result is not None else None
 
 	@property
 	def Value(self) -> float:
 		return self._Entity.Value
 
 
 class DesignLoadSubcaseMultiplierCol(IdNameEntityCol[DesignLoadSubcaseMultiplier]):
@@ -1000,27 +1032,29 @@
 
 class ZoneDesignResult(IdEntity):
 	def __init__(self, zoneDesignResult: _api.ZoneDesignResult):
 		self._Entity = zoneDesignResult
 
 	@property
 	def VariableParameter(self) -> types.VariableParameter:
-		return types.VariableParameter[self._Entity.VariableParameter.ToString()]
+		result = self._Entity.VariableParameter
+		return types.VariableParameter[result.ToString()] if result is not None else None
 
 	@property
 	def Value(self) -> float:
 		return self._Entity.Value
 
 	@property
 	def MaterialId(self) -> int:
 		return self._Entity.MaterialId
 
 	@property
 	def MaterialType(self) -> types.MaterialType:
-		return types.MaterialType[self._Entity.MaterialType.ToString()]
+		result = self._Entity.MaterialType
+		return types.MaterialType[result.ToString()] if result is not None else None
 
 
 class Vector3d:
 	'''
 	Represents a readonly 3D vector.
 	'''
 	def __init__(self, vector3d: _api.Vector3d):
@@ -1041,31 +1075,34 @@
 	def Z(self) -> float:
 		return self._Entity.Z
 
 	@overload
 	def Equals(self, other) -> bool: ...
 
 	@overload
-	def Equals(self, obj) -> bool: ...
-
-	def GetHashCode(self) -> int:
-		return self._Entity.GetHashCode()
+	def Equals(self, obj: object) -> bool: ...
 
 	def Equals(self, item1 = None) -> bool:
 		if isinstance(item1, Vector3d):
 			return self._Entity.Equals(item1._Entity)
 
+		if isinstance(item1, object):
+			return self._Entity.Equals(item1)
+
 		return self._Entity.Equals(item1._Entity)
 
 	def __eq__(self, other):
 		return self.Equals(other)
 
 	def __ne__(self, other):
 		return not self.Equals(other)
 
+	def __hash__(self) -> int:
+		return self._Entity.GetHashCode()
+
 
 class DiscreteField(IdNameEntityRenameable):
 	'''
 	Represents a table of discrete field data.
 	'''
 	def __init__(self, discreteField: _api.DiscreteField):
 		self._Entity = discreteField
@@ -1083,39 +1120,47 @@
 		return self._Entity.ColumnCount
 
 	@property
 	def DataType(self) -> types.DiscreteFieldDataType:
 		'''
 		Defines the type of data stored in a Discrete Field. Such as Vector, Scalar, String.
 		'''
-		return types.DiscreteFieldDataType[self._Entity.DataType.ToString()]
+		result = self._Entity.DataType
+		return types.DiscreteFieldDataType[result.ToString()] if result is not None else None
 
 	@property
 	def PhysicalEntityType(self) -> types.DiscreteFieldPhysicalEntityType:
 		'''
 		Defines the type of physical entity that a Discrete Field applies to, such as zone, element, joint, etc.
 		'''
-		return types.DiscreteFieldPhysicalEntityType[self._Entity.PhysicalEntityType.ToString()]
+		result = self._Entity.PhysicalEntityType
+		return types.DiscreteFieldPhysicalEntityType[result.ToString()] if result is not None else None
 
 	@property
 	def PointIds(self) -> list[Vector3d]:
 		return [Vector3d(vector3d) for vector3d in self._Entity.PointIds]
 
 	@property
 	def RowCount(self) -> int:
 		return self._Entity.RowCount
 
 	@property
 	def RowIds(self) -> list[int]:
 		return [int32 for int32 in self._Entity.RowIds]
 
 	def AddColumn(self, name: str) -> int:
+		'''
+		Create a new column with the given name. Returns the Id of the newly created column
+		'''
 		return self._Entity.AddColumn(name)
 
 	def AddPointRow(self, pointId: Vector3d) -> None:
+		'''
+		Create an empty row in a point-based table.
+		'''
 		return self._Entity.AddPointRow(pointId._Entity)
 
 	@overload
 	def ReadNumericCell(self, entityId: int, columnId: int) -> float: ...
 
 	@overload
 	def ReadNumericCell(self, pointId: Vector3d, columnId: int) -> float: ...
@@ -1144,51 +1189,60 @@
 	def DeleteAllRows(self) -> None:
 		'''
 		Delete all rows for this discrete field.
 		'''
 		return self._Entity.DeleteAllRows()
 
 	def DeleteColumn(self, columnId: int) -> None:
+		'''
+		Delete a specified column for this discrete field. Columns are 1-indexed.
+		'''
 		return self._Entity.DeleteColumn(columnId)
 
 	def DeletePointRow(self, pointId: Vector3d) -> None:
+		'''
+		Delete a specific row for a point-based table.
+		'''
 		return self._Entity.DeletePointRow(pointId._Entity)
 
 	def DeleteRow(self, entityId: int) -> None:
+		'''
+		Delete a specific row for a non-point-based table.
+		'''
 		return self._Entity.DeleteRow(entityId)
 
 	def DeleteRowsAndColumns(self) -> None:
 		'''
 		Delete all rows and columns for this discrete field.
 		'''
 		return self._Entity.DeleteRowsAndColumns()
 
 	def ReadNumericCell(self, item1 = None, item2 = None) -> float:
 		if isinstance(item1, int) and isinstance(item2, int):
-			return self._Entity.ReadNumericCell(item1, item2)
+			return float(self._Entity.ReadNumericCell(item1, item2))
 
 		if isinstance(item1, Vector3d) and isinstance(item2, int):
-			return self._Entity.ReadNumericCell(item1._Entity, item2)
+			return float(self._Entity.ReadNumericCell(item1._Entity, item2))
 
-		return self._Entity.ReadNumericCell(item1, item2)
+		return float(self._Entity.ReadNumericCell(item1, item2))
 
 	def ReadStringCell(self, item1 = None, item2 = None) -> str:
 		if isinstance(item1, int) and isinstance(item2, int):
 			return self._Entity.ReadStringCell(item1, item2)
 
 		if isinstance(item1, Vector3d) and isinstance(item2, int):
 			return self._Entity.ReadStringCell(item1._Entity, item2)
 
 		return self._Entity.ReadStringCell(item1, item2)
 
 	def SetNumericValue(self, item1 = None, item2 = None, item3 = None) -> None:
-		if isinstance(item1, int) and isinstance(item2, int) and isinstance(item3, float):
+		if isinstance(item1, int) and isinstance(item2, int) and isinstance(item3, float) and (isinstance(item3, float) or isinstance(item3, int)):
 			return self._Entity.SetNumericValue(item1, item2, item3)
 
-		if isinstance(item1, Vector3d) and isinstance(item2, int) and isinstance(item3, float):
+		if isinstance(item1, Vector3d) and isinstance(item2, int) and isinstance(item3, float) and (isinstance(item3, float) or isinstance(item3, int)):
 			return self._Entity.SetNumericValue(item1._Entity, item2, item3)
 
 		return self._Entity.SetNumericValue(item1, item2, item3)
 
 	def SetStringValue(self, item1 = None, item2 = None, item3 = None) -> None:
 		if isinstance(item1, int) and isinstance(item2, int) and isinstance(item3, str):
 			return self._Entity.SetStringValue(item1, item2, item3)
@@ -1267,42 +1321,45 @@
 	@property
 	def AssignedAnalysisProperty(self) -> AnalysisProperty:
 		result = self._Entity.AssignedAnalysisProperty
 		return AnalysisProperty(result) if result is not None else None
 
 	@property
 	def AssignedDesignProperty(self) -> DesignProperty:
-		thisClass = type(self._Entity.AssignedDesignProperty).__name__
+		result = self._Entity.AssignedDesignProperty
+		thisClass = type(result).__name__
 		givenClass = DesignProperty
 		for subclass in DesignProperty.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		result = self._Entity.AssignedDesignProperty
 		return givenClass(result) if result is not None else None
 
 	@property
 	def AssignedLoadProperty(self) -> LoadProperty:
-		thisClass = type(self._Entity.AssignedLoadProperty).__name__
+		result = self._Entity.AssignedLoadProperty
+		thisClass = type(result).__name__
 		givenClass = LoadProperty
 		for subclass in LoadProperty.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		result = self._Entity.AssignedLoadProperty
 		return givenClass(result) if result is not None else None
 
 	def AssignAnalysisProperty(self, id: int) -> PropertyAssignmentStatus:
 		return PropertyAssignmentStatus[self._Entity.AssignAnalysisProperty(id).ToString()]
 
 	def AssignDesignProperty(self, id: int) -> PropertyAssignmentStatus:
 		return PropertyAssignmentStatus[self._Entity.AssignDesignProperty(id).ToString()]
 
 	def AssignLoadProperty(self, id: int) -> PropertyAssignmentStatus:
 		return PropertyAssignmentStatus[self._Entity.AssignLoadProperty(id).ToString()]
 
 	def AssignProperty(self, property: AssignableProperty) -> PropertyAssignmentStatus:
+		'''
+		Assign a Property to this entity.
+		'''
 		return PropertyAssignmentStatus[self._Entity.AssignProperty(property._Entity).ToString()]
 
 
 class AnalysisResultCol(Generic[T]):
 	def __init__(self, analysisResultCol: _api.AnalysisResultCol):
 		self._Entity = analysisResultCol
 
@@ -1345,15 +1402,15 @@
 	def GetControllingResult(self) -> AnalysisResult:
 		result = self._Entity.GetControllingResult()
 		thisClass = type(result).__name__
 		givenClass = AnalysisResult
 		for subclass in AnalysisResult.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		return givenClass(result)
+		return givenClass(result) if result is not None else None
 
 	@abstractmethod
 	def GetAllResults(self) -> AnalysisResultCol:
 		return AnalysisResultCol(self._Entity.GetAllResults())
 
 
 class JointDesignResultCol(IdEntityCol[JointDesignResult]):
@@ -1378,35 +1435,41 @@
 		if isinstance(item1, types.JointSelectionId):
 			result = self._Entity.Get(_types.JointSelectionId(item1.value))
 			thisClass = type(result).__name__
 			givenClass = JointDesignResult
 			for subclass in JointDesignResult.__subclasses__():
 				if subclass.__name__ == thisClass:
 					givenClass = subclass
-			return givenClass(result)
+			return givenClass(result) if result is not None else None
 
 		if isinstance(item1, types.JointRangeId):
 			result = self._Entity.Get(_types.JointRangeId(item1.value))
 			thisClass = type(result).__name__
 			givenClass = JointDesignResult
 			for subclass in JointDesignResult.__subclasses__():
 				if subclass.__name__ == thisClass:
 					givenClass = subclass
-			return givenClass(result)
+			return givenClass(result) if result is not None else None
 
 		if isinstance(item1, int):
-			return JointDesignResult(super().Get(item1))
+			result = super().Get(item1)
+			thisClass = type(result).__name__
+			givenClass = JointDesignResult
+			for subclass in JointDesignResult.__subclasses__():
+				if subclass.__name__ == thisClass:
+					givenClass = subclass
+			return givenClass(result) if result is not None else None
 
 		result = self._Entity.Get(_types.JointSelectionId(item1.value))
 		thisClass = type(result).__name__
 		givenClass = JointDesignResult
 		for subclass in JointDesignResult.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		return givenClass(result)
+		return givenClass(result) if result is not None else None
 
 	def __getitem__(self, index: int):
 		return self.JointDesignResultColList[index]
 
 	def __iter__(self):
 		yield from self.JointDesignResultColList
 
@@ -1434,15 +1497,15 @@
 	def GetControllingResult(self) -> AnalysisResult:
 		result = self._Entity.GetControllingResult()
 		thisClass = type(result).__name__
 		givenClass = AnalysisResult
 		for subclass in AnalysisResult.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		return givenClass(result)
+		return givenClass(result) if result is not None else None
 
 	def GetMinimumMargin(self) -> Margin:
 		return Margin(self._Entity.GetMinimumMargin())
 
 
 class ZoneDesignResultCol(IdEntityCol[ZoneDesignResult]):
 	def __init__(self, zoneDesignResultCol: _api.ZoneDesignResultCol):
@@ -1685,30 +1748,36 @@
 	def GetObjectName(self, objectId: types.FamilyObjectUID) -> str:
 		return self._Entity.GetObjectName(_types.FamilyObjectUID(objectId.value))
 
 	def GetConceptName(self) -> str:
 		return self._Entity.GetConceptName()
 
 	def GetZoneDesignResults(self, solutionId: int = 1) -> ZoneDesignResultCol:
+		'''
+		Returns a collection of Zone Design Results for a Solution Id (default 1)
+		'''
 		return ZoneDesignResultCol(self._Entity.GetZoneDesignResults(solutionId))
 
 	def RenumberZone(self, newId: int) -> ZoneIdUpdateStatus:
+		'''
+		Attempt to update a zone's ID.
+		'''
 		return ZoneIdUpdateStatus[self._Entity.RenumberZone(newId).ToString()]
 
 	def GetAllResults(self) -> AnalysisResultCol:
 		return AnalysisResultCol(self._Entity.GetAllResults())
 
 	def GetControllingResult(self) -> AnalysisResult:
 		result = self._Entity.GetControllingResult()
 		thisClass = type(result).__name__
 		givenClass = AnalysisResult
 		for subclass in AnalysisResult.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		return givenClass(result)
+		return givenClass(result) if result is not None else None
 
 	def GetMinimumMargin(self) -> Margin:
 		return Margin(self._Entity.GetMinimumMargin())
 
 
 class ElementCol(IdEntityCol[Element]):
 	def __init__(self, elementCol: _api.ElementCol):
@@ -1747,15 +1816,16 @@
 
 	@property
 	def Objects(self) -> tuple[types.DiscreteDefinitionType]:
 		return tuple([types.DiscreteDefinitionType[discreteDefinitionType.ToString()] for discreteDefinitionType in self._Entity.Objects])
 
 	@property
 	def DiscreteTechnique(self) -> types.DiscreteTechnique:
-		return types.DiscreteTechnique[self._Entity.DiscreteTechnique.ToString()]
+		result = self._Entity.DiscreteTechnique
+		return types.DiscreteTechnique[result.ToString()] if result is not None else None
 
 	@property
 	def LeftSkinZoneId(self) -> int:
 		return self._Entity.LeftSkinZoneId
 
 	@property
 	def RightSkinZoneId(self) -> int:
@@ -1913,26 +1983,38 @@
 	def Get(self, name: str) -> Zone: ...
 
 	@overload
 	def Get(self, id: int) -> Zone: ...
 
 	def Get(self, item1 = None) -> Zone:
 		if isinstance(item1, str):
-			return Zone(super().Get(item1))
+			result = super().Get(item1)
+			thisClass = type(result).__name__
+			givenClass = Zone
+			for subclass in Zone.__subclasses__():
+				if subclass.__name__ == thisClass:
+					givenClass = subclass
+			return givenClass(result) if result is not None else None
 
 		if isinstance(item1, int):
-			return Zone(super().Get(item1))
+			result = super().Get(item1)
+			thisClass = type(result).__name__
+			givenClass = Zone
+			for subclass in Zone.__subclasses__():
+				if subclass.__name__ == thisClass:
+					givenClass = subclass
+			return givenClass(result) if result is not None else None
 
 		result = self._Entity.Get(item1)
 		thisClass = type(result).__name__
 		givenClass = Zone
 		for subclass in Zone.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		return givenClass(result)
+		return givenClass(result) if result is not None else None
 
 	def __getitem__(self, index: int):
 		return self.ZoneColList[index]
 
 	def __iter__(self):
 		yield from self.ZoneColList
 
@@ -2152,15 +2234,16 @@
 
 class AutomatedConstraint(IdNameEntityRenameable):
 	def __init__(self, automatedConstraint: _api.AutomatedConstraint):
 		self._Entity = automatedConstraint
 
 	@property
 	def ConstraintType(self) -> types.StiffnessCriteriaType:
-		return types.StiffnessCriteriaType[self._Entity.ConstraintType.ToString()]
+		result = self._Entity.ConstraintType
+		return types.StiffnessCriteriaType[result.ToString()] if result is not None else None
 
 	@property
 	def Set(self) -> str:
 		return self._Entity.Set
 
 	@property
 	def DesignLoadCases(self) -> list[str]:
@@ -2215,15 +2298,16 @@
 
 	@property
 	def GridId(self) -> int:
 		return self._Entity.GridId
 
 	@property
 	def Orientation(self) -> types.DisplacementShapeType:
-		return types.DisplacementShapeType[self._Entity.Orientation.ToString()]
+		result = self._Entity.Orientation
+		return types.DisplacementShapeType[result.ToString()] if result is not None else None
 
 	@property
 	def HasVector(self) -> bool:
 		return self._Entity.HasVector
 
 	@property
 	def X(self) -> float:
@@ -2295,15 +2379,16 @@
 
 class ManualConstraint(IdNameEntityRenameable):
 	def __init__(self, manualConstraint: _api.ManualConstraint):
 		self._Entity = manualConstraint
 
 	@property
 	def ConstraintType(self) -> types.ConstraintType:
-		return types.ConstraintType[self._Entity.ConstraintType.ToString()]
+		result = self._Entity.ConstraintType
+		return types.ConstraintType[result.ToString()] if result is not None else None
 
 	@property
 	def Set(self) -> str:
 		return self._Entity.Set
 
 	@property
 	def Limit(self) -> float:
@@ -2434,15 +2519,16 @@
 
 class DisplacementManualConstraint(ManualConstraintWithDesignLoad):
 	def __init__(self, displacementManualConstraint: _api.DisplacementManualConstraint):
 		self._Entity = displacementManualConstraint
 
 	@property
 	def DOF(self) -> types.DegreeOfFreedom:
-		return types.DegreeOfFreedom[self._Entity.DOF.ToString()]
+		result = self._Entity.DOF
+		return types.DegreeOfFreedom[result.ToString()] if result is not None else None
 
 	@property
 	def Nodes(self) -> list[int]:
 		return [int32 for int32 in self._Entity.Nodes]
 
 	@property
 	def RefNodes(self) -> list[int]:
@@ -2599,26 +2685,38 @@
 		if isinstance(item1, str):
 			return DisplacementAutomatedConstraint(self._Entity.GetDisplacement(item1))
 
 		return DisplacementAutomatedConstraint(self._Entity.GetDisplacement(item1))
 
 	def Get(self, item1 = None) -> AutomatedConstraint:
 		if isinstance(item1, str):
-			return AutomatedConstraint(super().Get(item1))
+			result = super().Get(item1)
+			thisClass = type(result).__name__
+			givenClass = AutomatedConstraint
+			for subclass in AutomatedConstraint.__subclasses__():
+				if subclass.__name__ == thisClass:
+					givenClass = subclass
+			return givenClass(result) if result is not None else None
 
 		if isinstance(item1, int):
-			return AutomatedConstraint(super().Get(item1))
+			result = super().Get(item1)
+			thisClass = type(result).__name__
+			givenClass = AutomatedConstraint
+			for subclass in AutomatedConstraint.__subclasses__():
+				if subclass.__name__ == thisClass:
+					givenClass = subclass
+			return givenClass(result) if result is not None else None
 
 		result = self._Entity.Get(item1)
 		thisClass = type(result).__name__
 		givenClass = AutomatedConstraint
 		for subclass in AutomatedConstraint.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		return givenClass(result)
+		return givenClass(result) if result is not None else None
 
 	def __getitem__(self, index: int):
 		return self.AutomatedConstraintColList[index]
 
 	def __iter__(self):
 		yield from self.AutomatedConstraintColList
 
@@ -2656,20 +2754,29 @@
 	@overload
 	def GetStaticMoment(self, id: int) -> StaticMomentManualConstraint: ...
 
 	@overload
 	def GetStaticMoment(self, name: str) -> StaticMomentManualConstraint: ...
 
 	def AddFrequencyConstraint(self, setName: str, limit: float, name: str = None) -> FrequencyManualConstraint:
+		'''
+		Add a Manual Constraint of type Frequency.
+		'''
 		return FrequencyManualConstraint(self._Entity.AddFrequencyConstraint(setName, limit, name))
 
 	def AddBucklingConstraint(self, setName: str, limit: float, name: str = None) -> BucklingManualConstraint:
+		'''
+		Add a Manual Constraint of type Buckling.
+		'''
 		return BucklingManualConstraint(self._Entity.AddBucklingConstraint(setName, limit, name))
 
 	def AddStaticMomentManualConstraint(self, setName: str, limit: float, name: str = None) -> StaticMomentManualConstraint:
+		'''
+		Add a Manual Constraint of type Static Moment.
+		'''
 		return StaticMomentManualConstraint(self._Entity.AddStaticMomentManualConstraint(setName, limit, name))
 
 	def AddDisplacementConstraint(self, setName: str, gridIds: list[int], limit: float, name: str = None) -> DisplacementManualConstraint:
 		gridIdsList = MakeCSharpIntList(gridIds)
 		return DisplacementManualConstraint(self._Entity.AddDisplacementConstraint(setName, gridIdsList, limit, name))
 
 	@overload
@@ -2759,17 +2866,23 @@
 
 	@property
 	def AutomatedConstraints(self) -> AutomatedConstraintCol:
 		result = self._Entity.AutomatedConstraints
 		return AutomatedConstraintCol(result) if result is not None else None
 
 	def RunIterations(self, numberOfIterations: int, startWithSizing: bool) -> None:
+		'''
+		Run HyperFEA.
+		'''
 		return self._Entity.RunIterations(numberOfIterations, startWithSizing)
 
 	def SetupSolver(self, solverPath: str, arguments: str) -> types.SimpleStatus:
+		'''
+		Setup FEA solver.
+		'''
 		return types.SimpleStatus(self._Entity.SetupSolver(solverPath, arguments))
 
 	def TestSolver(self) -> types.SimpleStatus:
 		'''
 		Test FEA solver setup.
 		'''
 		return types.SimpleStatus(self._Entity.TestSolver())
@@ -3004,17 +3117,24 @@
 	def Manufacturer(self, value: str) -> None:
 		self._Entity.Manufacturer = value
 
 	def AddTemperatureProperty(self, temperature: float, et: float, ec: float, g: float, ftu: float, fcu: float, fsu: float, ef: float = None, ffu: float = None, k: float = None, c: float = None) -> FoamTemperature:
 		return FoamTemperature(self._Entity.AddTemperatureProperty(temperature, et, ec, g, ftu, fcu, fsu, ef, ffu, k, c))
 
 	def DeleteTemperatureProperty(self, temperature: float) -> bool:
+		'''
+		Deletes a temperature-dependent property for a material.
+		'''
 		return self._Entity.DeleteTemperatureProperty(temperature)
 
 	def GetTemperature(self, lookupTemperature: float) -> FoamTemperature:
+		'''
+		Retrieve a Temperature from this material's temperature-dependent properties. Allows a degree of tolerance to avoid issues with floating point numbers.
+		:param LookupTemperature: Temperature to search for.
+		'''
 		return FoamTemperature(self._Entity.GetTemperature(lookupTemperature))
 
 	def Save(self) -> None:
 		'''
 		Save any changes to this foam material to the database.
 		'''
 		return self._Entity.Save()
@@ -3283,17 +3403,24 @@
 	def Manufacturer(self, value: str) -> None:
 		self._Entity.Manufacturer = value
 
 	def AddTemperatureProperty(self, temperature: float, et: float, ec: float, gw: float, gl: float, ftu: float, fcus: float, fcub: float, fcuc: float, fsuw: float, fsul: float, sScfl: float = None, sScfh: float = None, k1: float = None, k2: float = None, k3: float = None, c: float = None) -> HoneycombTemperature:
 		return HoneycombTemperature(self._Entity.AddTemperatureProperty(temperature, et, ec, gw, gl, ftu, fcus, fcub, fcuc, fsuw, fsul, sScfl, sScfh, k1, k2, k3, c))
 
 	def DeleteTemperatureProperty(self, temperature: float) -> bool:
+		'''
+		Deletes a temperature-dependent property for a material.
+		'''
 		return self._Entity.DeleteTemperatureProperty(temperature)
 
 	def GetTemperature(self, lookupTemperature: float) -> HoneycombTemperature:
+		'''
+		Retrieve a Temperature from this material's temperature-dependent properties. Allows a degree of tolerance to avoid issues with floating point numbers.
+		:param LookupTemperature: Temperature to search for.
+		'''
 		return HoneycombTemperature(self._Entity.GetTemperature(lookupTemperature))
 
 	def Save(self) -> None:
 		'''
 		Save any changes to this honeycomb material to the database.
 		'''
 		return self._Entity.Save()
@@ -3698,17 +3825,24 @@
 	def BucklingStiffnessKnockdown(self, value: float) -> None:
 		self._Entity.BucklingStiffnessKnockdown = value
 
 	def AddTemperatureProperty(self, temperature: float, et: float, ec: float, g: float, ftuL: float, ftyL: float, fcyL: float, ftuLT: float, ftyLT: float, fcyLT: float, fsu: float, alpha: float, n: float = None, f02: float = None, k: float = None, c: float = None, fbru15: float = None, fbry15: float = None, fbru20: float = None, fbry20: float = None, etyL: float = None, ecyL: float = None, etyLT: float = None, ecyLT: float = None, esu: float = None, fpadh: float = None, fsadh: float = None, esadh: float = None, cd: float = None, ffwt: float = None, ffxz: float = None, ffyz: float = None, ftFatigue: float = None, fcFatigue: float = None) -> IsotropicTemperature:
 		return IsotropicTemperature(self._Entity.AddTemperatureProperty(temperature, et, ec, g, ftuL, ftyL, fcyL, ftuLT, ftyLT, fcyLT, fsu, alpha, n, f02, k, c, fbru15, fbry15, fbru20, fbry20, etyL, ecyL, etyLT, ecyLT, esu, fpadh, fsadh, esadh, cd, ffwt, ffxz, ffyz, ftFatigue, fcFatigue))
 
 	def DeleteTemperatureProperty(self, temperature: float) -> bool:
+		'''
+		Deletes a temperature-dependent property for a material.
+		'''
 		return self._Entity.DeleteTemperatureProperty(temperature)
 
 	def GetTemperature(self, lookupTemperature: float) -> IsotropicTemperature:
+		'''
+		Retrieve a Temperature from this material's temperature-dependent properties. Allows a degree of tolerance to avoid issues with floating point numbers.
+		:param LookupTemperature: Temperature to search for.
+		'''
 		return IsotropicTemperature(self._Entity.GetTemperature(lookupTemperature))
 
 	def Save(self) -> None:
 		'''
 		Save any changes to this isotropic material to the database.
 		'''
 		return self._Entity.Save()
@@ -3784,79 +3918,86 @@
 
 	@property
 	def ModificationDate(self) -> DateTime:
 		return self._Entity.ModificationDate
 
 	@property
 	def PlankSetting(self) -> types.LaminateFamilySettingType:
-		return types.LaminateFamilySettingType[self._Entity.PlankSetting.ToString()]
+		result = self._Entity.PlankSetting
+		return types.LaminateFamilySettingType[result.ToString()] if result is not None else None
 
 	@property
 	def PlankMinRatio(self) -> float:
 		return self._Entity.PlankMinRatio
 
 	@property
 	def PlankMaxRatio(self) -> float:
 		return self._Entity.PlankMaxRatio
 
 	@property
 	def FootChargeSetting(self) -> types.LaminateFamilySettingType:
-		return types.LaminateFamilySettingType[self._Entity.FootChargeSetting.ToString()]
+		result = self._Entity.FootChargeSetting
+		return types.LaminateFamilySettingType[result.ToString()] if result is not None else None
 
 	@property
 	def FootChargeMinRatio(self) -> float:
 		return self._Entity.FootChargeMinRatio
 
 	@property
 	def FootChargeMaxRatio(self) -> float:
 		return self._Entity.FootChargeMaxRatio
 
 	@property
 	def WebChargeSetting(self) -> types.LaminateFamilySettingType:
-		return types.LaminateFamilySettingType[self._Entity.WebChargeSetting.ToString()]
+		result = self._Entity.WebChargeSetting
+		return types.LaminateFamilySettingType[result.ToString()] if result is not None else None
 
 	@property
 	def WebChargeMinRatio(self) -> float:
 		return self._Entity.WebChargeMinRatio
 
 	@property
 	def WebChargeMaxRatio(self) -> float:
 		return self._Entity.WebChargeMaxRatio
 
 	@property
 	def CapChargeSetting(self) -> types.LaminateFamilySettingType:
-		return types.LaminateFamilySettingType[self._Entity.CapChargeSetting.ToString()]
+		result = self._Entity.CapChargeSetting
+		return types.LaminateFamilySettingType[result.ToString()] if result is not None else None
 
 	@property
 	def CapChargeMinRatio(self) -> float:
 		return self._Entity.CapChargeMinRatio
 
 	@property
 	def CapChargeMaxRatio(self) -> float:
 		return self._Entity.CapChargeMaxRatio
 
 	@property
 	def CapCoverSetting(self) -> types.LaminateFamilySettingType:
-		return types.LaminateFamilySettingType[self._Entity.CapCoverSetting.ToString()]
+		result = self._Entity.CapCoverSetting
+		return types.LaminateFamilySettingType[result.ToString()] if result is not None else None
 
 	@property
 	def CapCoverMinRatio(self) -> float:
 		return self._Entity.CapCoverMinRatio
 
 	@property
 	def CapCoverMaxRatio(self) -> float:
 		return self._Entity.CapCoverMaxRatio
 
 	@property
 	def DropPattern(self) -> types.PlyDropPattern:
-		return types.PlyDropPattern[self._Entity.DropPattern.ToString()]
+		result = self._Entity.DropPattern
+		return types.PlyDropPattern[result.ToString()] if result is not None else None
 
 	@property
 	def LaminateStiffenerProfile(self) -> types.StiffenerProfile:
-		return types.StiffenerProfile[self._Entity.LaminateStiffenerProfile.ToString()]
+		result = self._Entity.LaminateStiffenerProfile
+		return types.StiffenerProfile[result.ToString()] if result is not None else None
 
 
 class LaminateLayerBase(ABC):
 	def __init__(self, laminateLayerBase: _api.LaminateLayerBase):
 		self._Entity = laminateLayerBase
 
 	@property
@@ -3868,15 +4009,16 @@
 		return self._Entity.LayerMaterial
 
 	@property
 	def LayerMaterialType(self) -> types.MaterialType:
 		'''
 		Represents a material's type.
 		'''
-		return types.MaterialType[self._Entity.LayerMaterialType.ToString()]
+		result = self._Entity.LayerMaterialType
+		return types.MaterialType[result.ToString()] if result is not None else None
 
 	@property
 	def Angle(self) -> float:
 		return self._Entity.Angle
 
 	@property
 	def Thickness(self) -> float:
@@ -3888,14 +4030,17 @@
 
 	@Angle.setter
 	@abstractmethod
 	def Angle(self, value: float) -> None:
 		self._Entity.Angle = value
 
 	def SetThickness(self, thickness: float) -> None:
+		'''
+		Set the thickness of a layer.
+		'''
 		return self._Entity.SetThickness(thickness)
 
 	@overload
 	def SetMaterial(self, matId: int) -> bool: ...
 
 	@overload
 	def SetMaterial(self, matName: str) -> bool: ...
@@ -3922,15 +4067,16 @@
 		return self._Entity.LayerId
 
 	@property
 	def LayerMaterialType(self) -> types.MaterialType:
 		'''
 		Represents a material's type.
 		'''
-		return types.MaterialType[self._Entity.LayerMaterialType.ToString()]
+		result = self._Entity.LayerMaterialType
+		return types.MaterialType[result.ToString()] if result is not None else None
 
 	@property
 	def Angle(self) -> float:
 		return self._Entity.Angle
 
 	@property
 	def Thickness(self) -> float:
@@ -3974,14 +4120,17 @@
 	def AddLayer(self, materialName: str, angle: float, thickness: float = None) -> LaminateLayer:
 		return LaminateLayer(self._Entity.AddLayer(materialName, angle, thickness))
 
 	def InsertLayer(self, layerId: int, materialName: str, angle: float, thickness: float = None) -> LaminateLayer:
 		return LaminateLayer(self._Entity.InsertLayer(layerId, materialName, angle, thickness))
 
 	def RemoveLayer(self, layerId: int) -> bool:
+		'''
+		Removes a layer from the laminate.
+		'''
 		return self._Entity.RemoveLayer(layerId)
 
 	def Save(self) -> None:
 		'''
 		Save any changes to this laminate material to the database.
 		'''
 		return self._Entity.Save()
@@ -4003,15 +4152,16 @@
 		return self._Entity.LayerId
 
 	@property
 	def LayerMaterialType(self) -> types.MaterialType:
 		'''
 		Represents a material's type.
 		'''
-		return types.MaterialType[self._Entity.LayerMaterialType.ToString()]
+		result = self._Entity.LayerMaterialType
+		return types.MaterialType[result.ToString()] if result is not None else None
 
 	@property
 	def Angle(self) -> float:
 		return self._Entity.Angle
 
 	@property
 	def Thickness(self) -> float:
@@ -4022,17 +4172,23 @@
 		return self._Entity.IsFabric
 
 	@Angle.setter
 	def Angle(self, value: float) -> None:
 		self._Entity.Angle = value
 
 	def AddLayerLocation(self, location: types.StiffenerLaminateLayerLocation) -> None:
+		'''
+		Add a layer location to this layer.
+		'''
 		return self._Entity.AddLayerLocation(_types.StiffenerLaminateLayerLocation(location.value))
 
 	def RemoveLayerLocation(self, location: types.StiffenerLaminateLayerLocation) -> bool:
+		'''
+		Remove a layer location from LayerLocations.
+		'''
 		return self._Entity.RemoveLayerLocation(_types.StiffenerLaminateLayerLocation(location.value))
 
 	@overload
 	def SetMaterial(self, matId: int) -> bool: ...
 
 	@overload
 	def SetMaterial(self, matName: str) -> bool: ...
@@ -4056,57 +4212,62 @@
 
 	@property
 	def Layers(self) -> list[StiffenerLaminateLayer]:
 		return [StiffenerLaminateLayer(stiffenerLaminateLayer) for stiffenerLaminateLayer in self._Entity.Layers]
 
 	@property
 	def LaminateStiffenerProfile(self) -> types.StiffenerProfile:
-		return types.StiffenerProfile[self._Entity.LaminateStiffenerProfile.ToString()]
+		result = self._Entity.LaminateStiffenerProfile
+		return types.StiffenerProfile[result.ToString()] if result is not None else None
 
 	@overload
 	def AddLayer(self, location: types.StiffenerLaminateLayerLocation, materialName: str, angle: float, thickness: float = None) -> StiffenerLaminateLayer: ...
 
 	@overload
 	def InsertLayer(self, location: types.StiffenerLaminateLayerLocation, layerId: int, materialName: str, angle: float, thickness: float = None) -> StiffenerLaminateLayer: ...
 
 	@overload
 	def AddLayer(self, locations: tuple[types.StiffenerLaminateLayerLocation], materialName: str, angle: float, thickness: float = None) -> StiffenerLaminateLayer: ...
 
 	@overload
 	def InsertLayer(self, locations: tuple[types.StiffenerLaminateLayerLocation], layerId: int, materialName: str, angle: float, thickness: float = None) -> StiffenerLaminateLayer: ...
 
 	def RemoveLayer(self, layerId: int) -> bool:
+		'''
+		Remove a layer by layerId.
+            Note, layerId is 1 indexed.
+		'''
 		return self._Entity.RemoveLayer(layerId)
 
 	def Save(self) -> None:
 		'''
 		Save laminate to database.
 		'''
 		return self._Entity.Save()
 
 	def AddLayer(self, item1 = None, item2 = None, item3 = None, item4 = None) -> StiffenerLaminateLayer:
-		if isinstance(item1, types.StiffenerLaminateLayerLocation) and isinstance(item2, str) and isinstance(item3, float) and isinstance(item4, float):
+		if isinstance(item1, types.StiffenerLaminateLayerLocation) and isinstance(item2, str) and isinstance(item3, float) and (isinstance(item3, float) or isinstance(item3, int)) and isinstance(item4, float) and (isinstance(item4, float) or item4 is None or isinstance(item4, int)):
 			return StiffenerLaminateLayer(self._Entity.AddLayer(_types.StiffenerLaminateLayerLocation(item1.value), item2, item3, item4))
 
-		if isinstance(item1, tuple) and item1 and isinstance(item1[0], types.StiffenerLaminateLayerLocation) and isinstance(item2, str) and isinstance(item3, float) and isinstance(item4, float):
+		if isinstance(item1, tuple) and item1 and isinstance(item1[0], types.StiffenerLaminateLayerLocation) and isinstance(item2, str) and isinstance(item3, float) and (isinstance(item3, float) or isinstance(item3, int)) and isinstance(item4, float) and (isinstance(item4, float) or item4 is None or isinstance(item4, int)):
 			locationsList = List[_types.StiffenerLaminateLayerLocation]()
 			if item1 is not None:
 				for thing in item1:
 					if thing is not None:
 						locationsList.Add(_types.StiffenerLaminateLayerLocation(thing.value))
 			locationsEnumerable = IEnumerable(locationsList)
 			return StiffenerLaminateLayer(self._Entity.AddLayer(locationsEnumerable, item2, item3, item4))
 
 		return StiffenerLaminateLayer(self._Entity.AddLayer(_types.StiffenerLaminateLayerLocation(item1.value), item2, item3, item4))
 
 	def InsertLayer(self, item1 = None, item2 = None, item3 = None, item4 = None, item5 = None) -> StiffenerLaminateLayer:
-		if isinstance(item1, types.StiffenerLaminateLayerLocation) and isinstance(item2, int) and isinstance(item3, str) and isinstance(item4, float) and isinstance(item5, float):
+		if isinstance(item1, types.StiffenerLaminateLayerLocation) and isinstance(item2, int) and isinstance(item3, str) and isinstance(item4, float) and (isinstance(item4, float) or isinstance(item4, int)) and isinstance(item5, float) and (isinstance(item5, float) or item5 is None or isinstance(item5, int)):
 			return StiffenerLaminateLayer(self._Entity.InsertLayer(_types.StiffenerLaminateLayerLocation(item1.value), item2, item3, item4, item5))
 
-		if isinstance(item1, tuple) and item1 and isinstance(item1[0], types.StiffenerLaminateLayerLocation) and isinstance(item2, int) and isinstance(item3, str) and isinstance(item4, float) and isinstance(item5, float):
+		if isinstance(item1, tuple) and item1 and isinstance(item1[0], types.StiffenerLaminateLayerLocation) and isinstance(item2, int) and isinstance(item3, str) and isinstance(item4, float) and (isinstance(item4, float) or isinstance(item4, int)) and isinstance(item5, float) and (isinstance(item5, float) or item5 is None or isinstance(item5, int)):
 			locationsList = List[_types.StiffenerLaminateLayerLocation]()
 			if item1 is not None:
 				for thing in item1:
 					if thing is not None:
 						locationsList.Add(_types.StiffenerLaminateLayerLocation(thing.value))
 			locationsEnumerable = IEnumerable(locationsList)
 			return StiffenerLaminateLayer(self._Entity.InsertLayer(locationsEnumerable, item2, item3, item4, item5))
@@ -4122,22 +4283,24 @@
 		self._Entity = orthotropicCorrectionFactorBase
 
 	@property
 	def CorrectionId(self) -> types.CorrectionId:
 		'''
 		Correction ID for a correction factor. (Columns in HyperX)
 		'''
-		return types.CorrectionId[self._Entity.CorrectionId.ToString()]
+		result = self._Entity.CorrectionId
+		return types.CorrectionId[result.ToString()] if result is not None else None
 
 	@property
 	def PropertyId(self) -> types.CorrectionProperty:
 		'''
 		Property name for a correction factor. (Rows in HyperX)
 		'''
-		return types.CorrectionProperty[self._Entity.PropertyId.ToString()]
+		result = self._Entity.PropertyId
+		return types.CorrectionProperty[result.ToString()] if result is not None else None
 
 
 class OrthotropicCorrectionFactorPoint:
 	'''
 	Pointer to an Equation-based or Tabular Correction Factor.
 	'''
 	def __init__(self, orthotropicCorrectionFactorPoint: _api.OrthotropicCorrectionFactorPoint):
@@ -4147,73 +4310,82 @@
 		return OrthotropicCorrectionFactorPoint(_api.OrthotropicCorrectionFactorPoint(_types.CorrectionProperty(property.value), _types.CorrectionId(id.value)))
 
 	@property
 	def CorrectionProperty(self) -> types.CorrectionProperty:
 		'''
 		Property name for a correction factor. (Rows in HyperX)
 		'''
-		return types.CorrectionProperty[self._Entity.CorrectionProperty.ToString()]
+		result = self._Entity.CorrectionProperty
+		return types.CorrectionProperty[result.ToString()] if result is not None else None
 
 	@property
 	def CorrectionId(self) -> types.CorrectionId:
 		'''
 		Correction ID for a correction factor. (Columns in HyperX)
 		'''
-		return types.CorrectionId[self._Entity.CorrectionId.ToString()]
+		result = self._Entity.CorrectionId
+		return types.CorrectionId[result.ToString()] if result is not None else None
 
 	@overload
 	def Equals(self, other) -> bool: ...
 
 	@overload
-	def Equals(self, obj) -> bool: ...
-
-	def GetHashCode(self) -> int:
-		return self._Entity.GetHashCode()
+	def Equals(self, obj: object) -> bool: ...
 
 	def Equals(self, item1 = None) -> bool:
 		if isinstance(item1, OrthotropicCorrectionFactorPoint):
 			return self._Entity.Equals(item1._Entity)
 
+		if isinstance(item1, object):
+			return self._Entity.Equals(item1)
+
 		return self._Entity.Equals(item1._Entity)
 
+	def __hash__(self) -> int:
+		return self._Entity.GetHashCode()
+
 
 class OrthotropicCorrectionFactorValue:
 	'''
 	Orthotropic material equation-based correction factor value. (NOT TABULAR)
 	'''
 	def __init__(self, orthotropicCorrectionFactorValue: _api.OrthotropicCorrectionFactorValue):
 		self._Entity = orthotropicCorrectionFactorValue
 
 	@property
 	def Property(self) -> types.CorrectionProperty:
 		'''
 		Property name for a correction factor. (Rows in HyperX)
 		'''
-		return types.CorrectionProperty[self._Entity.Property.ToString()]
+		result = self._Entity.Property
+		return types.CorrectionProperty[result.ToString()] if result is not None else None
 
 	@property
 	def Correction(self) -> types.CorrectionId:
 		'''
 		Correction ID for a correction factor. (Columns in HyperX)
 		'''
-		return types.CorrectionId[self._Entity.Correction.ToString()]
+		result = self._Entity.Correction
+		return types.CorrectionId[result.ToString()] if result is not None else None
 
 	@property
 	def Equation(self) -> types.CorrectionEquation:
 		'''
 		Equation for a correction factor.
 		'''
-		return types.CorrectionEquation[self._Entity.Equation.ToString()]
+		result = self._Entity.Equation
+		return types.CorrectionEquation[result.ToString()] if result is not None else None
 
 	@property
 	def EquationParameter(self) -> types.EquationParameterId:
 		'''
 		Correction factor parameter names.
 		'''
-		return types.EquationParameterId[self._Entity.EquationParameter.ToString()]
+		result = self._Entity.EquationParameter
+		return types.EquationParameterId[result.ToString()] if result is not None else None
 
 	@property
 	def Value(self) -> float:
 		return self._Entity.Value
 
 	@Value.setter
 	def Value(self, value: float) -> None:
@@ -4228,25 +4400,31 @@
 		self._Entity = orthotropicEquationCorrectionFactor
 
 	@property
 	def Equation(self) -> types.CorrectionEquation:
 		'''
 		Equation for a correction factor.
 		'''
-		return types.CorrectionEquation[self._Entity.Equation.ToString()]
+		result = self._Entity.Equation
+		return types.CorrectionEquation[result.ToString()] if result is not None else None
 
 	@property
 	def OrthotropicCorrectionValues(self) -> dict[types.EquationParameterId, OrthotropicCorrectionFactorValue]:
 		orthotropicCorrectionValuesDict = {}
 		for kvp in self._Entity.OrthotropicCorrectionValues:
 			orthotropicCorrectionValuesDict[types.EquationParameterId[kvp.Key.ToString()]] = OrthotropicCorrectionFactorValue(kvp.Value)
 
 		return orthotropicCorrectionValuesDict
 
 	def AddCorrectionFactorValue(self, equationParameterName: types.EquationParameterId, valueToAdd: float) -> OrthotropicCorrectionFactorValue:
+		'''
+		Add a correction factor value for a given correction factor.
+		:param equationParameterName: This represents the parameter of the equation that should be changed.
+		:param valueToAdd: This is the value that will be assigned to the chosen parameter.
+		'''
 		return OrthotropicCorrectionFactorValue(self._Entity.AddCorrectionFactorValue(_types.EquationParameterId(equationParameterName.value), valueToAdd))
 
 
 class TabularCorrectionFactorIndependentValue:
 	'''
 	Contains an independent value for a tabular correction factor row.
 	'''
@@ -4266,15 +4444,16 @@
 		return self._Entity.IntValue
 
 	@property
 	def ValueType(self) -> types.CorrectionValueType:
 		'''
 		Defines the type of the independent values on a tabular correction factor row.
 		'''
-		return types.CorrectionValueType[self._Entity.ValueType.ToString()]
+		result = self._Entity.ValueType
+		return types.CorrectionValueType[result.ToString()] if result is not None else None
 
 
 class TabularCorrectionFactorRow:
 	'''
 	Row data for a tabular correction factor.
 	'''
 	def __init__(self, tabularCorrectionFactorRow: _api.TabularCorrectionFactorRow):
@@ -4318,18 +4497,21 @@
 	@overload
 	def SetIndependentValue(self, correctionPointId: int, cid: types.CorrectionIndependentDefinition, value: bool) -> None: ...
 
 	@overload
 	def SetIndependentValue(self, correctionPointId: int, cid: types.CorrectionIndependentDefinition, value: int) -> None: ...
 
 	def SetKValue(self, correctionPointId: int, value: float) -> None:
+		'''
+		Set the dependent value for a specified row.
+		'''
 		return self._Entity.SetKValue(correctionPointId, value)
 
 	def SetIndependentValue(self, item1 = None, item2 = None, item3 = None) -> None:
-		if isinstance(item1, int) and isinstance(item2, types.CorrectionIndependentDefinition) and isinstance(item3, float):
+		if isinstance(item1, int) and isinstance(item2, types.CorrectionIndependentDefinition) and isinstance(item3, float) and (isinstance(item3, float) or isinstance(item3, int)):
 			return self._Entity.SetIndependentValue(item1, _types.CorrectionIndependentDefinition(item2.value), item3)
 
 		if isinstance(item1, int) and isinstance(item2, types.CorrectionIndependentDefinition) and isinstance(item3, bool):
 			return self._Entity.SetIndependentValue(item1, _types.CorrectionIndependentDefinition(item2.value), item3)
 
 		if isinstance(item1, int) and isinstance(item2, types.CorrectionIndependentDefinition) and isinstance(item3, int):
 			return self._Entity.SetIndependentValue(item1, _types.CorrectionIndependentDefinition(item2.value), item3)
@@ -4345,15 +4527,16 @@
 		self._Entity = orthotropicAllowableCurvePoint
 
 	@property
 	def Property_ID(self) -> types.AllowablePropertyName:
 		'''
 		Property name for a laminate allowable.
 		'''
-		return types.AllowablePropertyName[self._Entity.Property_ID.ToString()]
+		result = self._Entity.Property_ID
+		return types.AllowablePropertyName[result.ToString()] if result is not None else None
 
 	@property
 	def Temperature(self) -> float:
 		return self._Entity.Temperature
 
 	@property
 	def X(self) -> float:
@@ -4437,22 +4620,24 @@
 		self._Entity = orthotropicLaminateAllowable
 
 	@property
 	def Property_ID(self) -> types.AllowablePropertyName:
 		'''
 		Property name for a laminate allowable.
 		'''
-		return types.AllowablePropertyName[self._Entity.Property_ID.ToString()]
+		result = self._Entity.Property_ID
+		return types.AllowablePropertyName[result.ToString()] if result is not None else None
 
 	@property
 	def Method_ID(self) -> types.AllowableMethodName:
 		'''
 		Method name for a laminate allowable.
 		'''
-		return types.AllowableMethodName[self._Entity.Method_ID.ToString()]
+		result = self._Entity.Method_ID
+		return types.AllowableMethodName[result.ToString()] if result is not None else None
 
 	@Property_ID.setter
 	def Property_ID(self, value: types.AllowablePropertyName) -> None:
 		self._Entity.Property_ID = _types.AllowablePropertyName(value.value)
 
 	@Method_ID.setter
 	def Method_ID(self, value: types.AllowableMethodName) -> None:
@@ -4779,20 +4964,32 @@
 		self._Entity.TTt = value
 
 	@TTc.setter
 	def TTc(self, value: float) -> None:
 		self._Entity.TTc = value
 
 	def AddCurvePoint(self, property: types.AllowablePropertyName, x: float, y: float) -> OrthotropicAllowableCurvePoint:
+		'''
+		Add a curve point to a laminate allowable curve.
+		:param x: x represents an x-value (for a non-polynomial method) or an allowable polynomial coefficient (represented by an enum).
+		'''
 		return OrthotropicAllowableCurvePoint(self._Entity.AddCurvePoint(_types.AllowablePropertyName(property.value), x, y))
 
 	def DeleteCurvePoint(self, property: types.AllowablePropertyName, x: float) -> bool:
+		'''
+		Deletes a temperature-dependent property for a material.
+		:param x: x represents an x-value (for a non-polynomial method) or an allowable polynomial coefficient (represented by an enum).
+		'''
 		return self._Entity.DeleteCurvePoint(_types.AllowablePropertyName(property.value), x)
 
 	def GetCurvePoint(self, property: types.AllowablePropertyName, x: float) -> OrthotropicAllowableCurvePoint:
+		'''
+		Retrieve an allowable curve point from this temperature's allowable curve points.
+		:param x: x represents an x-value (for a non-polynomial method) or an allowable polynomial coefficient (represented by an enum).
+		'''
 		return OrthotropicAllowableCurvePoint(self._Entity.GetCurvePoint(_types.AllowablePropertyName(property.value), x))
 
 
 class Orthotropic:
 	'''
 	Orthotropic material.
 	'''
@@ -4985,44 +5182,83 @@
 		self._Entity.Cost = value
 
 	@BucklingStiffnessKnockdown.setter
 	def BucklingStiffnessKnockdown(self, value: float) -> None:
 		self._Entity.BucklingStiffnessKnockdown = value
 
 	def AddTemperatureProperty(self, temperature: float, et1: float, et2: float, vt12: float, ec1: float, ec2: float, vc12: float, g12: float, ftu1: float, ftu2: float, fcu1: float, fcu2: float, fsu12: float, alpha1: float, alpha2: float, etu1: float, etu2: float, ecu1: float, ecu2: float, esu12: float) -> OrthotropicTemperature:
+		'''
+		Adds a temperature-dependent property for a material.
+		'''
 		return OrthotropicTemperature(self._Entity.AddTemperatureProperty(temperature, et1, et2, vt12, ec1, ec2, vc12, g12, ftu1, ftu2, fcu1, fcu2, fsu12, alpha1, alpha2, etu1, etu2, ecu1, ecu2, esu12))
 
 	def DeleteTemperatureProperty(self, temperature: float) -> bool:
+		'''
+		Deletes a temperature-dependent property for a material.
+		'''
 		return self._Entity.DeleteTemperatureProperty(temperature)
 
 	def GetTemperature(self, lookupTemperature: float) -> OrthotropicTemperature:
+		'''
+		Retrieve a Temperature from this material's temperature-dependent properties. Allows a degree of tolerance to avoid issues with floating point numbers.
+		:param LookupTemperature: Temperature to search for.
+		'''
 		return OrthotropicTemperature(self._Entity.GetTemperature(lookupTemperature))
 
 	def IsEffectiveLaminate(self) -> bool:
 		'''
 		Returns true if this material is an effective laminate.
 		'''
 		return self._Entity.IsEffectiveLaminate()
 
 	def HasLaminateAllowable(self, property: types.AllowablePropertyName) -> bool:
+		'''
+		Returns true if this material has a specified laminate allowable property.
+		'''
 		return self._Entity.HasLaminateAllowable(_types.AllowablePropertyName(property.value))
 
 	def AddLaminateAllowable(self, property: types.AllowablePropertyName, method: types.AllowableMethodName) -> OrthotropicLaminateAllowable:
+		'''
+		Adds a laminate allowable to this material.
+            An orthotropic material can only have one laminate allowable of each property (as specified by the property argument).
+		:param property: The strain or stress property for a laminate allowable.
+		:param method: The method for a laminate allowable (AML, Percent 0/45, Polynomial).
+		'''
 		return OrthotropicLaminateAllowable(self._Entity.AddLaminateAllowable(_types.AllowablePropertyName(property.value), _types.AllowableMethodName(method.value)))
 
 	def GetLaminateAllowable(self, lookupAllowableProperty: types.AllowablePropertyName) -> OrthotropicLaminateAllowable:
+		'''
+		Retrieve a Laminate allowable from this material's laminate allowables.
+		:param LookupAllowableProperty: Laminate allowable property to search for.
+		'''
 		return OrthotropicLaminateAllowable(self._Entity.GetLaminateAllowable(_types.AllowablePropertyName(lookupAllowableProperty.value)))
 
 	def AddEquationCorrectionFactor(self, propertyId: types.CorrectionProperty, correctionId: types.CorrectionId, equationId: types.CorrectionEquation) -> OrthotropicEquationCorrectionFactor:
+		'''
+		Adds an equation-based correction factor for this material.
+		:param propertyId: The ID of the property to be affected by the correction factor. Specified with a CorrectionPropertyName enum.
+		:param correctionId: The ID for the type of correction factor to be applied. Specified with a CorrectionIDName enum.
+		:param equationId: The ID for the type of correction factor equation to use. Specified with a CorrectionEquationName enum.
+		'''
 		return OrthotropicEquationCorrectionFactor(self._Entity.AddEquationCorrectionFactor(_types.CorrectionProperty(propertyId.value), _types.CorrectionId(correctionId.value), _types.CorrectionEquation(equationId.value)))
 
 	def GetEquationCorrectionFactor(self, property: types.CorrectionProperty, correction: types.CorrectionId) -> OrthotropicEquationCorrectionFactor:
+		'''
+		Retrieve a Correction Factor from this material's correction factors.
+		:param property: CorrectionPropertyName to search for.
+		:param correction: CorrectionIDName to search for.
+		'''
 		return OrthotropicEquationCorrectionFactor(self._Entity.GetEquationCorrectionFactor(_types.CorrectionProperty(property.value), _types.CorrectionId(correction.value)))
 
 	def GetTabularCorrectionFactor(self, property: types.CorrectionProperty, correction: types.CorrectionId) -> OrthotropicTabularCorrectionFactor:
+		'''
+		Retrieve a Correction Factor from this material's correction factors.
+		:param property: CorrectionPropertyName to search for.
+		:param correction: CorrectionIDName to search for.
+		'''
 		return OrthotropicTabularCorrectionFactor(self._Entity.GetTabularCorrectionFactor(_types.CorrectionProperty(property.value), _types.CorrectionId(correction.value)))
 
 	def Save(self) -> None:
 		'''
 		Save any changes to this orthotropic material to the database.
 		'''
 		return self._Entity.Save()
@@ -5046,31 +5282,34 @@
 	def Y(self) -> float:
 		return self._Entity.Y
 
 	@overload
 	def Equals(self, other) -> bool: ...
 
 	@overload
-	def Equals(self, obj) -> bool: ...
-
-	def GetHashCode(self) -> int:
-		return self._Entity.GetHashCode()
+	def Equals(self, obj: object) -> bool: ...
 
 	def Equals(self, item1 = None) -> bool:
 		if isinstance(item1, Vector2d):
 			return self._Entity.Equals(item1._Entity)
 
+		if isinstance(item1, object):
+			return self._Entity.Equals(item1)
+
 		return self._Entity.Equals(item1._Entity)
 
 	def __eq__(self, other):
 		return self.Equals(other)
 
 	def __ne__(self, other):
 		return not self.Equals(other)
 
+	def __hash__(self) -> int:
+		return self._Entity.GetHashCode()
+
 
 class ElementSet(IdNameEntity):
 	'''
 	A set of elements defined in the input file.
 	'''
 	def __init__(self, elementSet: _api.ElementSet):
 		self._Entity = elementSet
@@ -5091,15 +5330,16 @@
 	@property
 	def Elements(self) -> ElementCol:
 		result = self._Entity.Elements
 		return ElementCol(result) if result is not None else None
 
 	@property
 	def FemType(self) -> types.FemType:
-		return types.FemType[self._Entity.FemType.ToString()]
+		result = self._Entity.FemType
+		return types.FemType[result.ToString()] if result is not None else None
 
 
 class ElementSetCol(IdEntityCol[ElementSet]):
 	def __init__(self, elementSetCol: _api.ElementSetCol):
 		self._Entity = elementSetCol
 		self._CollectedClass = ElementSet
 
@@ -5235,17 +5475,25 @@
 		return self._Entity.IsPrimary
 
 	@property
 	def ResultFilePath(self) -> str:
 		return self._Entity.ResultFilePath
 
 	def SetInputFilePath(self, filepath: str) -> RundeckUpdateStatus:
+		'''
+		The rundeck's input file path will point to the provided file path
+		:param filepath: The path to the rundeck
+		'''
 		return RundeckUpdateStatus[self._Entity.SetInputFilePath(filepath).ToString()]
 
 	def SetResultFilePath(self, filepath: str) -> RundeckUpdateStatus:
+		'''
+		The rundeck's result file path will point to the provided file path
+		:param filepath: The path to the result file
+		'''
 		return RundeckUpdateStatus[self._Entity.SetResultFilePath(filepath).ToString()]
 
 
 class RundeckPathPair:
 	def __init__(self, rundeckPathPair: _api.RundeckPathPair):
 		self._Entity = rundeckPathPair
 
@@ -5300,15 +5548,16 @@
 		self._Entity = sectionCut
 
 	@property
 	def ReferencePoint(self) -> types.SectionCutPropertyLocation:
 		'''
 		Centroid vs Origin
 		'''
-		return types.SectionCutPropertyLocation[self._Entity.ReferencePoint.ToString()]
+		result = self._Entity.ReferencePoint
+		return types.SectionCutPropertyLocation[result.ToString()] if result is not None else None
 
 	@property
 	def HorizontalVector(self) -> Vector3d:
 		'''
 		Represents a readonly 3D vector.
 		'''
 		result = self._Entity.HorizontalVector
@@ -5554,21 +5803,21 @@
 	def SetOrigin(self, vector: Vector3d) -> None:
 		return self._Entity.SetOrigin(vector._Entity)
 
 	def GetBeamLoads(self, loadCaseId: int, factor: types.LoadSubCaseFactor) -> BeamLoads:
 		return BeamLoads(self._Entity.GetBeamLoads(loadCaseId, _types.LoadSubCaseFactor(factor.value)))
 
 	def InclinationAngle(self, loadCaseId: int, factor: types.LoadSubCaseFactor) -> float:
-		return self._Entity.InclinationAngle(loadCaseId, _types.LoadSubCaseFactor(factor.value))
+		return float(self._Entity.InclinationAngle(loadCaseId, _types.LoadSubCaseFactor(factor.value)))
 
 	def HorizontalIntercept(self, loadCaseId: int, factor: types.LoadSubCaseFactor) -> float:
-		return self._Entity.HorizontalIntercept(loadCaseId, _types.LoadSubCaseFactor(factor.value))
+		return float(self._Entity.HorizontalIntercept(loadCaseId, _types.LoadSubCaseFactor(factor.value)))
 
 	def VerticalIntercept(self, loadCaseId: int, factor: types.LoadSubCaseFactor) -> float:
-		return self._Entity.VerticalIntercept(loadCaseId, _types.LoadSubCaseFactor(factor.value))
+		return float(self._Entity.VerticalIntercept(loadCaseId, _types.LoadSubCaseFactor(factor.value)))
 
 	def SetElements(self, elements: list[int]) -> bool:
 		elementsList = MakeCSharpIntList(elements)
 		return self._Entity.SetElements(elementsList)
 
 	def SetElementsByIntersection(self) -> None:
 		return self._Entity.SetElementsByIntersection()
@@ -5771,14 +6020,17 @@
 	def DeleteAll(self) -> None:
 		'''
 		Delete all plies in the collection.
 		'''
 		return self._Entity.DeleteAll()
 
 	def ExportToCSV(self, filepath: str) -> None:
+		'''
+		This feature is in development and may not work as expected. Use at your own risk!
+		'''
 		return self._Entity.ExportToCSV(filepath)
 
 	def ImportCSV(self, filepath: str) -> None:
 		return self._Entity.ImportCSV(filepath)
 
 	@overload
 	def Get(self, name: str) -> Ply: ...
@@ -5826,14 +6078,17 @@
 
 	@property
 	def Zones(self) -> ZoneCol:
 		result = self._Entity.Zones
 		return ZoneCol(result) if result is not None else None
 
 	def ExportVCP(self, fileName: str) -> None:
+		'''
+		Export VCP with this structure's element centroids.
+		'''
 		return self._Entity.ExportVCP(fileName)
 
 	def AddElements(self, elementIds: tuple[int]) -> CollectionModificationStatus:
 		elementIdsList = MakeCSharpIntList(elementIds)
 		elementIdsEnumerable = IEnumerable(elementIdsList)
 		return CollectionModificationStatus[self._Entity.AddElements(elementIdsEnumerable).ToString()]
 
@@ -5856,20 +6111,22 @@
 		elementIdsEnumerable = IEnumerable(elementIdsList)
 		result = self._Entity.CreateZone(elementIdsEnumerable, name)
 		thisClass = type(result).__name__
 		givenClass = Zone
 		for subclass in Zone.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		return givenClass(result)
+		return givenClass(result) if result is not None else None
 
 	def CreatePanelSegment(self, discreteTechnique: types.DiscreteTechnique, discreteElementLkp: dict[types.DiscreteDefinitionType, list[int]], name: str = None) -> PanelSegment:
 		discreteElementLkpDict = Dictionary[_types.DiscreteDefinitionType, List[int]]()
 		for kvp in discreteElementLkp:
-			discreteElementLkpDict.Add(_types.DiscreteDefinitionType(kvp.value), MakeCSharpIntList(discreteElementLkp[kvp]))
+			dictValue = discreteElementLkp[kvp]
+			dictValueList = MakeCSharpIntList(dictValue)
+			discreteElementLkpDict.Add(_types.DiscreteDefinitionType(kvp.value), dictValueList)
 		return PanelSegment(self._Entity.CreatePanelSegment(_types.DiscreteTechnique(discreteTechnique.value), discreteElementLkpDict, name))
 
 	@overload
 	def Remove(self, zoneIds: tuple[int], jointIds: tuple[int]) -> CollectionModificationStatus: ...
 
 	@overload
 	def Remove(self, zoneIds: tuple[int], jointIds: tuple[int], panelSegmentIds: tuple[int]) -> CollectionModificationStatus: ...
@@ -6053,14 +6310,17 @@
 		self._CollectedClass = AnalysisProperty
 
 	@property
 	def AnalysisPropertyColList(self) -> tuple[AnalysisProperty]:
 		return tuple([AnalysisProperty(analysisPropertyCol) for analysisPropertyCol in self._Entity])
 
 	def CreateAnalysisProperty(self, type: types.FamilyCategory, name: str = None) -> AnalysisProperty:
+		'''
+		Create an AnalysisProperty.
+		'''
 		return AnalysisProperty(self._Entity.CreateAnalysisProperty(_types.FamilyCategory(type.value), name))
 
 	@overload
 	def DeleteAnalysisProperty(self, name: str) -> bool: ...
 
 	@overload
 	def DeleteAnalysisProperty(self, id: int) -> bool: ...
@@ -6105,42 +6365,57 @@
 		self._CollectedClass = DesignProperty
 
 	@property
 	def DesignPropertyColList(self) -> tuple[DesignProperty]:
 		return tuple([DesignProperty(designPropertyCol) for designPropertyCol in self._Entity])
 
 	def CreateDesignProperty(self, familyConcept: types.FamilyConceptUID, materialMode: types.MaterialMode = types.MaterialMode.Any, name: str = None) -> DesignProperty:
+		'''
+		Create a DesignProperty.
+		'''
 		result = self._Entity.CreateDesignProperty(_types.FamilyConceptUID(familyConcept.value), _types.MaterialMode(materialMode.value), name)
 		thisClass = type(result).__name__
 		givenClass = DesignProperty
 		for subclass in DesignProperty.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		return givenClass(result)
+		return givenClass(result) if result is not None else None
 
 	@overload
 	def Get(self, name: str) -> DesignProperty: ...
 
 	@overload
 	def Get(self, id: int) -> DesignProperty: ...
 
 	def Get(self, item1 = None) -> DesignProperty:
 		if isinstance(item1, str):
-			return DesignProperty(super().Get(item1))
+			result = super().Get(item1)
+			thisClass = type(result).__name__
+			givenClass = DesignProperty
+			for subclass in DesignProperty.__subclasses__():
+				if subclass.__name__ == thisClass:
+					givenClass = subclass
+			return givenClass(result) if result is not None else None
 
 		if isinstance(item1, int):
-			return DesignProperty(super().Get(item1))
+			result = super().Get(item1)
+			thisClass = type(result).__name__
+			givenClass = DesignProperty
+			for subclass in DesignProperty.__subclasses__():
+				if subclass.__name__ == thisClass:
+					givenClass = subclass
+			return givenClass(result) if result is not None else None
 
 		result = self._Entity.Get(item1)
 		thisClass = type(result).__name__
 		givenClass = DesignProperty
 		for subclass in DesignProperty.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		return givenClass(result)
+		return givenClass(result) if result is not None else None
 
 	def __getitem__(self, index: int):
 		return self.DesignPropertyColList[index]
 
 	def __iter__(self):
 		yield from self.DesignPropertyColList
 
@@ -6154,21 +6429,24 @@
 		self._CollectedClass = LoadProperty
 
 	@property
 	def LoadPropertyColList(self) -> tuple[LoadProperty]:
 		return tuple([LoadProperty(loadPropertyCol) for loadPropertyCol in self._Entity])
 
 	def CreateLoadProperty(self, loadPropertyType: types.LoadPropertyType, category: types.FamilyCategory, name: str = None) -> LoadProperty:
+		'''
+		Create a new load property.
+		'''
 		result = self._Entity.CreateLoadProperty(_types.LoadPropertyType(loadPropertyType.value), _types.FamilyCategory(category.value), name)
 		thisClass = type(result).__name__
 		givenClass = LoadProperty
 		for subclass in LoadProperty.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		return givenClass(result)
+		return givenClass(result) if result is not None else None
 
 	@overload
 	def DeleteLoadProperty(self, id: int) -> bool: ...
 
 	@overload
 	def DeleteLoadProperty(self, name: str) -> bool: ...
 
@@ -6185,26 +6463,38 @@
 		if isinstance(item1, str):
 			return self._Entity.DeleteLoadProperty(item1)
 
 		return self._Entity.DeleteLoadProperty(item1)
 
 	def Get(self, item1 = None) -> LoadProperty:
 		if isinstance(item1, str):
-			return LoadProperty(super().Get(item1))
+			result = super().Get(item1)
+			thisClass = type(result).__name__
+			givenClass = LoadProperty
+			for subclass in LoadProperty.__subclasses__():
+				if subclass.__name__ == thisClass:
+					givenClass = subclass
+			return givenClass(result) if result is not None else None
 
 		if isinstance(item1, int):
-			return LoadProperty(super().Get(item1))
+			result = super().Get(item1)
+			thisClass = type(result).__name__
+			givenClass = LoadProperty
+			for subclass in LoadProperty.__subclasses__():
+				if subclass.__name__ == thisClass:
+					givenClass = subclass
+			return givenClass(result) if result is not None else None
 
 		result = self._Entity.Get(item1)
 		thisClass = type(result).__name__
 		givenClass = LoadProperty
 		for subclass in LoadProperty.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		return givenClass(result)
+		return givenClass(result) if result is not None else None
 
 	def __getitem__(self, index: int):
 		return self.LoadPropertyColList[index]
 
 	def __iter__(self):
 		yield from self.LoadPropertyColList
 
@@ -6252,20 +6542,30 @@
 		self._CollectedClass = DiscreteField
 
 	@property
 	def DiscreteFieldColList(self) -> tuple[DiscreteField]:
 		return tuple([DiscreteField(discreteFieldCol) for discreteFieldCol in self._Entity])
 
 	def Create(self, entityType: types.DiscreteFieldPhysicalEntityType, dataType: types.DiscreteFieldDataType, name: str = None) -> DiscreteField:
+		'''
+		Create a new DiscreteField.
+		'''
 		return DiscreteField(self._Entity.Create(_types.DiscreteFieldPhysicalEntityType(entityType.value), _types.DiscreteFieldDataType(dataType.value), name))
 
 	def CreateFromVCP(self, filepath: str) -> list[DiscreteField]:
+		'''
+		Create a list of DiscreteFields from VCP.
+		'''
 		return [DiscreteField(discreteField) for discreteField in self._Entity.CreateFromVCP(filepath)]
 
 	def Delete(self, id: int) -> CollectionModificationStatus:
+		'''
+		In the event of getting a CollectionModificationStatus.EntityMissingRemovalFailure,
+            note that the discrete field is associated with a ply, and therefore cannot be deleted.
+		'''
 		return CollectionModificationStatus[self._Entity.Delete(id).ToString()]
 
 	def CreateByPointMapToElements(self, elementIds: list[int], discreteFieldIds: list[int], suffix: str = None, tolerance: float = None) -> list[DiscreteField]:
 		elementIdsList = MakeCSharpIntList(elementIds)
 		discreteFieldIdsList = MakeCSharpIntList(discreteFieldIds)
 		return [DiscreteField(discreteField) for discreteField in self._Entity.CreateByPointMapToElements(elementIdsList, discreteFieldIdsList, suffix, tolerance)]
 
@@ -6345,20 +6645,34 @@
 		self._CollectedClass = Rundeck
 
 	@property
 	def RundeckColList(self) -> tuple[Rundeck]:
 		return tuple([Rundeck(rundeckCol) for rundeckCol in self._Entity])
 
 	def AddRundeck(self, inputPath: str, resultPath: str = None) -> Rundeck:
+		'''
+		The specified rundeck at the given filepath will be added to the project's
+            collection of rundecks
+		:param inputPath: The path to the rundeck
+		:param resultPath: The path to the rundeck's corresponding result file
+		'''
 		return Rundeck(self._Entity.AddRundeck(inputPath, resultPath))
 
 	def ReassignPrimary(self, id: int) -> RundeckUpdateStatus:
+		'''
+		The specified rundeck will be updated to become the new primary rundeck.
+		'''
 		return RundeckUpdateStatus[self._Entity.ReassignPrimary(id).ToString()]
 
 	def RemoveRundeck(self, id: int) -> RundeckRemoveStatus:
+		'''
+		The specified rundeck at the given filepath will be removed from the project's
+            collection of rundecks
+		:param id: The id of the rundeck to remove
+		'''
 		return RundeckRemoveStatus[self._Entity.RemoveRundeck(id).ToString()]
 
 	def UpdateAllRundecks(self, newPaths: list[RundeckPathPair]) -> RundeckBulkUpdateStatus:
 		newPathsList = List[_api.RundeckPathPair]()
 		if newPaths is not None:
 			for thing in newPaths:
 				if thing is not None:
@@ -6368,14 +6682,17 @@
 	def GetRundeckPathSetters(self) -> list[RundeckPathPair]:
 		'''
 		Get RundeckPathSetters to be edited and input to UpdateAllRundecks.
 		'''
 		return [RundeckPathPair(rundeckPathPair) for rundeckPathPair in self._Entity.GetRundeckPathSetters()]
 
 	def ReplaceStringInAllPaths(self, stringToReplace: str, newString: str) -> RundeckBulkUpdateStatus:
+		'''
+		Replace a given string with a new string in every rundeck path. This is useful when pointing to rundecks of the same name in a new directory.
+		'''
 		return RundeckBulkUpdateStatus[self._Entity.ReplaceStringInAllPaths(stringToReplace, newString).ToString()]
 
 	def __getitem__(self, index: int):
 		return self.RundeckColList[index]
 
 	def __iter__(self):
 		yield from self.RundeckColList
@@ -6430,14 +6747,18 @@
 		self._CollectedClass = Set
 
 	@property
 	def SetColList(self) -> tuple[Set]:
 		return tuple([Set(setCol) for setCol in self._Entity])
 
 	def Create(self, name: str = None) -> Set:
+		'''
+		Attempt to create a new Set.
+		:param name: The name of the set to be created.
+		'''
 		return Set(self._Entity.Create(name))
 
 	@overload
 	def Get(self, name: str) -> Set: ...
 
 	@overload
 	def Get(self, id: int) -> Set: ...
@@ -6467,14 +6788,19 @@
 		self._CollectedClass = Structure
 
 	@property
 	def StructureColList(self) -> tuple[Structure]:
 		return tuple([Structure(structureCol) for structureCol in self._Entity])
 
 	def Create(self, name: str = None) -> Structure:
+		'''
+		Attempt to create a new structure.
+            If the specified name is already used, it will be deconflicted.
+		:param name: The name of the structure to be created.
+		'''
 		return Structure(self._Entity.Create(name))
 
 	@overload
 	def DeleteStructure(self, structure: Structure) -> bool: ...
 
 	@overload
 	def DeleteStructure(self, name: str) -> bool: ...
@@ -6616,15 +6942,16 @@
 	@property
 	def LoadProperties(self) -> LoadPropertyCol:
 		result = self._Entity.LoadProperties
 		return LoadPropertyCol(result) if result is not None else None
 
 	@property
 	def FemFormat(self) -> types.ProjectModelFormat:
-		return types.ProjectModelFormat[self._Entity.FemFormat.ToString()]
+		result = self._Entity.FemFormat
+		return types.ProjectModelFormat[result.ToString()] if result is not None else None
 
 	def Upload(self, uploadSetName: str, company: str, program: str, tags: list[str], notes: str, zoneIds: set[int], jointIds: set[int]) -> bool:
 		tagsList = List[str]()
 		if tags is not None:
 			for thing in tags:
 				if thing is not None:
 					tagsList.Add(thing)
@@ -6644,26 +6971,38 @@
 		'''
 		This method fetches an array of Dashboard company names that are available to the user who is currently logged in. The URL and authentication token are taken from the last
             Dashboard login made through HyperX.
 		'''
 		return list[str](self._Entity.GetDashboardCompanies())
 
 	def GetDashboardPrograms(self, companyName: str) -> list[str]:
+		'''
+		This method fetches an array of Dashboard program names that are available to the user who is currently logged in. The URL and authentication token are taken from the last
+            Dashboard login made through HyperX.
+		'''
 		return list[str](self._Entity.GetDashboardPrograms(companyName))
 
 	def GetDashboardTags(self, companyName: str) -> list[str]:
+		'''
+		This method fetches an array of Dashboard tags that are available to the user who is currently logged in. The URL and authentication token are taken from the last
+            Dashboard login made through HyperX.
+		'''
 		return list[str](self._Entity.GetDashboardTags(companyName))
 
 	def Dispose(self) -> None:
 		return self._Entity.Dispose()
 
 	def ImportFem(self) -> None:
 		return self._Entity.ImportFem()
 
 	def ImportFeaResults(self, alwaysImport: bool = False) -> str:
+		'''
+		Manually import design loads.
+		:param alwaysImport: If true, loads are imported even if loads have already previously been imported.
+		'''
 		return self._Entity.ImportFeaResults(alwaysImport)
 
 	def SetFemFormat(self, femFormat: types.ProjectModelFormat) -> None:
 		return self._Entity.SetFemFormat(_types.ProjectModelFormat(femFormat.value))
 
 	def SetFemUnits(self, femForceId: DbForceUnit, femLengthId: DbLengthUnit, femMassId: DbMassUnit, femTemperatureId: DbTemperatureUnit) -> SetUnitsStatus:
 		return SetUnitsStatus[self._Entity.SetFemUnits(_api.DbForceUnit(femForceId.value), _api.DbLengthUnit(femLengthId.value), _api.DbMassUnit(femMassId.value), _api.DbTemperatureUnit(femTemperatureId.value)).ToString()]
@@ -6693,21 +7032,24 @@
 	@overload
 	def SizeZones(self, zones: list[Zone] = None) -> types.SimpleStatus: ...
 
 	@overload
 	def SizeZones(self, zoneIds: list[int]) -> types.SimpleStatus: ...
 
 	def CreateNonFeaZone(self, category: types.FamilyCategory, name: str = None) -> Zone:
+		'''
+		Create a non-FEA zone by name and category.
+		'''
 		result = self._Entity.CreateNonFeaZone(_types.FamilyCategory(category.value), name)
 		thisClass = type(result).__name__
 		givenClass = Zone
 		for subclass in Zone.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		return givenClass(result)
+		return givenClass(result) if result is not None else None
 
 	def ReturnToUnusedFem(self, zoneNumbers: list[int] = None, jointIds: set[int] = None) -> None:
 		zoneNumbersList = MakeCSharpIntList(zoneNumbers)
 		jointIdsSet = HashSet[int]()
 		if jointIds is not None:
 			for thing in jointIds:
 				if thing is not None:
@@ -6717,14 +7059,17 @@
 	def UnimportFemAsync(self) -> Task:
 		return Task(self._Entity.UnimportFemAsync())
 
 	def ExportFem(self, destinationFolder: str) -> None:
 		return self._Entity.ExportFem(destinationFolder)
 
 	def ImportCad(self, filePath: str) -> None:
+		'''
+		Import CAD from a file.
+		'''
 		return self._Entity.ImportCad(filePath)
 
 	@overload
 	def ExportCad(self, filePath: str) -> None: ...
 
 	@overload
 	def ExportCad(self, cadIds: tuple[int], filePath: str) -> None: ...
@@ -6825,26 +7170,36 @@
 	def FoamColList(self) -> tuple[Foam]:
 		return tuple([Foam(foamCol) for foamCol in self._Entity])
 
 	def Count(self) -> int:
 		return self._Entity.Count()
 
 	def Get(self, materialName: str) -> Foam:
+		'''
+		Look up an Foam material by its name.
+		'''
 		return Foam(self._Entity.Get(materialName))
 
 	def Contains(self, materialName: str) -> bool:
+		'''
+		Check if an foam material exists in this collection.
+		'''
 		return self._Entity.Contains(materialName)
 
 	def Create(self, materialFamilyName: str, density: float, newMaterialName: str = None, femId: int = None) -> Foam:
 		return Foam(self._Entity.Create(materialFamilyName, density, newMaterialName, femId))
 
 	def Copy(self, fmToCopyName: str, newMaterialName: str = None, femId: int = None) -> Foam:
 		return Foam(self._Entity.Copy(fmToCopyName, newMaterialName, femId))
 
 	def Delete(self, materialName: str) -> bool:
+		'''
+		Delete a foam material by name.
+            Returns false if the method the material is not found.
+		'''
 		return self._Entity.Delete(materialName)
 
 	def __getitem__(self, index: int):
 		return self.FoamColList[index]
 
 	def __iter__(self):
 		yield from self.FoamColList
@@ -6861,26 +7216,36 @@
 	def HoneycombColList(self) -> tuple[Honeycomb]:
 		return tuple([Honeycomb(honeycombCol) for honeycombCol in self._Entity])
 
 	def Count(self) -> int:
 		return self._Entity.Count()
 
 	def Get(self, materialName: str) -> Honeycomb:
+		'''
+		Look up an Honeycomb material by its name.
+		'''
 		return Honeycomb(self._Entity.Get(materialName))
 
 	def Contains(self, materialName: str) -> bool:
+		'''
+		Check if an honeycomb material exists in this collection.
+		'''
 		return self._Entity.Contains(materialName)
 
 	def Create(self, materialFamilyName: str, density: float, newMaterialName: str = None, femId: int = None) -> Honeycomb:
 		return Honeycomb(self._Entity.Create(materialFamilyName, density, newMaterialName, femId))
 
 	def Copy(self, honeyToCopyName: str, newMaterialName: str = None, femId: int = None) -> Honeycomb:
 		return Honeycomb(self._Entity.Copy(honeyToCopyName, newMaterialName, femId))
 
 	def Delete(self, materialName: str) -> bool:
+		'''
+		Delete a honeycomb material by name.
+            Returns false if the method the material is not found.
+		'''
 		return self._Entity.Delete(materialName)
 
 	def __getitem__(self, index: int):
 		return self.HoneycombColList[index]
 
 	def __iter__(self):
 		yield from self.HoneycombColList
@@ -6897,26 +7262,36 @@
 	def IsotropicColList(self) -> tuple[Isotropic]:
 		return tuple([Isotropic(isotropicCol) for isotropicCol in self._Entity])
 
 	def Count(self) -> int:
 		return self._Entity.Count()
 
 	def Get(self, materialName: str) -> Isotropic:
+		'''
+		Look up an Isotropic material by its name.
+		'''
 		return Isotropic(self._Entity.Get(materialName))
 
 	def Contains(self, materialName: str) -> bool:
+		'''
+		Check if an isotropic material exists in this collection.
+		'''
 		return self._Entity.Contains(materialName)
 
 	def Create(self, materialFamilyName: str, density: float, newMaterialName: str = None, femId: int = None) -> Isotropic:
 		return Isotropic(self._Entity.Create(materialFamilyName, density, newMaterialName, femId))
 
 	def Copy(self, isoToCopyName: str, newMaterialName: str = None, femId: int = None) -> Isotropic:
 		return Isotropic(self._Entity.Copy(isoToCopyName, newMaterialName, femId))
 
 	def Delete(self, materialName: str) -> bool:
+		'''
+		Delete an isotropic material by name.
+            Returns false if the method the material is not found.
+		'''
 		return self._Entity.Delete(materialName)
 
 	def __getitem__(self, index: int):
 		return self.IsotropicColList[index]
 
 	def __iter__(self):
 		yield from self.IsotropicColList
@@ -6967,47 +7342,69 @@
 	def LaminateColList(self) -> tuple[Laminate]:
 		return tuple([Laminate(laminateCol) for laminateCol in self._Entity])
 
 	def Count(self) -> int:
 		return self._Entity.Count()
 
 	def Get(self, laminateName: str) -> LaminateBase:
+		'''
+		Look up a Laminate by its name.
+		'''
 		result = self._Entity.Get(laminateName)
 		thisClass = type(result).__name__
 		givenClass = LaminateBase
 		for subclass in LaminateBase.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		return givenClass(result)
+		return givenClass(result) if result is not None else None
 
 	def Contains(self, laminateName: str) -> bool:
 		return self._Entity.Contains(laminateName)
 
 	def CreateLaminate(self, materialFamily: str, laminateName: str = None) -> Laminate:
+		'''
+		Create laminate.
+		'''
 		return Laminate(self._Entity.CreateLaminate(materialFamily, laminateName))
 
 	def CreateStiffenerLaminate(self, materialFamily: str, stiffenerProfile: types.StiffenerProfile, laminateName: str = None) -> StiffenerLaminate:
+		'''
+		Create a stiffener laminate.
+		'''
 		return StiffenerLaminate(self._Entity.CreateStiffenerLaminate(materialFamily, _types.StiffenerProfile(stiffenerProfile.value), laminateName))
 
 	def Copy(self, laminateToCopyName: str, newLaminateName: str = None) -> LaminateBase:
+		'''
+		Copy a laminate material by name.
+		'''
 		result = self._Entity.Copy(laminateToCopyName, newLaminateName)
 		thisClass = type(result).__name__
 		givenClass = LaminateBase
 		for subclass in LaminateBase.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		return givenClass(result)
+		return givenClass(result) if result is not None else None
 
 	def Delete(self, name: str) -> bool:
+		'''
+		Delete a laminate material by name.
+            Returns false if the material is not found or removed.
+		'''
 		return self._Entity.Delete(name)
 
 	def GetLaminate(self, name: str) -> Laminate:
+		'''
+		Get a laminate by name.
+		'''
 		return Laminate(self._Entity.GetLaminate(name))
 
 	def GetStiffenerLaminate(self, name: str) -> StiffenerLaminate:
+		'''
+		Get a stiffener laminate by name.
+		'''
 		return StiffenerLaminate(self._Entity.GetStiffenerLaminate(name))
 
 	def __getitem__(self, index: int):
 		return self.LaminateColList[index]
 
 	def __iter__(self):
 		yield from self.LaminateColList
@@ -7024,26 +7421,36 @@
 	def OrthotropicColList(self) -> tuple[Orthotropic]:
 		return tuple([Orthotropic(orthotropicCol) for orthotropicCol in self._Entity])
 
 	def Count(self) -> int:
 		return self._Entity.Count()
 
 	def Get(self, materialName: str) -> Orthotropic:
+		'''
+		Look up an Orthotropic material by its name.
+		'''
 		return Orthotropic(self._Entity.Get(materialName))
 
 	def Contains(self, materialName: str) -> bool:
+		'''
+		Check if an orthotropic material exists in this collection.
+		'''
 		return self._Entity.Contains(materialName)
 
 	def Create(self, materialFamilyName: str, thickness: float, density: float, newMaterialName: str = None, femId: int = None) -> Orthotropic:
 		return Orthotropic(self._Entity.Create(materialFamilyName, thickness, density, newMaterialName, femId))
 
 	def Copy(self, orthoToCopyName: str, newMaterialName: str = None, femId: int = None) -> Orthotropic:
 		return Orthotropic(self._Entity.Copy(orthoToCopyName, newMaterialName, femId))
 
 	def Delete(self, materialName: str) -> bool:
+		'''
+		Delete an orthotropic material by name.
+            Returns false if the method the material is not found.
+		'''
 		return self._Entity.Delete(materialName)
 
 	def __getitem__(self, index: int):
 		return self.OrthotropicColList[index]
 
 	def __iter__(self):
 		yield from self.OrthotropicColList
@@ -7058,14 +7465,17 @@
 		self._CollectedClass = PluginPackage
 
 	@property
 	def PluginPackageColList(self) -> tuple[PluginPackage]:
 		return tuple([PluginPackage(pluginPackageCol) for pluginPackageCol in self._Entity])
 
 	def AddPluginPackage(self, path: str) -> PluginPackage:
+		'''
+		Add a plugin package by path.
+		'''
 		return PluginPackage(self._Entity.AddPluginPackage(path))
 
 	@overload
 	def RemovePluginPackage(self, name: str) -> bool: ...
 
 	@overload
 	def RemovePluginPackage(self, id: int) -> bool: ...
@@ -7165,15 +7575,15 @@
 
 	@property
 	def UnitSystem(self) -> UnitSystem:
 		'''
 		Unit system specified when starting a scripting Application.
 		'''
 		result = self._Entity.UnitSystem
-		return UnitSystem(result) if result is not None else None
+		return UnitSystem[result.ToString()] if result is not None else None
 
 	@property
 	def CompilationDate(self) -> str:
 		return self._Entity.CompilationDate
 
 	@property
 	def DatabasePath(self) -> str:
@@ -7280,23 +7690,44 @@
 		return self._Entity.UserName
 
 	@UserName.setter
 	def UserName(self, value: str) -> None:
 		self._Entity.UserName = value
 
 	def CloseDatabase(self, delay: int = 0) -> None:
+		'''
+		Close the currently open database if one exists.
+		:param delay: Delay closing the connection for this many seconds.
+		'''
 		return self._Entity.CloseDatabase(delay)
 
 	def CopyProject(self, projectId: int, newName: str = None, copyDesignProperties: bool = True, copyAnalysisProperties: bool = True, copyLoadProperties: bool = True, copyWorkingFolder: bool = True) -> ProjectInfo:
+		'''
+		Copy a project
+		:param projectId: Id of the project to copy
+		:param newName: Name for the new project
+		:param copyDesignProperties: Flag indicating whether design properties should be copied in the new project
+		:param copyAnalysisProperties: Flag indicating whether analysis properties should be copied in the new project
+		:param copyLoadProperties: Flag indicating whether load properties should be copied in the new project
+		:param copyWorkingFolder: Flag indicating whether working folder should be copied
+		'''
 		return ProjectInfo(self._Entity.CopyProject(projectId, newName, copyDesignProperties, copyAnalysisProperties, copyLoadProperties, copyWorkingFolder))
 
 	def CreateDatabaseFromTemplate(self, templateName: str, newPath: str) -> None:
+		'''
+		Create a new database.
+		:param templateName: The name of the template to base this database on.
+		:param newPath: The path to the new database.
+		'''
 		return self._Entity.CreateDatabaseFromTemplate(templateName, newPath)
 
 	def CreateProject(self, projectName: str = None) -> ProjectInfo:
+		'''
+		Create a Project.
+		'''
 		return ProjectInfo(self._Entity.CreateProject(projectName))
 
 	def DeleteProject(self, projectName: str) -> ProjectDeletionStatus:
 		return ProjectDeletionStatus[self._Entity.DeleteProject(projectName).ToString()]
 
 	def Dispose(self) -> None:
 		'''
@@ -7308,26 +7739,46 @@
 	def GetAnalyses(self) -> dict[int, AnalysisDefinition]:
 		'''
 		Get all Analysis Definitions in the database.
 		'''
 		return dict[int, AnalysisDefinition](self._Entity.GetAnalyses())
 
 	def Login(self, userName: str, password: str = "") -> None:
+		'''
+		Login to the Scripting API with a specified username and password.
+		:param userName: Username to login with.
+		:param password: Password to log in with
+		'''
 		return self._Entity.Login(userName, password)
 
 	def Migrate(self, databasePath: str) -> str:
+		'''
+		Migrate the database to the latest version.
+		'''
 		return self._Entity.Migrate(databasePath)
 
 	def CheckDatabaseIsUpToDate(self, databasePath: str) -> bool:
+		'''
+		Returns true if the database version matches the version of this scripting API.
+            Otherwise returns false.
+		'''
 		return self._Entity.CheckDatabaseIsUpToDate(databasePath)
 
 	def OpenDatabase(self, databasePath: str) -> None:
+		'''
+		Open a database to manipulate with the API.
+		:param databasePath: File path to the DB.
+		'''
 		return self._Entity.OpenDatabase(databasePath)
 
 	def SelectProject(self, projectName: str) -> Project:
+		'''
+		Select the active project.
+            Activating a project will deactivate the current project (if present).
+		'''
 		return Project(self._Entity.SelectProject(projectName))
 
 
 class JointDesignProperty(DesignProperty):
 	def __init__(self, jointDesignProperty: _api.JointDesignProperty):
 		self._Entity = jointDesignProperty
 
@@ -7341,15 +7792,16 @@
 		return self._Entity.MaterialId
 
 	@property
 	def MaterialType(self) -> types.MaterialType:
 		'''
 		Represents a material's type.
 		'''
-		return types.MaterialType[self._Entity.MaterialType.ToString()]
+		result = self._Entity.MaterialType
+		return types.MaterialType[result.ToString()] if result is not None else None
 
 
 class SizingMaterialCol(IdEntityCol[SizingMaterial]):
 	def __init__(self, sizingMaterialCol: _api.SizingMaterialCol):
 		self._Entity = sizingMaterialCol
 		self._CollectedClass = SizingMaterial
 
@@ -7441,15 +7893,16 @@
 
 	@property
 	def DesignId(self) -> int:
 		return self._Entity.DesignId
 
 	@property
 	def FamilyId(self) -> types.BeamPanelFamily:
-		return types.BeamPanelFamily[self._Entity.FamilyId.ToString()]
+		result = self._Entity.FamilyId
+		return types.BeamPanelFamily[result.ToString()] if result is not None else None
 
 	@property
 	def ConceptId(self) -> int:
 		return self._Entity.ConceptId
 
 	@property
 	def VariableId(self) -> int:
@@ -7477,15 +7930,16 @@
 
 	@property
 	def PlyStepSize(self) -> int:
 		return self._Entity.PlyStepSize
 
 	@property
 	def InputMode(self) -> types.VariableInputMode:
-		return types.VariableInputMode[self._Entity.InputMode.ToString()]
+		result = self._Entity.InputMode
+		return types.VariableInputMode[result.ToString()] if result is not None else None
 
 	@property
 	def SizingMaterials(self) -> SizingMaterialCol:
 		result = self._Entity.SizingMaterials
 		return SizingMaterialCol(result) if result is not None else None
 
 	@property
@@ -7494,15 +7948,16 @@
 
 	@property
 	def AnalysisMaterial(self) -> str:
 		return self._Entity.AnalysisMaterial
 
 	@property
 	def AnalysisMaterialType(self) -> types.MaterialType:
-		return types.MaterialType[self._Entity.AnalysisMaterialType.ToString()]
+		result = self._Entity.AnalysisMaterialType
+		return types.MaterialType[result.ToString()] if result is not None else None
 
 	@MinBound.setter
 	def MinBound(self, value: float) -> None:
 		self._Entity.MinBound = value
 
 	@MaxBound.setter
 	def MaxBound(self, value: float) -> None:
@@ -7553,15 +8008,16 @@
 		return self._Entity.ConstraintValue
 
 	@property
 	def ToolingSelectionType(self) -> types.ToolingSelectionType:
 		'''
 		Defines which selection a given tooling constraint is currently set to.
 		'''
-		return types.ToolingSelectionType[self._Entity.ToolingSelectionType.ToString()]
+		result = self._Entity.ToolingSelectionType
+		return types.ToolingSelectionType[result.ToString()] if result is not None else None
 
 	def SetToAnyValue(self) -> None:
 		return self._Entity.SetToAnyValue()
 
 	def SetToInequality(self, value: float) -> None:
 		return self._Entity.SetToInequality(value)
 
@@ -7578,14 +8034,17 @@
 		self._CollectedClass = ZoneOverride
 
 	@property
 	def ZoneOverrideColList(self) -> tuple[ZoneOverride]:
 		return tuple([ZoneOverride(zoneOverrideCol) for zoneOverrideCol in self._Entity])
 
 	def Get(self, zoneNumber: int) -> ZoneOverride:
+		'''
+		Get override for a zone by the zone number
+		'''
 		return ZoneOverride(self._Entity.Get(zoneNumber))
 
 	def __getitem__(self, index: int):
 		return self.ZoneOverrideColList[index]
 
 	def __iter__(self):
 		yield from self.ZoneOverrideColList
@@ -7600,15 +8059,16 @@
             Min, max, steps, materials.
 	'''
 	def __init__(self, designVariable: _api.DesignVariable):
 		self._Entity = designVariable
 
 	@property
 	def VariableParameter(self) -> types.VariableParameter:
-		return types.VariableParameter[self._Entity.VariableParameter.ToString()]
+		result = self._Entity.VariableParameter
+		return types.VariableParameter[result.ToString()] if result is not None else None
 
 	@property
 	def AllowMaterials(self) -> bool:
 		return self._Entity.AllowMaterials
 
 	@property
 	def Max(self) -> float:
@@ -7632,19 +8092,21 @@
 
 	@property
 	def AnalysisMaterial(self) -> str:
 		return self._Entity.AnalysisMaterial
 
 	@property
 	def AnalysisMaterialType(self) -> types.MaterialType:
-		return types.MaterialType[self._Entity.AnalysisMaterialType.ToString()]
+		result = self._Entity.AnalysisMaterialType
+		return types.MaterialType[result.ToString()] if result is not None else None
 
 	@property
 	def SizingMaterialType(self) -> types.MaterialType:
-		return types.MaterialType[self._Entity.SizingMaterialType.ToString()]
+		result = self._Entity.SizingMaterialType
+		return types.MaterialType[result.ToString()] if result is not None else None
 
 	@property
 	def AnalysisValue(self) -> float:
 		return self._Entity.AnalysisValue
 
 	@property
 	def Overrides(self) -> ZoneOverrideCol:
@@ -7692,15 +8154,15 @@
 		materialIdsEnumerable = IEnumerable(materialIdsList)
 		return self._Entity.RemoveSizingMaterials(materialIds if materialIds is None else materialIdsEnumerable)
 
 	def GetAnalysisMaterial(self) -> int:
 		'''
 		Get the material used for analysis, if it exists.
 		'''
-		return self._Entity.GetAnalysisMaterial()
+		return int(self._Entity.GetAnalysisMaterial())
 
 	def RemoveAnalysisMaterial(self) -> None:
 		'''
 		Remove the analysis material assigned to this variable.
 		'''
 		return self._Entity.RemoveAnalysisMaterial()
 
@@ -7794,23 +8256,25 @@
 
 class ZoneDesignProperty(DesignProperty):
 	def __init__(self, zoneDesignProperty: _api.ZoneDesignProperty):
 		self._Entity = zoneDesignProperty
 
 	@property
 	def FamilyId(self) -> types.BeamPanelFamily:
-		return types.BeamPanelFamily[self._Entity.FamilyId.ToString()]
+		result = self._Entity.FamilyId
+		return types.BeamPanelFamily[result.ToString()] if result is not None else None
 
 	@property
 	def ConceptId(self) -> int:
 		return self._Entity.ConceptId
 
 	@property
 	def FamilyConceptUID(self) -> types.FamilyConceptUID:
-		return types.FamilyConceptUID[self._Entity.FamilyConceptUID.ToString()]
+		result = self._Entity.FamilyConceptUID
+		return types.FamilyConceptUID[result.ToString()] if result is not None else None
 
 	@property
 	def ToolingConstraints(self) -> ToolingConstraintCol:
 		result = self._Entity.ToolingConstraints
 		return ToolingConstraintCol(result) if result is not None else None
 
 	@property
@@ -7844,15 +8308,16 @@
 
 	@property
 	def LoadPropertyId(self) -> int:
 		return self._Entity.LoadPropertyId
 
 	@property
 	def Type(self) -> types.LoadSetType:
-		return types.LoadSetType[self._Entity.Type.ToString()]
+		result = self._Entity.Type
+		return types.LoadSetType[result.ToString()] if result is not None else None
 
 	@property
 	def ReferenceTemperature(self) -> float:
 		return self._Entity.ReferenceTemperature
 
 	@property
 	def PressureOrTemperature(self) -> float:
@@ -7953,14 +8418,17 @@
 
 
 class LoadPropertyUserFeaBeamRow(LoadPropertyUserBeamRow):
 	def __init__(self, loadPropertyUserFeaBeamRow: _api.LoadPropertyUserFeaBeamRow):
 		self._Entity = loadPropertyUserFeaBeamRow
 
 	def SetName(self, name: str) -> None:
+		'''
+		Set the name for the scenario
+		'''
 		return self._Entity.SetName(name)
 
 
 class LoadPropertyUserFeaBeamRowBulkUpdater(LoadPropertyUserRowBulkUpdater):
 	def __init__(self, loadPropertyUserFeaBeamRowBulkUpdater: _api.LoadPropertyUserFeaBeamRowBulkUpdater):
 		self._Entity = loadPropertyUserFeaBeamRowBulkUpdater
 
@@ -8043,14 +8511,17 @@
 
 
 class LoadPropertyUserFeaJointRow(LoadPropertyUserPanelJointRow):
 	def __init__(self, loadPropertyUserFeaJointRow: _api.LoadPropertyUserFeaJointRow):
 		self._Entity = loadPropertyUserFeaJointRow
 
 	def SetName(self, name: str) -> None:
+		'''
+		Set the name for the scenario
+		'''
 		return self._Entity.SetName(name)
 
 
 class LoadPropertyUserFeaJointRowBulkUpdater(LoadPropertyUserRowBulkUpdater):
 	def __init__(self, loadPropertyUserFeaJointRowBulkUpdater: _api.LoadPropertyUserFeaJointRowBulkUpdater):
 		self._Entity = loadPropertyUserFeaJointRowBulkUpdater
 
@@ -8064,14 +8535,17 @@
 
 
 class LoadPropertyUserFeaPanelRow(LoadPropertyUserPanelJointRow):
 	def __init__(self, loadPropertyUserFeaPanelRow: _api.LoadPropertyUserFeaPanelRow):
 		self._Entity = loadPropertyUserFeaPanelRow
 
 	def SetName(self, name: str) -> None:
+		'''
+		Set the name for the scenario
+		'''
 		return self._Entity.SetName(name)
 
 
 class LoadPropertyUserFeaPanelRowBulkUpdater(LoadPropertyUserRowBulkUpdater):
 	def __init__(self, loadPropertyUserFeaPanelRowBulkUpdater: _api.LoadPropertyUserFeaPanelRowBulkUpdater):
 		self._Entity = loadPropertyUserFeaPanelRowBulkUpdater
 
@@ -8118,43 +8592,51 @@
 
 	@property
 	def Torque(self) -> float:
 		return self._Entity.Torque
 
 	@property
 	def M1AType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.M1AType.ToString()]
+		result = self._Entity.M1AType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def M2AType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.M2AType.ToString()]
+		result = self._Entity.M2AType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def M1BType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.M1BType.ToString()]
+		result = self._Entity.M1BType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def M2BType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.M2BType.ToString()]
+		result = self._Entity.M2BType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def V1Type(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.V1Type.ToString()]
+		result = self._Entity.V1Type
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def V2Type(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.V2Type.ToString()]
+		result = self._Entity.V2Type
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def AxialType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.AxialType.ToString()]
+		result = self._Entity.AxialType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def TorqueType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.TorqueType.ToString()]
+		result = self._Entity.TorqueType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@M1A.setter
 	def M1A(self, value: float) -> None:
 		self._Entity.M1A = value
 
 	@M2A.setter
 	def M2A(self, value: float) -> None:
@@ -8232,43 +8714,51 @@
 
 	@property
 	def Qy(self) -> float:
 		return self._Entity.Qy
 
 	@property
 	def NxType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.NxType.ToString()]
+		result = self._Entity.NxType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def NyType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.NyType.ToString()]
+		result = self._Entity.NyType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def NxyType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.NxyType.ToString()]
+		result = self._Entity.NxyType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def MxType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.MxType.ToString()]
+		result = self._Entity.MxType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def MyType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.MyType.ToString()]
+		result = self._Entity.MyType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def MxyType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.MxyType.ToString()]
+		result = self._Entity.MxyType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def QxType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.QxType.ToString()]
+		result = self._Entity.QxType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def QyType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.QyType.ToString()]
+		result = self._Entity.QyType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@Nx.setter
 	def Nx(self, value: float) -> None:
 		self._Entity.Nx = value
 
 	@Ny.setter
 	def Ny(self, value: float) -> None:
@@ -8463,15 +8953,16 @@
 
 class LoadPropertyAverage(LoadPropertyFea):
 	def __init__(self, loadPropertyAverage: _api.LoadPropertyAverage):
 		self._Entity = loadPropertyAverage
 
 	@property
 	def ElementType(self) -> types.LoadPropertyAverageElementType:
-		return types.LoadPropertyAverageElementType[self._Entity.ElementType.ToString()]
+		result = self._Entity.ElementType
+		return types.LoadPropertyAverageElementType[result.ToString()] if result is not None else None
 
 	@ElementType.setter
 	def ElementType(self, value: types.LoadPropertyAverageElementType) -> None:
 		self._Entity.ElementType = _types.LoadPropertyAverageElementType(value.value)
 
 
 class LoadPropertyElementBased(LoadPropertyFea):
@@ -8494,15 +8985,16 @@
 
 class LoadPropertyPeakLoad(LoadPropertyFea):
 	def __init__(self, loadPropertyPeakLoad: _api.LoadPropertyPeakLoad):
 		self._Entity = loadPropertyPeakLoad
 
 	@property
 	def ElementScope(self) -> types.LoadPropertyPeakElementScope:
-		return types.LoadPropertyPeakElementScope[self._Entity.ElementScope.ToString()]
+		result = self._Entity.ElementScope
+		return types.LoadPropertyPeakElementScope[result.ToString()] if result is not None else None
 
 	@ElementScope.setter
 	def ElementScope(self, value: types.LoadPropertyPeakElementScope) -> None:
 		self._Entity.ElementScope = _types.LoadPropertyPeakElementScope(value.value)
 
 
 class LoadPropertyStatistical(LoadPropertyFea):
@@ -8531,14 +9023,17 @@
 		givenClass = T
 		for subclass in T.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
 		return tuple([givenClass(loadPropertyUserFeaRowCol) for loadPropertyUserFeaRowCol in self._Entity])
 
 	def AddScenario(self, name: str = None) -> T:
+		'''
+		Adds a load scenario with default values.
+		'''
 		return self._Entity.AddScenario(name)
 
 	@overload
 	def DeleteScenario(self, scenarioId: int) -> bool: ...
 
 	@overload
 	def DeleteScenario(self, scenarioName: str) -> bool: ...
@@ -8750,123 +9245,161 @@
 
 	@property
 	def UserFeaRows(self) -> LoadPropertyUserFeaPanelRowCol:
 		result = self._Entity.UserFeaRows
 		return LoadPropertyUserFeaPanelRowCol(result) if result is not None else None
 
 	def SetIsZeroCurvature(self, isZeroCurvature: bool) -> None:
+		'''
+		Is there an enum for this?
+		'''
 		return self._Entity.SetIsZeroCurvature(isZeroCurvature)
 
 
 class LoadPropertyUserGeneralDoubleRow(IdNameEntity):
 	def __init__(self, loadPropertyUserGeneralDoubleRow: _api.LoadPropertyUserGeneralDoubleRow):
 		self._Entity = loadPropertyUserGeneralDoubleRow
 
 	@property
 	def MechanicalRow(self) -> LoadPropertyUserRow:
-		thisClass = type(self._Entity.MechanicalRow).__name__
+		result = self._Entity.MechanicalRow
+		thisClass = type(result).__name__
 		givenClass = LoadPropertyUserRow
 		for subclass in LoadPropertyUserRow.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		result = self._Entity.MechanicalRow
 		return givenClass(result) if result is not None else None
 
 	@property
 	def ThermalRow(self) -> LoadPropertyUserRow:
-		thisClass = type(self._Entity.ThermalRow).__name__
+		result = self._Entity.ThermalRow
+		thisClass = type(result).__name__
 		givenClass = LoadPropertyUserRow
 		for subclass in LoadPropertyUserRow.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		result = self._Entity.ThermalRow
 		return givenClass(result) if result is not None else None
 
 	def SetName(self, name: str) -> None:
+		'''
+		Update name for the scenario
+		'''
 		return self._Entity.SetName(name)
 
 
 class LoadPropertyUserGeneralBeamDoubleRow(LoadPropertyUserGeneralDoubleRow):
 	def __init__(self, loadPropertyUserGeneralBeamDoubleRow: _api.LoadPropertyUserGeneralBeamDoubleRow):
 		self._Entity = loadPropertyUserGeneralBeamDoubleRow
 
 	@property
 	def MechanicalRow(self) -> LoadPropertyUserRow:
-		thisClass = type(self._Entity.MechanicalRow).__name__
+		result = self._Entity.MechanicalRow
+		thisClass = type(result).__name__
 		givenClass = LoadPropertyUserRow
 		for subclass in LoadPropertyUserRow.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		result = self._Entity.MechanicalRow
 		return givenClass(result) if result is not None else None
 
 	@property
 	def ThermalRow(self) -> LoadPropertyUserRow:
-		thisClass = type(self._Entity.ThermalRow).__name__
+		result = self._Entity.ThermalRow
+		thisClass = type(result).__name__
 		givenClass = LoadPropertyUserRow
 		for subclass in LoadPropertyUserRow.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		result = self._Entity.ThermalRow
 		return givenClass(result) if result is not None else None
 
 	@property
 	def M1AType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.M1AType.ToString()]
+		result = self._Entity.M1AType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def M2AType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.M2AType.ToString()]
+		result = self._Entity.M2AType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def M1BType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.M1BType.ToString()]
+		result = self._Entity.M1BType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def M2BType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.M2BType.ToString()]
+		result = self._Entity.M2BType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def V1Type(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.V1Type.ToString()]
+		result = self._Entity.V1Type
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def V2Type(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.V2Type.ToString()]
+		result = self._Entity.V2Type
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def AxialType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.AxialType.ToString()]
+		result = self._Entity.AxialType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def TorqueType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.TorqueType.ToString()]
+		result = self._Entity.TorqueType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	def SetM1AType(self, type: types.BoundaryConditionType) -> None:
+		'''
+		Set M1A type for the scenario
+		'''
 		return self._Entity.SetM1AType(_types.BoundaryConditionType(type.value))
 
 	def SetM2AType(self, type: types.BoundaryConditionType) -> None:
+		'''
+		Set M2A type for the scenario
+		'''
 		return self._Entity.SetM2AType(_types.BoundaryConditionType(type.value))
 
 	def SetM1BType(self, type: types.BoundaryConditionType) -> None:
+		'''
+		Set M1B type for the scenario
+		'''
 		return self._Entity.SetM1BType(_types.BoundaryConditionType(type.value))
 
 	def SetM2BType(self, type: types.BoundaryConditionType) -> None:
+		'''
+		Set M2B type for the scenario
+		'''
 		return self._Entity.SetM2BType(_types.BoundaryConditionType(type.value))
 
 	def SetV1Type(self, type: types.BoundaryConditionType) -> None:
+		'''
+		Set V1 type for the scenario
+		'''
 		return self._Entity.SetV1Type(_types.BoundaryConditionType(type.value))
 
 	def SetV2Type(self, type: types.BoundaryConditionType) -> None:
+		'''
+		Set V2 type for the scenario
+		'''
 		return self._Entity.SetV2Type(_types.BoundaryConditionType(type.value))
 
 	def SetAxialType(self, type: types.BoundaryConditionType) -> None:
+		'''
+		Set Axial type for the scenario
+		'''
 		return self._Entity.SetAxialType(_types.BoundaryConditionType(type.value))
 
 	def SetTorqueType(self, type: types.BoundaryConditionType) -> None:
+		'''
+		Set torque type for the scenario
+		'''
 		return self._Entity.SetTorqueType(_types.BoundaryConditionType(type.value))
 
 
 class LoadPropertyUserGeneralRowCol(IdNameEntityCol, Generic[T]):
 	def __init__(self, loadPropertyUserGeneralRowCol: _api.LoadPropertyUserGeneralRowCol):
 		self._Entity = loadPropertyUserGeneralRowCol
 		self._CollectedClass = T
@@ -8879,14 +9412,17 @@
 		givenClass = T
 		for subclass in T.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
 		return tuple([givenClass(loadPropertyUserGeneralRowCol) for loadPropertyUserGeneralRowCol in self._Entity])
 
 	def AddScenario(self, name: str = None) -> T:
+		'''
+		Add scenario.
+		'''
 		return self._Entity.AddScenario(name)
 
 	@overload
 	def DeleteScenario(self, scenarioId: int) -> bool: ...
 
 	@overload
 	def DeleteScenario(self, scenarioName: str) -> bool: ...
@@ -9105,14 +9641,17 @@
 	def AddScenario(self) -> None:
 		'''
 		Adds a load scenario with default values
 		'''
 		return self._Entity.AddScenario()
 
 	def DeleteScenario(self, scenarioId: int) -> bool:
+		'''
+		Delete a load scenario by id
+		'''
 		return self._Entity.DeleteScenario(scenarioId)
 
 	def __getitem__(self, index: int):
 		return self.LoadPropertyUserGeneralBoltedRowColList[index]
 
 	def __iter__(self):
 		yield from self.LoadPropertyUserGeneralBoltedRowColList
@@ -9137,35 +9676,40 @@
 
 	@property
 	def LoadPropertyId(self) -> int:
 		return self._Entity.LoadPropertyId
 
 	@property
 	def JointConceptId(self) -> types.JointConceptId:
-		return types.JointConceptId[self._Entity.JointConceptId.ToString()]
+		result = self._Entity.JointConceptId
+		return types.JointConceptId[result.ToString()] if result is not None else None
 
 	@property
 	def BondedBcId(self) -> int:
 		return self._Entity.BondedBcId
 
 	@property
 	def AxialType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.AxialType.ToString()]
+		result = self._Entity.AxialType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def MomentType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.MomentType.ToString()]
+		result = self._Entity.MomentType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def TransverseType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.TransverseType.ToString()]
+		result = self._Entity.TransverseType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def ShearType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.ShearType.ToString()]
+		result = self._Entity.ShearType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def Axial(self) -> float:
 		return self._Entity.Axial
 
 	@property
 	def Moment(self) -> float:
@@ -9245,15 +9789,16 @@
 
 	@property
 	def LoadPropertyId(self) -> int:
 		return self._Entity.LoadPropertyId
 
 	@property
 	def JConceptId(self) -> types.JointConceptId:
-		return types.JointConceptId[self._Entity.JConceptId.ToString()]
+		result = self._Entity.JConceptId
+		return types.JointConceptId[result.ToString()] if result is not None else None
 
 	@property
 	def Ex(self) -> float:
 		return self._Entity.Ex
 
 	@property
 	def Kx(self) -> float:
@@ -9300,86 +9845,118 @@
 
 class LoadPropertyUserGeneralPanelDoubleRow(LoadPropertyUserGeneralDoubleRow):
 	def __init__(self, loadPropertyUserGeneralPanelDoubleRow: _api.LoadPropertyUserGeneralPanelDoubleRow):
 		self._Entity = loadPropertyUserGeneralPanelDoubleRow
 
 	@property
 	def MechanicalRow(self) -> LoadPropertyUserRow:
-		thisClass = type(self._Entity.MechanicalRow).__name__
+		result = self._Entity.MechanicalRow
+		thisClass = type(result).__name__
 		givenClass = LoadPropertyUserRow
 		for subclass in LoadPropertyUserRow.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		result = self._Entity.MechanicalRow
 		return givenClass(result) if result is not None else None
 
 	@property
 	def ThermalRow(self) -> LoadPropertyUserRow:
-		thisClass = type(self._Entity.ThermalRow).__name__
+		result = self._Entity.ThermalRow
+		thisClass = type(result).__name__
 		givenClass = LoadPropertyUserRow
 		for subclass in LoadPropertyUserRow.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
-		result = self._Entity.ThermalRow
 		return givenClass(result) if result is not None else None
 
 	@property
 	def NxType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.NxType.ToString()]
+		result = self._Entity.NxType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def NyType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.NyType.ToString()]
+		result = self._Entity.NyType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def NxyType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.NxyType.ToString()]
+		result = self._Entity.NxyType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def MxType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.MxType.ToString()]
+		result = self._Entity.MxType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def MyType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.MyType.ToString()]
+		result = self._Entity.MyType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def MxyType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.MxyType.ToString()]
+		result = self._Entity.MxyType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def QxType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.QxType.ToString()]
+		result = self._Entity.QxType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	@property
 	def QyType(self) -> types.BoundaryConditionType:
-		return types.BoundaryConditionType[self._Entity.QyType.ToString()]
+		result = self._Entity.QyType
+		return types.BoundaryConditionType[result.ToString()] if result is not None else None
 
 	def SetNxType(self, type: types.BoundaryConditionType) -> None:
+		'''
+		Set Nx type for the scenario
+		'''
 		return self._Entity.SetNxType(_types.BoundaryConditionType(type.value))
 
 	def SetNyType(self, type: types.BoundaryConditionType) -> None:
+		'''
+		Set Ny type for the scenario
+		'''
 		return self._Entity.SetNyType(_types.BoundaryConditionType(type.value))
 
 	def SetNxyType(self, type: types.BoundaryConditionType) -> None:
+		'''
+		Set Nxy type for the scenario
+		'''
 		return self._Entity.SetNxyType(_types.BoundaryConditionType(type.value))
 
 	def SetMxType(self, type: types.BoundaryConditionType) -> None:
+		'''
+		Set Mx type for the scenario
+		'''
 		return self._Entity.SetMxType(_types.BoundaryConditionType(type.value))
 
 	def SetMyType(self, type: types.BoundaryConditionType) -> None:
+		'''
+		Set My type for the scenario
+		'''
 		return self._Entity.SetMyType(_types.BoundaryConditionType(type.value))
 
 	def SetMxyType(self, type: types.BoundaryConditionType) -> None:
+		'''
+		Set Mxy type for the scenario
+		'''
 		return self._Entity.SetMxyType(_types.BoundaryConditionType(type.value))
 
 	def SetQxType(self, type: types.BoundaryConditionType) -> None:
+		'''
+		Set Qx type for the scenario
+		'''
 		return self._Entity.SetQxType(_types.BoundaryConditionType(type.value))
 
 	def SetQyType(self, type: types.BoundaryConditionType) -> None:
+		'''
+		Set Qy type for the scenario
+		'''
 		return self._Entity.SetQyType(_types.BoundaryConditionType(type.value))
 
 
 class LoadPropertyUserGeneralPanelRowCol(LoadPropertyUserGeneralRowCol[LoadPropertyUserGeneralPanelDoubleRow]):
 	def __init__(self, loadPropertyUserGeneralPanelRowCol: _api.LoadPropertyUserGeneralPanelRowCol):
 		self._Entity = loadPropertyUserGeneralPanelRowCol
 		self._CollectedClass = LoadPropertyUserGeneralPanelDoubleRow
@@ -9442,24 +10019,28 @@
 		return self._Entity.IsIncludingThermal
 
 	@IsIncludingThermal.setter
 	def IsIncludingThermal(self, value: bool) -> None:
 		self._Entity.IsIncludingThermal = value
 
 	def SetIsZeroCurvature(self, isZeroCurvature: bool) -> None:
+		'''
+		Is there an enum for this?
+		'''
 		return self._Entity.SetIsZeroCurvature(isZeroCurvature)
 
 
 class JointSelectionDesignResult(JointDesignResult):
 	def __init__(self, jointSelectionDesignResult: _api.JointSelectionDesignResult):
 		self._Entity = jointSelectionDesignResult
 
 	@property
 	def JointSelectionId(self) -> types.JointSelectionId:
-		return types.JointSelectionId[self._Entity.JointSelectionId.ToString()]
+		result = self._Entity.JointSelectionId
+		return types.JointSelectionId[result.ToString()] if result is not None else None
 
 
 class JointFastenerDesignResult(JointSelectionDesignResult):
 	def __init__(self, jointFastenerDesignResult: _api.JointFastenerDesignResult):
 		self._Entity = jointFastenerDesignResult
 
 	@property
@@ -9480,24 +10061,26 @@
 		return self._Entity.MaterialId
 
 	@property
 	def MaterialType(self) -> types.MaterialType:
 		'''
 		Represents a material's type.
 		'''
-		return types.MaterialType[self._Entity.MaterialType.ToString()]
+		result = self._Entity.MaterialType
+		return types.MaterialType[result.ToString()] if result is not None else None
 
 
 class JointRangeDesignResult(JointDesignResult):
 	def __init__(self, jointRangeDesignResult: _api.JointRangeDesignResult):
 		self._Entity = jointRangeDesignResult
 
 	@property
 	def JointRangeId(self) -> types.JointRangeId:
-		return types.JointRangeId[self._Entity.JointRangeId.ToString()]
+		result = self._Entity.JointRangeId
+		return types.JointRangeId[result.ToString()] if result is not None else None
 
 	@property
 	def Value(self) -> float:
 		return self._Entity.Value
 
 
 class JointRivetDesignResult(JointSelectionDesignResult):
@@ -9517,14 +10100,21 @@
 	'''
 	Represents HyperX's execution environment (where HyperX is installed).
 	'''
 	def __init__(self, environment: _api.Environment):
 		self._Entity = environment
 
 	def SetLocation(location: str) -> None:
+		'''
+		Set the directory location of the HyperX binaries.
+            * This method is *not* required for Python and IronPython client application.
+            * This method is required for C# and VB.NET clients as these applications
+              need HyperX.Scripting.dll alongside its binaries.
+		:param location: Path to the binaries.
+		'''
 		return _api.Environment.SetLocation(location)
 
 	def Initialize() -> None:
 		'''
 		Initialize the HyperX scripting environment.
 		'''
 		return _api.Environment.Initialize()
@@ -9581,15 +10171,16 @@
 		return self._Entity.PlyMaterialId
 
 	@property
 	def PlyMaterialType(self) -> types.MaterialType:
 		'''
 		Represents a material's type.
 		'''
-		return types.MaterialType[self._Entity.PlyMaterialType.ToString()]
+		result = self._Entity.PlyMaterialType
+		return types.MaterialType[result.ToString()] if result is not None else None
 
 	@property
 	def Angle(self) -> float:
 		return self._Entity.Angle
 
 	@property
 	def Thickness(self) -> float:
@@ -9613,15 +10204,16 @@
 
 	@property
 	def DisplaySequenceId(self) -> int:
 		return self._Entity.DisplaySequenceId
 
 	@property
 	def PlyStiffenerSubType(self) -> types.PlyStiffenerSubType:
-		return types.PlyStiffenerSubType[self._Entity.PlyStiffenerSubType.ToString()]
+		result = self._Entity.PlyStiffenerSubType
+		return types.PlyStiffenerSubType[result.ToString()] if result is not None else None
 
 	@property
 	def Object1(self) -> bool:
 		return self._Entity.Object1
 
 	@property
 	def Object2(self) -> bool:
@@ -9652,17 +10244,23 @@
 		return self._Entity.IsInWeb
 
 	@property
 	def IsInCap(self) -> bool:
 		return self._Entity.IsInCap
 
 	def SetMaterial(self, matId: int) -> bool:
+		'''
+		Sets the material of a ply to the matId. This includes: PlyMaterialId and PlyMaterialType, and updates Thickness and IsFabric
+		'''
 		return self._Entity.SetMaterial(matId)
 
 	def SetAngle(self, angle: float) -> bool:
+		'''
+		Sets the angle of a ply
+		'''
 		return self._Entity.SetAngle(angle)
 
 
 class Beam(Zone):
 	def __init__(self, beam: _api.Beam):
 		self._Entity = beam
 
@@ -9680,15 +10278,16 @@
 
 	@property
 	def K2(self) -> float:
 		return self._Entity.K2
 
 	@property
 	def ReferencePlane(self) -> types.ReferencePlaneBeam:
-		return types.ReferencePlaneBeam[self._Entity.ReferencePlane.ToString()]
+		result = self._Entity.ReferencePlane
+		return types.ReferencePlaneBeam[result.ToString()] if result is not None else None
 
 	@Phi.setter
 	def Phi(self, value: float) -> None:
 		self._Entity.Phi = value
 
 	@K1.setter
 	def K1(self, value: float) -> None:
@@ -9727,15 +10326,16 @@
 
 	@property
 	def Area(self) -> float:
 		return self._Entity.Area
 
 	@property
 	def ReferencePlane(self) -> types.ReferencePlanePanel:
-		return types.ReferencePlanePanel[self._Entity.ReferencePlane.ToString()]
+		result = self._Entity.ReferencePlane
+		return types.ReferencePlanePanel[result.ToString()] if result is not None else None
 
 	@property
 	def AddedOffset(self) -> float:
 		return self._Entity.AddedOffset
 
 	@property
 	def YSpan(self) -> float:
@@ -9751,15 +10351,16 @@
 
 	@property
 	def IsFullCylinder(self) -> bool:
 		return self._Entity.IsFullCylinder
 
 	@property
 	def BucklingMode(self) -> types.ZoneBucklingMode:
-		return types.ZoneBucklingMode[self._Entity.BucklingMode.ToString()]
+		result = self._Entity.BucklingMode
+		return types.ZoneBucklingMode[result.ToString()] if result is not None else None
 
 	@property
 	def PerformLocalPostbuckling(self) -> bool:
 		return self._Entity.PerformLocalPostbuckling
 
 	@property
 	def A11Required(self) -> float:
```

## hyperx/api/types/__init__.py

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 from ...library import _api, _types
 
 from typing import TypeVar, Generic, overload
 from enum import Enum
 from System.Collections.Generic import List, IEnumerable, Dictionary, HashSet
 from System.Threading.Tasks import Task
-from System import Guid, DateTime
+from System import Guid, DateTime, Double, String, Nullable
 
 from abc import ABC, abstractmethod
 
 T = TypeVar('T')
 
 
 class AnalysisId(Enum):
@@ -1171,76 +1171,81 @@
 	@property
 	def Message(self) -> str:
 		return self._Entity.Message
 
 	def ToString(self) -> str:
 		return self._Entity.ToString()
 
-	def GetHashCode(self) -> int:
-		return self._Entity.GetHashCode()
-
 	@overload
-	def Equals(self, obj) -> bool: ...
+	def Equals(self, obj: object) -> bool: ...
 
 	@overload
 	def Equals(self, other) -> bool: ...
 
 	def Equals(self, item1 = None) -> bool:
+		if isinstance(item1, object):
+			return self._Entity.Equals(item1)
+
 		if isinstance(item1, SimpleStatus):
 			return self._Entity.Equals(_types.SimpleStatus(item1.value))
 
 		return self._Entity.Equals(item1)
 
 	def __eq__(self, other):
 		return self.Equals(other)
 
 	def __ne__(self, other):
 		return not self.Equals(other)
 
+	def __hash__(self) -> int:
+		return self._Entity.GetHashCode()
+
 
 class DesignLink:
 	def __init__(self, designLink: _types.DesignLink):
 		self._Entity = designLink
 
 	def Create_DesignLink(designId: int, familyId: BeamPanelFamily, conceptId: int, linkedVariableId: int):
 		return DesignLink(_api.DesignLink(designId, _types.BeamPanelFamily(familyId.value), conceptId, linkedVariableId))
 
 	@property
 	def DesignId(self) -> int:
 		return self._Entity.DesignId
 
 	@property
 	def FamilyId(self) -> BeamPanelFamily:
-		return BeamPanelFamily[self._Entity.FamilyId.ToString()]
+		result = self._Entity.FamilyId
+		return BeamPanelFamily[result.ToString()] if result is not None else None
 
 	@property
 	def ConceptId(self) -> int:
 		return self._Entity.ConceptId
 
 	@property
 	def LinkedVariableId(self) -> int:
 		return self._Entity.LinkedVariableId
 
-	def Equals(self, obj) -> bool:
-		return self._Entity.Equals(obj._Entity)
+	def Equals(self, obj: object) -> bool:
+		return self._Entity.Equals(obj)
 
-	def GetHashCode(self) -> int:
+	def __hash__(self) -> int:
 		return self._Entity.GetHashCode()
 
 
 class HyperFeaSolver:
 	def __init__(self, hyperFeaSolver: _types.HyperFeaSolver):
 		self._Entity = hyperFeaSolver
 
 	def Create_HyperFeaSolver(projectModelFormat: ProjectModelFormat, solverPath: str, arguments: str):
 		return HyperFeaSolver(_api.HyperFeaSolver(_types.ProjectModelFormat(projectModelFormat.value), solverPath, arguments))
 
 	@property
 	def ProjectModelFormat(self) -> ProjectModelFormat:
-		return ProjectModelFormat[self._Entity.ProjectModelFormat.ToString()]
+		result = self._Entity.ProjectModelFormat
+		return ProjectModelFormat[result.ToString()] if result is not None else None
 
 	@property
 	def SolverPath(self) -> str:
 		return self._Entity.SolverPath
 
 	@property
 	def Arguments(self) -> str:
```

## hyperx/utils/utils.py

```diff
@@ -1,11 +1,12 @@
 """
 Utility methods.
 """
 
+from __future__ import annotations
 from contextlib import contextmanager
 import os
 import subprocess
 import csv
 from pathlib import Path
 from typing import Any, Generator
 import errno
```

## Comparing `hyperx-2024.1.9.dist-info/METADATA` & `hyperx-2024.1.9.1.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hyperx
-Version: 2024.1.9
+Version: 2024.1.9.1
 Summary: HyperX scripting for Python
 Author-email: Kelly Ann Smith <kellyann.smith@collieraerospace.com>, Noah Prezant <noah.prezant@collieraerospace.com>
 Project-URL: Homepage, https://collieraerospace.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: pythonnet >=3.0.1
 
 # HyperX
 
 A python package for scripting in HyperX. Bridges the gap between the C# scripting API and Python.
```

