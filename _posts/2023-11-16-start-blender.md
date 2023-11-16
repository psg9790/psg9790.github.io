---
title:  "[Blender] 블렌더 231116"
excerpt: "블렌더 첫시간 단축키 & 기능 배우기"

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
  - **tab** : 모드 전환 (object - edit) (text input)  
  - **/** : 해당 오브젝트만 보기  
  - **z** : 렌더 모드  
  - **m (inspector)** : collection 묶기  
  - **h** : Hide, 씬에서 숨김
- **<span style="color:orange">side 9 num</span>**  
  - **1(back),3(right),7(top),0(camera)** : 시점 변환  
  - **2,4,6,8** : 특정 각도로 돌리고 싶을 때  
  - **.** : 해당 오브젝트를 중앙으로 설정  
- **<span style="color:orange">select</span>**  
  - **shift+a** : 물체 추가  
  - **ctrl+ +** : 근방의 다른 요소 추가  
  - **ctrl+ -** : 근방의 다른 요소 제거  
  - **1 (edit mode)** : vertex(점)  
  - **2 (edit mode)** : edge(선)  
  - **3 (edit mode)** : surface(면)  
  - **g** : Move(이동)  
  - **r** : Rotate(회전)  
  - **s** : Scale(스케일)  
*(각 g, r, s 동작은 x, y, z 버튼을 추가로 눌러 적용되는 축을 제한할 수 있음)*  
  - **ctrl+j** : Join, 두 물체를 하나로 합침  
  - **p** : Seperate, 합친 물체를 분리  
  - **e** : Extrude, 확장  
  - **i** : Inset, 평행하게 면 하나 더 생성  
  - **ctrl+b** : Bevel, 부드러운 코너 깎기  
  - **ctrl+r** : insert loop edge, scroll로 개수 추가 가능  
  - **m (perspective)** : Merge, 두 정점 가운데로 합치기  
- **<span style="color:orange">scroll</span>**   
  - **scroll(click)** : 회전  
  - **shift+scroll(click)** : 이동  
  - **alt+scroll(click)** : 평면 회전  
  - **ctrl+scroll(click) || scroll(roll)** : 확대 축소 
  
   
## Modifier  
- **Array** : 규칙적이고 반복적으로 모델 배치... 귀찮은 반복작업 대신 사용    
- **Bevel** : 모델의 전체 엣지를 Bevel  
- **Boolean** : 합집합, 합치기, 차집합... 모델 수정 가능  
- **Build** : 애니메이션처럼... 시간의 흐름에 따라 모델을 순차로 렌더링 가능  
- **Decimate** : lowpoly화... 최적화에 사용  
- **Edge Split** : 모든 엣지 분리... 설정한 각도 이상의 엣지들이 분리됨, 분리된 엣지의 면을 모델에서 떼어내기 가능  
- **Mask** : Weight Paint로 설정한 가중치에 따라 모델의 일부를 지울 수 있음  
- **Mirror** : 타겟 위치를 잡고 대칭 모델링을 만들 수 있음  
- **Subdivision Surface** : 부드러운 면이 되도록 폴리곤들을 쪼개줌, Bevel(ctrl+b)과 Edge Loop(ctrl+_r)로 억제 가능  
- **MultiResolution** : 둥글어지게 모델을 깎아줌? Subdivision 과의 차이점은 적용&적용해제를 왔다갔다 할 수 있다... sculpt mode에서 조각할 수 있다
- **Screw** : 2D 선으로 면을 확장해 드릴 만들 수 있음  
- **Solidify** : 모델의 두께를 만들 수 있음  
- **Triangulate** : 모델의 메시를 보다 세밀한 삼각 메시 두 개로 쪼개줌  
- **Weld** : 설정한 거리보다 짧은 거리의 두 점을 합침  
- **Wireframe** : Plane -> Subdivide 12 -> Poke Faces -> Tris to Quads -> Wireframe modifier, 쉽게 철조망 만들 수 있음  
- **Curve** : 2D 선 오브젝트를 따라 3D 오브젝트의 모양을 맞출 수 있음  
- **Cast** : 타겟을 중심으로 원하는 모양을 만들어줌  
- **Displace** : 텍스쳐로 모델에 bumping 변형을 줄 수 있음
- **Hook** : Weight Paint 후 타겟을 정하면, 그 타겟을 움직여 물체를 끌고 다닐 수 있음, paint 값에 따라 끌려다니는 정도가 달라짐
- **Lattice** : 모델링에 틀을 씌움, 씌운 틀의 정점을 움직이면 내부에 담긴 모델링도 따라 움직임
- **ShrinkWrap** : Sphere위에 Plane을 덮는 예제, 옷이나 가면에 사용 가능
- **SimpleDeform** : 간단히 면을 뒤틀거나, 변형하고 싶을 때 사용
- **SurfaceDeform** : bind 후 다른 모델의 면을 뒤틂에 따라 현재 모델의 면을 동시에 뒤틀 수 있음