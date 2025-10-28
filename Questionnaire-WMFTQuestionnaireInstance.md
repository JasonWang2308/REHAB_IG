# WMFT上肢功能評估問卷 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **WMFT上肢功能評估問卷**

## Questionnaire: WMFT上肢功能評估問卷 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/Questionnaire/WMFTQuestionnaireInstance | *Version*:0.1.0 |
| Active as of 2025-10-28 | *Computable Name*:WMFTQuestionnaire |

 
WMFT上肢功能評評估問卷(Wolf et al., 1995; Whitall, Savin, Harris-Love, & Waller, 2006)，分左右邊各75分 

 
提供標準化的上肢感覺評估工具，用於中風復健評估 

Profile: [評估問卷](StructureDefinition-SPACQuestionnaire.md)

**Structure**

* [LinkID](https://hl7.org/fhir/R4/formats.html#table): WMFTQuestionnaire
  * [Text](https://hl7.org/fhir/R4/formats.html#table): WMFT上肢功能評評估問卷(Wolf et al., 1995; Whitall, Savin, Harris-Love, & Waller, 2006)，分左右邊各75分
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 
  * [Type](https://hl7.org/fhir/R4/formats.html#table): Questionnaire
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): http://example.org/Questionnaire/WMFTQuestionnaireInstance#0.1.0
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)assessment-side-wmft
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 請選擇評估側
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[2 options](#opt-item.assessment-side-wmft)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-group.png)A-timed-joint-segment-movements
  * [Text](https://hl7.org/fhir/R4/formats.html#table): A.定時關節分段動作評估
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [group](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-group)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-I-forearm-to-table-side
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 透過外展肩膀將前臂放在桌子上
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[6 options](#opt-item.A-I-forearm-to-table-side)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-I-forearm-to-box-side
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 將前臂放在一個 25.4 公分高的箱子上，透過肩部外展
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[6 options](#opt-item.A-I-forearm-to-box-side)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-I-extended-elbow-side
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 將手肘伸向一側，越過一張 28 公分長的桌子
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[6 options](#opt-item.A-I-extended-elbow-side)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-I-extended-elbow-to-the-side-with-1lb-weight
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 透過伸展手肘將重量推向桌子對面的外腕關節
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[6 options](#opt-item.A-I-extended-elbow-to-the-side-with-1lb-weight)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-I-hand-to-table-front
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 將手放在桌上
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[6 options](#opt-item.A-I-hand-to-table-front)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-I-hand-to-box-front
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 將手放在桌面上的盒子上
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[6 options](#opt-item.A-I-hand-to-box-front)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-integer.png)A-timed-joint-segment-movements-subscore
  * [Text](https://hl7.org/fhir/R4/formats.html#table): A.定時關節段運動分量表分數
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 0..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [integer](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-integer)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): ![](icon-qi-readonly.png)![](icon-qi-readonly.png)
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-group.png)B-timed-integrative-functional-movements
  * [Text](https://hl7.org/fhir/R4/formats.html#table): B.定時整合功能動作評估
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [group](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-group)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-I-lift-can-front
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 舉起一個罐子，並用圓柱形的抓握方式將其靠近嘴唇
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[6 options](#opt-item.B-I-lift-can-front)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-I-lift-pencil-front
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 使用三爪卡盤抓握來拿起鉛筆
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[6 options](#opt-item.B-I-lift-pencil-front)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-I-pick-up-paper-clip-front
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 用鉗子抓取回形針
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[6 options](#opt-item.B-I-pick-up-paper-clip-front)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-I-stack-checkers-front
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 將棋子堆疊到中心棋子上
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[6 options](#opt-item.B-I-stack-checkers-front)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-I-flip-3-cards-front
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 用鉗子抓握，客戶嘗試翻轉每張卡片
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[6 options](#opt-item.B-I-flip-3-cards-front)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-I-turning-the-key-in-lock-front
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 使用鉗子抓握並保持接觸，將鑰匙向左和向右旋轉 180 度
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[6 options](#opt-item.B-I-turning-the-key-in-lock-front)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-I-fold-towel-front
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 抓住毛巾，縱向折疊，然後用被測試的手將毛巾再次對折
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[6 options](#opt-item.B-I-fold-towel-front)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-I-lift-basket-standing
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 提起一個椅子上 3 磅重的籃子，並將其放在床頭櫃上
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[6 options](#opt-item.B-I-lift-basket-standing)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-integer.png)B-timed-integrative-functional-movements-subscore
  * [Text](https://hl7.org/fhir/R4/formats.html#table): B.定時關節段運動分量表分數
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 0..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [integer](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-integer)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): ![](icon-qi-readonly.png)![](icon-qi-readonly.png)
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-integer.png)C-total-score-WMFT
  * [Text](https://hl7.org/fhir/R4/formats.html#table): C.WMFT總分計算
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [integer](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-integer)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC)Documentation for this format

-------

**Options Sets**

**Answer options for assessment-side-wmft**

* http://snomed.info/sct#24028007 ("患者左側")
* http://snomed.info/sct#7771000 ("患者右側")

**Answer options for A-I-forearm-to-table-side**

* 0
* 1
* 2
* 3
* 4
* 5

**Answer options for A-I-forearm-to-box-side**

* 0
* 1
* 2
* 3
* 4
* 5

**Answer options for A-I-extended-elbow-side**

* 0
* 1
* 2
* 3
* 4
* 5

**Answer options for A-I-extended-elbow-to-the-side-with-1lb-weight**

* 0
* 1
* 2
* 3
* 4
* 5

**Answer options for A-I-hand-to-table-front**

* 0
* 1
* 2
* 3
* 4
* 5

**Answer options for A-I-hand-to-box-front**

* 0
* 1
* 2
* 3
* 4
* 5

**Answer options for B-I-lift-can-front**

* 0
* 1
* 2
* 3
* 4
* 5

**Answer options for B-I-lift-pencil-front**

* 0
* 1
* 2
* 3
* 4
* 5

**Answer options for B-I-pick-up-paper-clip-front**

* 0
* 1
* 2
* 3
* 4
* 5

**Answer options for B-I-stack-checkers-front**

* 0
* 1
* 2
* 3
* 4
* 5

**Answer options for B-I-flip-3-cards-front**

* 0
* 1
* 2
* 3
* 4
* 5

**Answer options for B-I-turning-the-key-in-lock-front**

* 0
* 1
* 2
* 3
* 4
* 5

**Answer options for B-I-fold-towel-front**

* 0
* 1
* 2
* 3
* 4
* 5

**Answer options for B-I-lift-basket-standing**

* 0
* 1
* 2
* 3
* 4
* 5



## Resource Content

```json
{
  "resourceType" : "Questionnaire",
  "id" : "WMFTQuestionnaireInstance",
  "meta" : {
    "profile" : ["http://example.org/StructureDefinition/SPACQuestionnaire"]
  },
  "url" : "http://example.org/Questionnaire/WMFTQuestionnaireInstance",
  "version" : "0.1.0",
  "name" : "WMFTQuestionnaire",
  "title" : "WMFT上肢功能評評估問卷",
  "status" : "active",
  "subjectType" : ["Patient"],
  "date" : "2025-10-28T11:34:57+08:00",
  "publisher" : "Example Publisher",
  "contact" : [
    {
      "name" : "Example Publisher",
      "telecom" : [
        {
          "system" : "url",
          "value" : "http://example.org/example-publisher"
        }
      ]
    }
  ],
  "description" : "WMFT上肢功能評評估問卷(Wolf et al., 1995; Whitall, Savin, Harris-Love, & Waller, 2006)，分左右邊各75分",
  "purpose" : "提供標準化的上肢感覺評估工具，用於中風復健評估",
  "item" : [
    {
      "linkId" : "assessment-side-wmft",
      "text" : "請選擇評估側",
      "type" : "choice",
      "required" : true,
      "answerOption" : [
        {
          "valueCoding" : {
            "system" : "http://snomed.info/sct",
            "code" : "24028007",
            "display" : "患者左側"
          }
        },
        {
          "valueCoding" : {
            "system" : "http://snomed.info/sct",
            "code" : "7771000",
            "display" : "患者右側"
          }
        }
      ]
    },
    {
      "linkId" : "A-timed-joint-segment-movements",
      "text" : "A.定時關節分段動作評估",
      "type" : "group",
      "required" : true,
      "item" : [
        {
          "extension" : [
            {
              "url" : "http://example.org/fhir/TestTimeExtension"
            }
          ],
          "linkId" : "A-I-forearm-to-table-side",
          "text" : "透過外展肩膀將前臂放在桌子上",
          "type" : "choice",
          "required" : true,
          "answerOption" : [
            {
              "valueInteger" : 0
            },
            {
              "valueInteger" : 1
            },
            {
              "valueInteger" : 2
            },
            {
              "valueInteger" : 3
            },
            {
              "valueInteger" : 4
            },
            {
              "valueInteger" : 5
            }
          ]
        },
        {
          "extension" : [
            {
              "url" : "http://example.org/fhir/TestTimeExtension"
            }
          ],
          "linkId" : "A-I-forearm-to-box-side",
          "text" : "將前臂放在一個 25.4 公分高的箱子上，透過肩部外展",
          "type" : "choice",
          "required" : true,
          "answerOption" : [
            {
              "valueInteger" : 0
            },
            {
              "valueInteger" : 1
            },
            {
              "valueInteger" : 2
            },
            {
              "valueInteger" : 3
            },
            {
              "valueInteger" : 4
            },
            {
              "valueInteger" : 5
            }
          ]
        },
        {
          "extension" : [
            {
              "url" : "http://example.org/fhir/TestTimeExtension"
            }
          ],
          "linkId" : "A-I-extended-elbow-side",
          "text" : "將手肘伸向一側，越過一張 28 公分長的桌子",
          "type" : "choice",
          "required" : true,
          "answerOption" : [
            {
              "valueInteger" : 0
            },
            {
              "valueInteger" : 1
            },
            {
              "valueInteger" : 2
            },
            {
              "valueInteger" : 3
            },
            {
              "valueInteger" : 4
            },
            {
              "valueInteger" : 5
            }
          ]
        },
        {
          "extension" : [
            {
              "url" : "http://example.org/fhir/TestTimeExtension"
            }
          ],
          "linkId" : "A-I-extended-elbow-to-the-side-with-1lb-weight",
          "text" : "透過伸展手肘將重量推向桌子對面的外腕關節",
          "type" : "choice",
          "required" : true,
          "answerOption" : [
            {
              "valueInteger" : 0
            },
            {
              "valueInteger" : 1
            },
            {
              "valueInteger" : 2
            },
            {
              "valueInteger" : 3
            },
            {
              "valueInteger" : 4
            },
            {
              "valueInteger" : 5
            }
          ]
        },
        {
          "extension" : [
            {
              "url" : "http://example.org/fhir/TestTimeExtension"
            }
          ],
          "linkId" : "A-I-hand-to-table-front",
          "text" : "將手放在桌上",
          "type" : "choice",
          "required" : true,
          "answerOption" : [
            {
              "valueInteger" : 0
            },
            {
              "valueInteger" : 1
            },
            {
              "valueInteger" : 2
            },
            {
              "valueInteger" : 3
            },
            {
              "valueInteger" : 4
            },
            {
              "valueInteger" : 5
            }
          ]
        },
        {
          "extension" : [
            {
              "url" : "http://example.org/fhir/TestTimeExtension"
            }
          ],
          "linkId" : "A-I-hand-to-box-front",
          "text" : "將手放在桌面上的盒子上",
          "type" : "choice",
          "required" : true,
          "answerOption" : [
            {
              "valueInteger" : 0
            },
            {
              "valueInteger" : 1
            },
            {
              "valueInteger" : 2
            },
            {
              "valueInteger" : 3
            },
            {
              "valueInteger" : 4
            },
            {
              "valueInteger" : 5
            }
          ]
        },
        {
          "extension" : [
            {
              "url" : "http://hl7.org/fhir/uv/sdc/StructureDefinition/sdc-questionnaire-calculatedExpression",
              "valueExpression" : {
                "language" : "text/fhirpath",
                "expression" : "%TimedJointSegmentMovementScore"
              }
            },
            {
              "url" : "http://hl7.org/fhir/uv/sdc/StructureDefinition/sdc-questionnaire-observationExtract",
              "valueBoolean" : true
            }
          ],
          "linkId" : "A-timed-joint-segment-movements-subscore",
          "text" : "A.定時關節段運動分量表分數",
          "type" : "integer",
          "readOnly" : true
        }
      ]
    },
    {
      "linkId" : "B-timed-integrative-functional-movements",
      "text" : "B.定時整合功能動作評估",
      "type" : "group",
      "required" : true,
      "item" : [
        {
          "extension" : [
            {
              "url" : "http://example.org/fhir/TestTimeExtension"
            }
          ],
          "linkId" : "B-I-lift-can-front",
          "text" : "舉起一個罐子，並用圓柱形的抓握方式將其靠近嘴唇",
          "type" : "choice",
          "required" : true,
          "answerOption" : [
            {
              "valueInteger" : 0
            },
            {
              "valueInteger" : 1
            },
            {
              "valueInteger" : 2
            },
            {
              "valueInteger" : 3
            },
            {
              "valueInteger" : 4
            },
            {
              "valueInteger" : 5
            }
          ]
        },
        {
          "extension" : [
            {
              "url" : "http://example.org/fhir/TestTimeExtension"
            }
          ],
          "linkId" : "B-I-lift-pencil-front",
          "text" : "使用三爪卡盤抓握來拿起鉛筆",
          "type" : "choice",
          "required" : true,
          "answerOption" : [
            {
              "valueInteger" : 0
            },
            {
              "valueInteger" : 1
            },
            {
              "valueInteger" : 2
            },
            {
              "valueInteger" : 3
            },
            {
              "valueInteger" : 4
            },
            {
              "valueInteger" : 5
            }
          ]
        },
        {
          "extension" : [
            {
              "url" : "http://example.org/fhir/TestTimeExtension"
            }
          ],
          "linkId" : "B-I-pick-up-paper-clip-front",
          "text" : "用鉗子抓取回形針",
          "type" : "choice",
          "required" : true,
          "answerOption" : [
            {
              "valueInteger" : 0
            },
            {
              "valueInteger" : 1
            },
            {
              "valueInteger" : 2
            },
            {
              "valueInteger" : 3
            },
            {
              "valueInteger" : 4
            },
            {
              "valueInteger" : 5
            }
          ]
        },
        {
          "extension" : [
            {
              "url" : "http://example.org/fhir/TestTimeExtension"
            }
          ],
          "linkId" : "B-I-stack-checkers-front",
          "text" : "將棋子堆疊到中心棋子上",
          "type" : "choice",
          "required" : true,
          "answerOption" : [
            {
              "valueInteger" : 0
            },
            {
              "valueInteger" : 1
            },
            {
              "valueInteger" : 2
            },
            {
              "valueInteger" : 3
            },
            {
              "valueInteger" : 4
            },
            {
              "valueInteger" : 5
            }
          ]
        },
        {
          "extension" : [
            {
              "url" : "http://example.org/fhir/TestTimeExtension"
            }
          ],
          "linkId" : "B-I-flip-3-cards-front",
          "text" : "用鉗子抓握，客戶嘗試翻轉每張卡片",
          "type" : "choice",
          "required" : true,
          "answerOption" : [
            {
              "valueInteger" : 0
            },
            {
              "valueInteger" : 1
            },
            {
              "valueInteger" : 2
            },
            {
              "valueInteger" : 3
            },
            {
              "valueInteger" : 4
            },
            {
              "valueInteger" : 5
            }
          ]
        },
        {
          "extension" : [
            {
              "url" : "http://example.org/fhir/TestTimeExtension"
            }
          ],
          "linkId" : "B-I-turning-the-key-in-lock-front",
          "text" : "使用鉗子抓握並保持接觸，將鑰匙向左和向右旋轉 180 度",
          "type" : "choice",
          "required" : true,
          "answerOption" : [
            {
              "valueInteger" : 0
            },
            {
              "valueInteger" : 1
            },
            {
              "valueInteger" : 2
            },
            {
              "valueInteger" : 3
            },
            {
              "valueInteger" : 4
            },
            {
              "valueInteger" : 5
            }
          ]
        },
        {
          "extension" : [
            {
              "url" : "http://example.org/fhir/TestTimeExtension"
            }
          ],
          "linkId" : "B-I-fold-towel-front",
          "text" : "抓住毛巾，縱向折疊，然後用被測試的手將毛巾再次對折",
          "type" : "choice",
          "required" : true,
          "answerOption" : [
            {
              "valueInteger" : 0
            },
            {
              "valueInteger" : 1
            },
            {
              "valueInteger" : 2
            },
            {
              "valueInteger" : 3
            },
            {
              "valueInteger" : 4
            },
            {
              "valueInteger" : 5
            }
          ]
        },
        {
          "extension" : [
            {
              "url" : "http://example.org/fhir/TestTimeExtension"
            }
          ],
          "linkId" : "B-I-lift-basket-standing",
          "text" : "提起一個椅子上 3 磅重的籃子，並將其放在床頭櫃上",
          "type" : "choice",
          "required" : true,
          "answerOption" : [
            {
              "valueInteger" : 0
            },
            {
              "valueInteger" : 1
            },
            {
              "valueInteger" : 2
            },
            {
              "valueInteger" : 3
            },
            {
              "valueInteger" : 4
            },
            {
              "valueInteger" : 5
            }
          ]
        },
        {
          "extension" : [
            {
              "url" : "http://hl7.org/fhir/uv/sdc/StructureDefinition/sdc-questionnaire-calculatedExpression",
              "valueExpression" : {
                "language" : "text/fhirpath",
                "expression" : "%TimedIntegrativeFunctionalMovementScore"
              }
            },
            {
              "url" : "http://hl7.org/fhir/uv/sdc/StructureDefinition/sdc-questionnaire-observationExtract",
              "valueBoolean" : true
            }
          ],
          "linkId" : "B-timed-integrative-functional-movements-subscore",
          "text" : "B.定時關節段運動分量表分數",
          "type" : "integer",
          "readOnly" : true
        }
      ]
    },
    {
      "extension" : [
        {
          "url" : "http://hl7.org/fhir/uv/sdc/StructureDefinition/sdc-questionnaire-calculatedExpression",
          "valueExpression" : {
            "language" : "text/fhirpath",
            "expression" : "%resource.item.descendants().where(type='choice').answer.valueInteger.sum()"
          }
        },
        {
          "url" : "http://hl7.org/fhir/uv/sdc/StructureDefinition/sdc-questionnaire-observationExtract",
          "valueBoolean" : true
        }
      ],
      "linkId" : "C-total-score-WMFT",
      "text" : "C.WMFT總分計算",
      "type" : "integer",
      "required" : true
    }
  ]
}

```
