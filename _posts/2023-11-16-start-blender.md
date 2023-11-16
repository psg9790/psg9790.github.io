---
title:  "[Blender] 블렌더 첫시간"
excerpt: "블렌더 첫시간 단축키 배우기"

categories:
  - Blender
tags:
  - [Blender]

toc: true
toc_sticky: true
 
date: 2023-11-16 09:30:00+0900
last_modified_at: 2023-11-16 09:30:00+0900
---

## 단축키 (shortcuts)  
- **<span style="color:orange">mode</span>**  
**[ tab ]** : 모드 전환 (object - edit) (text input) 
**[ ctrl+tab ]** : 여러 모드 선택  
**[ / ]** : 해당 오브젝트만 보기  
**[ z ]** : 렌더 모드  
**[ m ] (inspector)** : collection 묶기  
- **<span style="color:orange">select</span>**  
**[ shift+a ]** : 물체 추가  
**[ ctrl+ + ]** : 근방의 다른 요소들을 추가할 수 있음  
**[ ctrl+ - ]** : 추가한 근방의 다른 요소들을 제거할 수 있음  
**[ 1 ] (edit mode)** : vertex(점)  
**[ 2 ] (edit mode)** : edge(선)  
**[ 3 ] (edit mode)** : surface(면)  
**[ g ]** : Move(이동)  
**[ r ]** : Rotate(회전)  
**[ s ]** : Scale(스케일)  
*(각 g, r, s 동작은 x,y,z 버튼을 추가로 눌러 적용되는 축을 제한할 수 있음)*  
**[ ctrl+j ]** : Join, 두 물체를 합침  
**[ p ]** : Seperate, 합친 물체를 분리  
**[ e ]** : Extrude, 확장  
**[ i ]** : Inset,  
**[ ctrl+b ]** : Bevel,  
**[ m ] (perspective)** : Merge,  
**[ ctrl+r ]** : insert loop edge, scroll로 개수 추가  
**[ h ]** : Hide
- **<span style="color:orange">scroll</span>**   
**[ scroll(click) ]** : 회전  
**[ shift+scroll ]** : 이동  
**[ alt+scroll ]** : 평면 회전  
**[ ctrl+scroll(click) || scroll(roll) ]** : 확대 축소  
- **<span style="color:orange">side 9 num</span>**  
**[ 1(back),3(right),7(top),0(camera) ]** : 시점 변환  
**[ 2,4,6,8 ]** : 특정 각도로 돌리고 싶을 때  
**[ . ]** : 해당 오브젝트를 중앙으로 설정  

## Modifier
Array: 규칙적이고 반복적으로... 복사 가능
Bevel: 전체 베벨...
Boolean: 합집합, 합치기, 차집합... 으로 모델 수정
Build: 애니메이션... 처럼 보임
Decimate: 로우폴리화... 최적화에 사용
Edge Split: 모든 엣지 분리... 해당 각도 이상의 엣지들을 분리시킬 수 있음, 면 떼어내기 가능
Mask: Weight Paint로 설정한 가중치로 메쉬를 지울 수 있음
Mirror: 중심축을 잡고 거울상 맺을 수 있음
Subdivision Surface: 부드러운 면이 되도록 폴리곤들을 쪼개줌, Bevel과 Edge Loop로 억제 가능
MultiResolution: 구형이 되도록 폴리곤들을 쪼개줌? Subdivision 과의 차이점은 왔다갔다 할 수 있다... sculpt mode에서 조각할 수 있고 원하는 만큼 테스트해볼 수 있음
Screw: 2D 선으로 드릴 만들 수 있음
Solidify: 두께 만들 수 있음
Triangulate: 사각 메시를 삼각 두개로 쪼개줌
Weld: 설정한 거리보다 짧은 거리의 두 점을 합침
Wireframe: Plane -> Subdivide 12 -> Poke Faces -> Tris to Quads -> Wireframe modifier
Curve: 2D 선 위에 3D 오브젝트의 모양을 맞출 수 있음
Cast: 타겟을 중심으로 원하는 모양을 만들어줌