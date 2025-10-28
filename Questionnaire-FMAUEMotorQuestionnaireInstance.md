# Fugl-Meyer上肢動作評估問卷 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Fugl-Meyer上肢動作評估問卷**

## Questionnaire: Fugl-Meyer上肢動作評估問卷 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/Questionnaire/FMAUEMotorQuestionnaireInstance | *Version*:0.1.0 |
| Active as of 2025-10-01 | *Computable Name*:FMAUEMotorQuestionnaire |

 
衛福部Fugl-Meyer上肢動作評估問卷，總分66分 

 
提供標準化的上肢動作功能評估工具，用於中風復健評估 

Profile: [評估問卷](StructureDefinition-SPACQuestionnaire.md)

**Structure**

* [LinkID](https://hl7.org/fhir/R4/formats.html#table): FMAUEMotorQuestionnaire
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 衛福部Fugl-Meyer上肢動作評估問卷，總分66分
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 
  * [Type](https://hl7.org/fhir/R4/formats.html#table): Questionnaire
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): http://example.org/Questionnaire/FMAUEMotorQuestionnaireInstance#0.1.0
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)assessment-phase-fmaue-motion
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 請選擇評估階段
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[4 options](#opt-item.assessment-phase-fmaue-motion)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)assessment-side-fmaue-motion
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 請選擇患側
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[2 options](#opt-item.assessment-side-fmaue-motion)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-group.png)A-shoulder-elbow-forearm
  * [Text](https://hl7.org/fhir/R4/formats.html#table): A.肩部/肘部/前臂
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [group](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-group)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-group.png)A-I-FMAUEMotion
  * [Text](https://hl7.org/fhir/R4/formats.html#table): I.反射反應
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [group](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-group)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-I-a-flexors
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 二頭肌或手指屈肌
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[2 options](#opt-item.A-I-a-flexors)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-I-a-extensors
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 三頭肌
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[2 options](#opt-item.A-I-a-extensors)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-group.png)A-II-a-FMAUEMotion
  * [Text](https://hl7.org/fhir/R4/formats.html#table): II.a.屈肌協同動作
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [group](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-group)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-II-a-shoulder-retraction
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 肩部回縮
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.A-II-a-shoulder-retraction)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-II-a-shoulder-elevation
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 肩部抬高
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.A-II-a-shoulder-elevation)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-II-a-shoulder-abduction
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 肩外展
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.A-II-a-shoulder-abduction)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-II-a-shoulder-outwards-rotation
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 肩膀外旋
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.A-II-a-shoulder-outwards-rotation)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-II-a-elbow-flexion
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 手肘屈曲
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.A-II-a-elbow-flexion)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-II-a-forearm-supination
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 前臂旋後
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.A-II-a-forearm-supination)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-group.png)A-II-b-FMAUEMotion
  * [Text](https://hl7.org/fhir/R4/formats.html#table): II.b.伸肌協同動作
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [group](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-group)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-II-b-shoulder-add-inward-rotation
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 肩部內旋/外旋
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.A-II-b-shoulder-add-inward-rotation)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-II-b-elbow-extension
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 手肘伸展
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.A-II-b-elbow-extension)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-II-b-forearm-pronation
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 前臂旋前
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.A-II-b-forearm-pronation)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-group.png)A-III-FMAUEMotion
  * [Text](https://hl7.org/fhir/R4/formats.html#table): III.部份協同動作（不可代償）
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [group](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-group)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-III-hand-to-lumbar-spine
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 手到腰椎
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.A-III-hand-to-lumbar-spine)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-III-shoulder-flexion-0-90
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 肩部屈曲0° - 90°
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.A-III-shoulder-flexion-0-90)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-III-elbow-pro-supination
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 手肘 90° 前傾/旋後
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.A-III-elbow-pro-supination)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-group.png)A-IV-FMAUEMotion
  * [Text](https://hl7.org/fhir/R4/formats.html#table): IV.自主運動
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [group](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-group)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-IV-shoulder-abduction-0-90
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 肩外展 0° - 90°
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.A-IV-shoulder-abduction-0-90)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-IV-shoulder-flexion-90-180
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 肩部屈曲90°-180°
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.A-IV-shoulder-flexion-90-180)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-IV-elbow-0-pronation-supination
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 手肘 0° 前傾/旋後
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.A-IV-elbow-0-pronation-supination)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-group.png)A-V-FMAUEMotion
  * [Text](https://hl7.org/fhir/R4/formats.html#table): V.反射強度
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [group](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-group)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)A-V-normal-reflex-activity
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 正常反射活動（屈肌/伸肌）
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.A-V-normal-reflex-activity)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-group.png)B-wrist-hand
  * [Text](https://hl7.org/fhir/R4/formats.html#table): B.手腕/手部
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [group](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-group)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-group.png)B-I-FMAUEMotion
  * [Text](https://hl7.org/fhir/R4/formats.html#table): I.手腕穩定度
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [group](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-group)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-I-elbow-90-wrist-stability
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 手肘 90° 腕部穩定性
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.B-I-elbow-90-wrist-stability)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-I-elbow-90-wrist-flex-extension
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 手肘 90° 腕關節屈曲/伸展
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.B-I-elbow-90-wrist-flex-extension)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-I-elbow-0-wrist-stability
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 手肘 0° 腕部穩定性
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.B-I-elbow-0-wrist-stability)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-I-elbow-0-wrist-flex-extension
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 手肘 0° 腕部屈曲/伸展
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.B-I-elbow-0-wrist-flex-extension)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-I-wrist-circumduction
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 腕部旋轉
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.B-I-wrist-circumduction)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-group.png)B-II-FMAUEMotion
  * [Text](https://hl7.org/fhir/R4/formats.html#table): II.手指伸屈
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [group](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-group)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-II-fingers-mass-flexion
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 手指屈曲
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.B-II-fingers-mass-flexion)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-II-fingers-mass-extension
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 手指伸展
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.B-II-fingers-mass-extension)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-group.png)B-III-FMAUEMotion
  * [Text](https://hl7.org/fhir/R4/formats.html#table): III.抓握功能
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [group](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-group)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-III-grasp-a
  * [Text](https://hl7.org/fhir/R4/formats.html#table): a. MP 關節伸展，PIP 和 DIP 彎曲；測試抓握力是否抵抗阻力
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.B-III-grasp-a)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-III-grasp-b
  * [Text](https://hl7.org/fhir/R4/formats.html#table): b. 指導患者將拇指內收，其他關節在 0° 位置
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.B-III-grasp-b)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-III-grasp-c
  * [Text](https://hl7.org/fhir/R4/formats.html#table): c. 食指拇指肚對著，中間插一支鉛筆
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.B-III-grasp-c)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-III-grasp-d
  * [Text](https://hl7.org/fhir/R4/formats.html#table): d. 患者用食指和中指的掌側表面互相抵住，抓住一個圓柱形物體（小罐子）。
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.B-III-grasp-d)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)B-III-grasp-e
  * [Text](https://hl7.org/fhir/R4/formats.html#table): e. 球形抓握；病人抓住一個網球
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.B-III-grasp-e)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-group.png)C-coordination-speed
  * [Text](https://hl7.org/fhir/R4/formats.html#table): C.協調性/速度
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [group](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-group)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)C-I-finger-to-nose-tremor
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 手指觸碰鼻子：顫抖
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.C-I-finger-to-nose-tremor)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)C-I-finger-to-nose-dysmetria
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 手指觸鼻：辨距不良
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.C-I-finger-to-nose-dysmetria)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-coding.png)C-I-finger-to-nose-time
  * [Text](https://hl7.org/fhir/R4/formats.html#table): 手指到鼻子：時間
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 1..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [choice](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-choice)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): 
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): Options:[3 options](#opt-item.C-I-finger-to-nose-time)
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](icon-q-integer.png)D-total-score-FMAUEMotion
  * [Text](https://hl7.org/fhir/R4/formats.html#table): D.FMAUE動作總分
  * [Cardinality](https://hl7.org/fhir/R4/formats.html#table): 0..1
  * [Type](https://hl7.org/fhir/R4/formats.html#table): [integer](https://hl7.org/fhir/R4/codesystem-item-type.html#item-type-integer)
  * [Flags](https://hl7.org/fhir/R4/formats.html#table): ![](icon-qi-readonly.png)![](icon-qi-readonly.png)
  * [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC): 
* [LinkID](https://hl7.org/fhir/R4/formats.html#table): ![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3goXBCwdPqAP0wAAAldJREFUOMuNk0tIlFEYhp9z/vE2jHkhxXA0zJCMitrUQlq4lnSltEqCFhFG2MJFhIvIFpkEWaTQqjaWZRkp0g26URZkTpbaaOJkDqk10szoODP//7XIMUe0elcfnPd9zsfLOYplGrpRwZaqTtw3K7PtGem7Q6FoidbGgqHVy/HRb669R+56zx7eRV1L31JGxYbBtjKK93cxeqfyQHbehkZbUkK20goELEuIzEd+dHS+qz/Y8PTSif0FnGkbiwcAjHaU1+QWOptFiyCLp/LnKptpqIuXHx6rbR26kJcBX3yLgBfnd7CxwJmflpP2wUg0HIAoUUpZBmKzELGWcN8nAr6Gpu7tLU/CkwAaoKTWRSQyt89Q8w6J+oVQkKnBoblH7V0PPvUOvDYXfopE/SJmALsxnVm6LbkotrUtNowMeIrVrBcBpaMmdS0j9df7abpSuy7HWehwJdt1lhVwi/J58U5beXGAF6c3UXLycw1wdFklArBn87xdh0ZsZtArghBdAA3+OEDVubG4UEzP6x1FOWneHh2VDAHBAt80IbdXDcesNoCvs3E5AFyNSU5nbrDPZpcUEQQTFZiEVx+51fxMhhyJEAgvlriadIJZZksRuwBYMOPBbO3hePVVqgEJhFeUuFLhIPkRP6BQLIBrmMenujm/3g4zc398awIe90Zb5A1vREALqneMcYgP/xVQWlG+Ncu5vgwwlaUNx+3799rfe96u9K0JSDXcOzOTJg4B6IgmXfsygc7/Bvg9g9E58/cDVmGIBOP/zT8Bz1zqWqpbXIsd0O9hajXfL6u4BaOS6SeWAAAAAElFTkSuQmCC)Documentation for this format

-------

**Options Sets**

**Answer options for assessment-phase-fmaue-motion**

* 初評
* 期中
* 延展
* 結案

**Answer options for assessment-side-fmaue-motion**

* http://snomed.info/sct#24028007 ("患者左側")
* http://snomed.info/sct#7771000 ("患者右側")

**Answer options for A-I-a-flexors**

* 0
* 2

**Answer options for A-I-a-extensors**

* 0
* 2

**Answer options for A-II-a-shoulder-retraction**

* 0
* 1
* 2

**Answer options for A-II-a-shoulder-elevation**

* 0
* 1
* 2

**Answer options for A-II-a-shoulder-abduction**

* 0
* 1
* 2

**Answer options for A-II-a-shoulder-outwards-rotation**

* 0
* 1
* 2

**Answer options for A-II-a-elbow-flexion**

* 0
* 1
* 2

**Answer options for A-II-a-forearm-supination**

* 0
* 1
* 2

**Answer options for A-II-b-shoulder-add-inward-rotation**

* 0
* 1
* 2

**Answer options for A-II-b-elbow-extension**

* 0
* 1
* 2

**Answer options for A-II-b-forearm-pronation**

* 0
* 1
* 2

**Answer options for A-III-hand-to-lumbar-spine**

* 0
* 1
* 2

**Answer options for A-III-shoulder-flexion-0-90**

* 0
* 1
* 2

**Answer options for A-III-elbow-pro-supination**

* 0
* 1
* 2

**Answer options for A-IV-shoulder-abduction-0-90**

* 0
* 1
* 2

**Answer options for A-IV-shoulder-flexion-90-180**

* 0
* 1
* 2

**Answer options for A-IV-elbow-0-pronation-supination**

* 0
* 1
* 2

**Answer options for A-V-normal-reflex-activity**

* 0
* 1
* 2

**Answer options for B-I-elbow-90-wrist-stability**

* 0
* 1
* 2

**Answer options for B-I-elbow-90-wrist-flex-extension**

* 0
* 1
* 2

**Answer options for B-I-elbow-0-wrist-stability**

* 0
* 1
* 2

**Answer options for B-I-elbow-0-wrist-flex-extension**

* 0
* 1
* 2

**Answer options for B-I-wrist-circumduction**

* 0
* 1
* 2

**Answer options for B-II-fingers-mass-flexion**

* 0
* 1
* 2

**Answer options for B-II-fingers-mass-extension**

* 0
* 1
* 2

**Answer options for B-III-grasp-a**

* 0
* 1
* 2

**Answer options for B-III-grasp-b**

* 0
* 1
* 2

**Answer options for B-III-grasp-c**

* 0
* 1
* 2

**Answer options for B-III-grasp-d**

* 0
* 1
* 2

**Answer options for B-III-grasp-e**

* 0
* 1
* 2

**Answer options for C-I-finger-to-nose-tremor**

* 0
* 1
* 2

**Answer options for C-I-finger-to-nose-dysmetria**

* 0
* 1
* 2

**Answer options for C-I-finger-to-nose-time**

* 0
* 1
* 2



## Resource Content

```json
{
  "resourceType" : "Questionnaire",
  "id" : "FMAUEMotorQuestionnaireInstance",
  "meta" : {
    "profile" : ["http://example.org/StructureDefinition/SPACQuestionnaire"]
  },
  "url" : "http://example.org/Questionnaire/FMAUEMotorQuestionnaireInstance",
  "version" : "0.1.0",
  "name" : "FMAUEMotorQuestionnaire",
  "title" : "Fugl-Meyer上肢動作評估問卷",
  "status" : "active",
  "subjectType" : ["Patient"],
  "date" : "2025-10-01",
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
  "description" : "衛福部Fugl-Meyer上肢動作評估問卷，總分66分",
  "purpose" : "提供標準化的上肢動作功能評估工具，用於中風復健評估",
  "item" : [
    {
      "linkId" : "assessment-phase-fmaue-motion",
      "text" : "請選擇評估階段",
      "type" : "choice",
      "required" : true,
      "answerOption" : [
        {
          "valueString" : "初評"
        },
        {
          "valueString" : "期中"
        },
        {
          "valueString" : "延展"
        },
        {
          "valueString" : "結案"
        }
      ]
    },
    {
      "linkId" : "assessment-side-fmaue-motion",
      "text" : "請選擇患側",
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
      "linkId" : "A-shoulder-elbow-forearm",
      "text" : "A.肩部/肘部/前臂",
      "type" : "group",
      "required" : true,
      "item" : [
        {
          "linkId" : "A-I-FMAUEMotion",
          "text" : "I.反射反應",
          "type" : "group",
          "required" : true,
          "item" : [
            {
              "linkId" : "A-I-a-flexors",
              "text" : "二頭肌或手指屈肌",
              "type" : "choice",
              "required" : true,
              "answerOption" : [
                {
                  "valueInteger" : 0
                },
                {
                  "valueInteger" : 2
                }
              ]
            },
            {
              "linkId" : "A-I-a-extensors",
              "text" : "三頭肌",
              "type" : "choice",
              "required" : true,
              "answerOption" : [
                {
                  "valueInteger" : 0
                },
                {
                  "valueInteger" : 2
                }
              ]
            }
          ]
        },
        {
          "linkId" : "A-II-a-FMAUEMotion",
          "text" : "II.a.屈肌協同動作",
          "type" : "group",
          "required" : true,
          "item" : [
            {
              "linkId" : "A-II-a-shoulder-retraction",
              "text" : "肩部回縮",
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
                }
              ]
            },
            {
              "linkId" : "A-II-a-shoulder-elevation",
              "text" : "肩部抬高",
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
                }
              ]
            },
            {
              "linkId" : "A-II-a-shoulder-abduction",
              "text" : "肩外展",
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
                }
              ]
            },
            {
              "linkId" : "A-II-a-shoulder-outwards-rotation",
              "text" : "肩膀外旋",
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
                }
              ]
            },
            {
              "linkId" : "A-II-a-elbow-flexion",
              "text" : "手肘屈曲",
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
                }
              ]
            },
            {
              "linkId" : "A-II-a-forearm-supination",
              "text" : "前臂旋後",
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
                }
              ]
            }
          ]
        },
        {
          "linkId" : "A-II-b-FMAUEMotion",
          "text" : "II.b.伸肌協同動作",
          "type" : "group",
          "required" : true,
          "item" : [
            {
              "linkId" : "A-II-b-shoulder-add-inward-rotation",
              "text" : "肩部內旋/外旋",
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
                }
              ]
            },
            {
              "linkId" : "A-II-b-elbow-extension",
              "text" : "手肘伸展",
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
                }
              ]
            },
            {
              "linkId" : "A-II-b-forearm-pronation",
              "text" : "前臂旋前",
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
                }
              ]
            }
          ]
        },
        {
          "linkId" : "A-III-FMAUEMotion",
          "text" : "III.部份協同動作（不可代償）",
          "type" : "group",
          "required" : true,
          "item" : [
            {
              "linkId" : "A-III-hand-to-lumbar-spine",
              "text" : "手到腰椎",
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
                }
              ]
            },
            {
              "linkId" : "A-III-shoulder-flexion-0-90",
              "text" : "肩部屈曲0° - 90°",
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
                }
              ]
            },
            {
              "linkId" : "A-III-elbow-pro-supination",
              "text" : "手肘 90° 前傾/旋後",
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
                }
              ]
            }
          ]
        },
        {
          "linkId" : "A-IV-FMAUEMotion",
          "text" : "IV.自主運動",
          "type" : "group",
          "required" : true,
          "item" : [
            {
              "linkId" : "A-IV-shoulder-abduction-0-90",
              "text" : "肩外展 0° - 90°",
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
                }
              ]
            },
            {
              "linkId" : "A-IV-shoulder-flexion-90-180",
              "text" : "肩部屈曲90°-180°",
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
                }
              ]
            },
            {
              "linkId" : "A-IV-elbow-0-pronation-supination",
              "text" : "手肘 0° 前傾/旋後",
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
                }
              ]
            }
          ]
        },
        {
          "linkId" : "A-V-FMAUEMotion",
          "text" : "V.反射強度",
          "type" : "group",
          "required" : true,
          "item" : [
            {
              "linkId" : "A-V-normal-reflex-activity",
              "text" : "正常反射活動（屈肌/伸肌）",
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
                }
              ]
            }
          ]
        }
      ]
    },
    {
      "linkId" : "B-wrist-hand",
      "text" : "B.手腕/手部",
      "type" : "group",
      "required" : true,
      "item" : [
        {
          "linkId" : "B-I-FMAUEMotion",
          "text" : "I.手腕穩定度",
          "type" : "group",
          "required" : true,
          "item" : [
            {
              "linkId" : "B-I-elbow-90-wrist-stability",
              "text" : "手肘 90° 腕部穩定性",
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
                }
              ]
            },
            {
              "linkId" : "B-I-elbow-90-wrist-flex-extension",
              "text" : "手肘 90° 腕關節屈曲/伸展",
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
                }
              ]
            },
            {
              "linkId" : "B-I-elbow-0-wrist-stability",
              "text" : "手肘 0° 腕部穩定性",
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
                }
              ]
            },
            {
              "linkId" : "B-I-elbow-0-wrist-flex-extension",
              "text" : "手肘 0° 腕部屈曲/伸展",
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
                }
              ]
            },
            {
              "linkId" : "B-I-wrist-circumduction",
              "text" : "腕部旋轉",
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
                }
              ]
            }
          ]
        },
        {
          "linkId" : "B-II-FMAUEMotion",
          "text" : "II.手指伸屈",
          "type" : "group",
          "required" : true,
          "item" : [
            {
              "linkId" : "B-II-fingers-mass-flexion",
              "text" : "手指屈曲",
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
                }
              ]
            },
            {
              "linkId" : "B-II-fingers-mass-extension",
              "text" : "手指伸展",
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
                }
              ]
            }
          ]
        },
        {
          "linkId" : "B-III-FMAUEMotion",
          "text" : "III.抓握功能",
          "type" : "group",
          "required" : true,
          "item" : [
            {
              "linkId" : "B-III-grasp-a",
              "text" : "a. MP 關節伸展，PIP 和 DIP 彎曲；測試抓握力是否抵抗阻力",
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
                }
              ]
            },
            {
              "linkId" : "B-III-grasp-b",
              "text" : "b. 指導患者將拇指內收，其他關節在 0° 位置",
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
                }
              ]
            },
            {
              "linkId" : "B-III-grasp-c",
              "text" : "c. 食指拇指肚對著，中間插一支鉛筆",
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
                }
              ]
            },
            {
              "linkId" : "B-III-grasp-d",
              "text" : "d. 患者用食指和中指的掌側表面互相抵住，抓住一個圓柱形物體（小罐子）。",
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
                }
              ]
            },
            {
              "linkId" : "B-III-grasp-e",
              "text" : "e. 球形抓握；病人抓住一個網球",
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
                }
              ]
            }
          ]
        }
      ]
    },
    {
      "linkId" : "C-coordination-speed",
      "text" : "C.協調性/速度",
      "type" : "group",
      "required" : true,
      "item" : [
        {
          "linkId" : "C-I-finger-to-nose-tremor",
          "text" : "手指觸碰鼻子：顫抖",
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
            }
          ]
        },
        {
          "linkId" : "C-I-finger-to-nose-dysmetria",
          "text" : "手指觸鼻：辨距不良",
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
            }
          ]
        },
        {
          "linkId" : "C-I-finger-to-nose-time",
          "text" : "手指到鼻子：時間",
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
            }
          ]
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
      "linkId" : "D-total-score-FMAUEMotion",
      "text" : "D.FMAUE動作總分",
      "type" : "integer",
      "readOnly" : true
    }
  ]
}

```
